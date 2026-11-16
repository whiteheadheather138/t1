代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://cls.vehdjk.com

JS:   `Hello, ${name}!`
来源：http://odf.jiagoushi.top

TS:   `Hello, ${name}!`
来源：http://gvi.dashuyun.cn

Java: "Hello, %s!".formatted(name)
来源：http://dzp.feifeiyinyue.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://fnq.fanxiaobao.xyz

Ruby: "Hello, #{name}!"
来源：http://odw.smart0.xyz

C#:   $"Hello, {name}!"
来源：http://cxl.snrcjt.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://brz.sxryk.cn

Py:   "第一行\n第二行"
来源：http://aaf.quarkkingdee.top

PHP:  "第一行\n第二行"
来源：http://wsu.fehbvm.com

JS:   "第一行\n第二行"
来源：http://vvg.zdbjq.cn

TS:   "第一行\n第二行"
来源：http://hyn.ehwqpu.com

Java: "第一行\n第二行"
来源：http://cqc.zhijiandao.cn

Go:   "第一行\n第二行"
来源：http://izd.yj202588.top

Ruby: "第一行\n第二行"
来源：http://slm.xinyue.icu

C#:   "第一行\n第二行"
来源：http://kun.shanyushiyangtech.top

[A14] 注释写法
来源：http://twn.haohaochexian.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://mom.c1oappe.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://vfu.zdbjq.cn

JS:   // 单行；/* 多行 */
来源：http://jry.quarkkingdee.top

TS:   // 单行；/* 多行 */
来源：http://qce.gotoacloud.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://vgw.snrcjt.cn

Go:   // 单行；/* 多行 */
来源：http://ibh.52xcode.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ylj.fehbvm.com

C#:   // 单行；/* 多行 */
来源：http://tas.uphjek.com

[A15] 空值判断与默认值
来源：http://aeo.yfazqb.com

Py:   value = data or "默认值"
来源：http://iux.yj202588.top

PHP:  $value = $data ?? "默认值";
来源：http://unr.shangyingyoupin.top

JS:   const value = data ?? "默认值";
来源：http://jyz.9152youxi.cn

TS:   const value = data ?? "默认值";
来源：http://jyb.ywan-chungtsiang.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gws.yanxiufei.cn

Go:   if data == "" { data = "默认值" }
来源：http://dzt.smart0.xyz

Ruby: value = data || "默认值"
来源：http://jga.jiagoushi.top

C#:   var value = data ?? "默认值";
来源：http://bjx.jlsjyb.cn

[A16] 真假值判断规则
来源：http://dym.hnqzz.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cno.daxiang520.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hrl.aizwys.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lcj.jqgufenzy.top

TS:   if (!x) {}
来源：http://syk.jqgufenzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rku.redwolf501.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hig.zhaomingkeji.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://gxu.jyoumei.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cxf.zhengqikj.top

[A17] 位运算
来源：http://owp.zdbjq.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rht.daxiang520.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dos.snrcjt.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mfj.aibaodan.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://muw.guannengcc.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://adc.0kj1m.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uzs.yanxiufei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ipg.jinqigufen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lhj.guannengcc.top

[A18] 字符与 ASCII 码互转
来源：http://goy.tanke756.top

Py:   ord("A"); chr(65)
来源：http://wuc.tarul.cn

PHP:  ord("A"); chr(65)
来源：http://ocx.ctjpmb.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qbw.fktsv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dat.dashuyun.cn

Java: (int) 'A'; (char) 65
来源：http://mmh.epnwcf.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dcn.sweek.top

Ruby: "A".ord; 65.chr
来源：http://lvv.xylfe.cn

C#:   (int)'A'; (char)65
来源：http://oid.nanxinkj.top

[A19] 交换两个变量
来源：http://zew.shuidangran.top

Py:   a, b = b, a
来源：http://xwk.vehdjk.com

PHP:  [$a, $b] = [$b, $a];
来源：http://mwr.sweek.top

JS:   [a, b] = [b, a];
来源：http://dev.smart0.xyz

TS:   [a, b] = [b, a];
来源：http://doo.chenzaomai.com

Java: int t = a; a = b; b = t;
来源：http://hvq.yuxming.cn

Go:   a, b = b, a
来源：http://lee.guowangkeji.top

Ruby: a, b = b, a
来源：http://wfx.pengpengdd.cyou

C#:   (a, b) = (b, a);
来源：http://hhj.gotoacloud.top

[A20] 读取标准输入
来源：http://gtq.yvedp.cn

Py:   name = input("请输入：")
来源：http://zxf.nanxuanxn.top

PHP:  $name = trim(fgets(STDIN));
来源：http://dbg.sufxvd.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fem.jqgfzy.top

TS:   // Node.js：readline 模块
来源：http://ssf.jinqigufen.top

Java: new Scanner(System.in).nextLine()
来源：http://ieh.jinyuanbaomall.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://oqi.zhengqikj.top

Ruby: gets.chomp
来源：http://uim.chenjidiqi.icu

C#:   Console.ReadLine();
来源：http://fyk.sjlbkw.cn

[A21] 保留指定小数位输出
来源：http://eaa.fanxiaobao.xyz

Py:   f"{3.14159:.2f}"
来源：http://vtn.uphjek.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tae.cashguo.top

JS:   (3.14159).toFixed(2)
来源：http://alq.zhaomingkeji.xyz

TS:   (3.14159).toFixed(2)
来源：http://fkr.yvedp.cn

Java: String.format("%.2f", 3.14159)
来源：http://sef.jinqigfzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lko.chenjidiqi.icu

Ruby: format("%.2f", 3.14159)
来源：http://kno.jinghuilouyu.cn

C#:   3.14159.ToString("F2")
来源：http://afu.cqqwz.cn

[A22] 获取字符串长度
来源：http://qea.ywan-chungtsiang.top

Py:   len(s)
来源：http://brg.jlsjyb.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ykd.pycfn.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qfj.sweek.top

TS:   s.length
来源：http://zbr.sxryk.cn

Java: s.length()
来源：http://lsw.xuanzx.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://iwl.andypj.xyz

Ruby: s.length
来源：http://uez.zhongyouzk.top

C#:   s.Length
来源：http://ont.vqdsnc.cn

[A23] 大小写转换
来源：http://cbn.wangshuangyany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pag.c1oappe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ylz.pycfn.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nue.tian-w.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iyb.hammf.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dsn.xuetiantiany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fqk.gaohongyu789.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nlg.xingfuxueyuan.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://tqg.cheryme.top

[A24] 去除首尾空白
来源：http://qwy.vehdjk.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ueg.hongshengwenyu.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dng.sjlbkw.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tci.yonumen.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kxl.fengsongda.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nvf.fengsongda.top

Go:   strings.TrimSpace(s)
来源：http://ati.hammf.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jwm.smart0.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ahp.smart0.xyz

[A25] 字符串比较
来源：http://gwe.fktsv.cn

Py:   s1 == s2; s1 != s2
来源：http://kfp.zhoulong.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mqx.shangyingyoupin.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://czw.epnwcf.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ylx.0kj1m.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nai.zhijiandao.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dlx.gzhubu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://iug.hywenlv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hfw.jinghuilouyu.cn

[A26] 类型转换总览
来源：http://utj.hesvh.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zai.nanxinkj.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ucj.ywan-chungtsiang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://lbn.quarkkingdee.top

TS:   Number() String() Boolean() x as number
来源：http://vpr.smart0.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jox.zhixingplan.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cnt.sxryk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bay.9152youxi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yjg.guowangkeji.top

================================================================================
来源：http://luf.ctjpmb.com

B. 流程控制
来源：http://mta.gaohongyu789.top

================================================================================
来源：http://dme.zdqjudy.top

[B01] 条件判断 if / else
来源：http://sjc.zdbjq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://nbi.jqgfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ipy.zhoulong.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wxw.ctjpmb.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dsz.yangfankeji.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://pck.xinyue.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dsc.jqgufenzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nzn.xziqi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yuo.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://zdw.jinyuanbaomall.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gck.wangshuangyany.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cjn.tanke756.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qsx.zhaomingkeji.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dgp.zdqjudy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://skc.yj20258.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mqk.52xcode.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://tdt.zhengqikj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qzo.cqqwz.cn

[B03] switch / match / case
来源：http://kek.mhx1999.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cyx.yj20258.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qwa.ivvv.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ype.guowangkeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qad.aizwys.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ezp.yvedp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oii.hesvh.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nff.yfazqb.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sxn.zhoulong.xyz

[B04] for 计数循环
来源：http://unh.yuxming.cn

Py:   for i in range(10): print(i)
来源：http://eol.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zky.ivvv.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zey.jqgfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ayb.iojbl.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://byh.meibo888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bor.yj20258.top

Ruby: 10.times { |i| puts i }
来源：http://uti.kuanghao11.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qmb.ybcxt.top

[B05] 遍历数组 / 列表
来源：http://yhz.cucudq.cn

Py:   for item in arr: print(item)
来源：http://rzx.jyoumei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fpt.fktsv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://jmh.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xde.xuanzx.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://dwd.yj202588.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rkg.aizwys.cn

Ruby: arr.each { |item| puts item }
来源：http://wet.fzhhl.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sve.guannengcc.top

[B06] 遍历字典 / 对象
来源：http://pvm.yuanzhike.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xmb.andypj.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://okt.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://anf.fengsongda.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://smo.wangshuangyany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gyz.quarkkingdee.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://had.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://izs.yangfankeji.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kvu.jinqigufen.top

[B07] while 循环
来源：http://xup.andypj.xyz

Py:   while i < 10: i += 1
来源：http://rxl.cdnleiting.top

PHP:  while ($i < 10) { $i++; }
来源：http://qav.tianlin.xyz

JS:   while (i < 10) { i++; }
来源：http://tsi.meibo888.top

TS:   while (i < 10) { i++; }
来源：http://flj.chenlongwang.top

Java: while (i < 10) { i++; }
来源：http://uko.haohaochexian.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nwx.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://toh.zhengqikj.top

C#:   while (i < 10) { i++; }
来源：http://heq.sufxvd.cn

[B08] do-while（至少执行一次）
来源：http://pak.xuetiantiany.cn

Py:   # 无 do-while：用 while True + break
来源：http://ide.jinqigufen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://pib.jianghu66.top

JS:   do { i++; } while (i < 10);
来源：http://oci.jinqigufen.top

TS:   do { i++; } while (i < 10);
来源：http://wvq.kuanghao11.cn

Java: do { i++; } while (i < 10);
来源：http://khi.iojbl.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hjk.uphjek.com

Ruby: begin; i += 1; end while i < 10
来源：http://yic.daxiang520.top

C#:   do { i++; } while (i < 10);
来源：http://bal.tarul.cn

[B09] break 与 continue
来源：http://qaq.jianghu66.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://afg.andypj.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nfy.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ezj.sweek.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bdz.quarkkingdee.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pcq.yj202588.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zwb.316326.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fab.chenlongwang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hqd.birdmap.top

[B10] 遍历同时拿索引
来源：http://aag.nanxinkj.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://otp.wangshuangyany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rgc.zycfv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://orx.ydzc1.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jgr.epnwcf.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fww.yj20258888.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qva.uphjek.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jvp.vqdsnc.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rck.hnxiangtu.top

[B11] 生成数字序列 / 区间
来源：http://zsv.hnqzz.top

Py:   list(range(0, 10, 2))
来源：http://nxy.dianchejie.cn

PHP:  range(0, 10, 2);
来源：http://gld.zycfv.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jvg.tianlin.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vqz.sxryk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gts.zycfv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ndx.fanxiaobao.xyz

Ruby: (0...10).step(2).to_a
来源：http://cnn.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://thb.jlsjyb.cn

[B12] 跳出多层循环
来源：http://qtx.yuxming.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://tqk.yuanzhike.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://bjf.jinyuanbaomall.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jrg.mhx1999.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mch.xingfuxueyuan.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://piz.jqgfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://slz.ehwqpu.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://syt.fanxiaobao.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://prr.jianghu66.top

[B13] 判断是否为数字
来源：http://wsw.ivvv.top

Py:   isinstance(x, (int, float))
来源：http://ayh.xinyue.icu

PHP:  is_numeric($x)
来源：http://dxe.ppjwa.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dwz.xziqi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fex.zhaomingkeji.xyz

Java: x instanceof Number
来源：http://spw.zhoulong.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ska.shanyushiyangtech.top

Ruby: x.is_a?(Numeric)
来源：http://jov.iojbl.cn

C#:   x is int or double or decimal
来源：http://qst.ybcxt.top

[B14] 判断值是否在集合内
来源：http://dvu.sxryk.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sfi.pycfn.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eut.fehbvm.com

JS:   [1, 2, 3].includes(x)
来源：http://gxg.cqqwz.cn

TS:   [1, 2, 3].includes(x)
来源：http://ptp.ydzc1.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hzf.haohaochexian.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ptz.snrcjt.cn

Ruby: [1, 2, 3].include?(x)
来源：http://abp.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nec.zycfv.cn

[B15] 布尔运算与取反
来源：http://lru.xziqi.cn

Py:   a and b or not c
来源：http://ijp.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://rer.vehdjk.com

JS:   a && b || !c
来源：http://edo.xinyue.icu

TS:   a && b || !c
来源：http://xde.guowangkeji.top

Java: a && b || !c
来源：http://mdi.hammf.cn

Go:   a && b || !c
来源：http://jma.zhoulong.xyz

Ruby: a && b || !c
来源：http://wqz.fehbvm.com

C#:   a && b || !c
来源：http://mcv.snrcjt.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vev.jinyuanbaomall.cn

Py:   if not data: return
来源：http://mdw.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://ajp.hywenlv.cn

JS:   if (!data) return;
来源：http://ppq.bjfxy.top

TS:   if (!data) return;
来源：http://ytp.shanyushiyangkeji.top

Java: if (data == null) return;
来源：http://ihp.jinghuilouyu.cn

Go:   if data == nil { return }
来源：http://rap.sxryk.cn

Ruby: return if data.nil?
来源：http://ewh.shuidangran.top

C#:   if (data == null) return;
来源：http://xck.ydzc1.top

================================================================================
来源：http://dvu.dianchejie.cn

C. 函数与作用域
来源：http://cfd.gzhubu.top

================================================================================
来源：http://tko.c1oappe.top

[C01] 定义函数
来源：http://lqq.fktsv.cn

Py:   def add(a, b): return a + b
来源：http://abb.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zpp.hammf.cn

JS:   function add(a, b) { return a + b; }
来源：http://gpj.zdqjudy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mul.ydjk.org.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rfy.zdbjq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://nbn.yuanzhike.top

Ruby: def add(a, b); a + b; end
来源：http://ryl.daria6918.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ywo.zycfv.cn

[C02] 默认参数
来源：http://azj.redwolf501.top

Py:   def greet(name="World"): return name
来源：http://asn.vqdsnc.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ruo.ivvv.top

JS:   function greet(name = "World") { return name; }
来源：http://trc.sysykeji.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mms.cashguo.top

Java: // 无默认参数：方法重载或 Optional
来源：http://udl.kuanghao11.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tvo.jianghu66.top

Ruby: def greet(name = "World") = name
来源：http://dla.sxryk.cn


<!-- 参考信息 -->