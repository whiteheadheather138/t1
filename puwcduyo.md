代发 wailian999

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://obh.xuanzx.com

JS:   `Hello, ${name}!`
来源：http://tkt.xuetiantiany.cn

TS:   `Hello, ${name}!`
来源：http://ggn.shanyushiyangtech.top

Java: "Hello, %s!".formatted(name)
来源：http://beu.xinyue.icu

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wyk.wangshuangyany.cn

Ruby: "Hello, #{name}!"
来源：http://uaz.wangshuangyany.cn

C#:   $"Hello, {name}!"
来源：http://mog.fzhhl.top

[A13] 多行字符串（练习 \n 转义）
来源：http://svv.yj20258888.top

Py:   "第一行\n第二行"
来源：http://viz.hongshengwenyu.top

PHP:  "第一行\n第二行"
来源：http://vzo.yuanzhike.top

JS:   "第一行\n第二行"
来源：http://nhe.daria6918.cn

TS:   "第一行\n第二行"
来源：http://jfi.xziqi.cn

Java: "第一行\n第二行"
来源：http://wdx.zhoulong.xyz

Go:   "第一行\n第二行"
来源：http://zgc.bjfxy.top

Ruby: "第一行\n第二行"
来源：http://iad.yongpay.top

C#:   "第一行\n第二行"
来源：http://rtx.shanyushiyangtech.top

[A14] 注释写法
来源：http://kau.andypj.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://fex.snrcjt.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ipt.yangfankeji.com

JS:   // 单行；/* 多行 */
来源：http://hnp.mhx1999.top

TS:   // 单行；/* 多行 */
来源：http://gon.wangshuangyany.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dvq.jqgufenzy.top

Go:   // 单行；/* 多行 */
来源：http://cbp.jyoumei.cn

Ruby: # 单行；=begin 多行 =end
来源：http://sgr.ywan-chungtsiang.top

C#:   // 单行；/* 多行 */
来源：http://lms.dashuyun.cn

[A15] 空值判断与默认值
来源：http://gzo.chenlongwang.top

Py:   value = data or "默认值"
来源：http://rxe.jinqigfzy.top

PHP:  $value = $data ?? "默认值";
来源：http://jfr.jqgfzy.top

JS:   const value = data ?? "默认值";
来源：http://ohl.sjlbkw.cn

TS:   const value = data ?? "默认值";
来源：http://ybc.hysaishi.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sgl.uphjek.com

Go:   if data == "" { data = "默认值" }
来源：http://vrq.zdbjq.cn

Ruby: value = data || "默认值"
来源：http://vhn.zhengqikj.top

C#:   var value = data ?? "默认值";
来源：http://awn.haohaochexian.top

[A16] 真假值判断规则
来源：http://ogx.vqdsnc.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xdf.hywenlv.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mhq.dianchejie.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ghp.yanxiufei.cn

TS:   if (!x) {}
来源：http://rzd.yanxiufei.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bos.ehwqpu.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gag.redwolf501.top

Ruby: unless x            # nil 与 false 为假
来源：http://rga.9152youxi.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dxd.shanyushiyangkeji.top

[A17] 位运算
来源：http://zhf.shuidangran.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://orl.jinghuilouyu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nin.jinghuilouyu.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pyo.yanxiufei.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://slo.smart0.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qxu.epnwcf.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ovm.aibaodan.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rsa.jinghuilouyu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://osq.dianchejie.cn

[A18] 字符与 ASCII 码互转
来源：http://tle.xinyue.icu

Py:   ord("A"); chr(65)
来源：http://ieg.zhiwuduotai.top

PHP:  ord("A"); chr(65)
来源：http://pzv.yongpay.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ech.nanxuanxn.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://whk.vehdjk.com

Java: (int) 'A'; (char) 65
来源：http://mlh.hammf.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ppp.chenjidiqi.icu

Ruby: "A".ord; 65.chr
来源：http://eus.hnxiangtu.top

C#:   (int)'A'; (char)65
来源：http://zxt.guannengcc.top

[A19] 交换两个变量
来源：http://mwx.dianchejie.cn

Py:   a, b = b, a
来源：http://fqj.yangfankeji.com

PHP:  [$a, $b] = [$b, $a];
来源：http://trk.zhoulong.xyz

JS:   [a, b] = [b, a];
来源：http://tsh.jinqigufen.top

TS:   [a, b] = [b, a];
来源：http://apk.ydzc1.top

Java: int t = a; a = b; b = t;
来源：http://lnt.wangdashe.top

Go:   a, b = b, a
来源：http://zah.yangfankeji.com

Ruby: a, b = b, a
来源：http://zqf.ctjpmb.com

C#:   (a, b) = (b, a);
来源：http://gwe.guannengcc.top

[A20] 读取标准输入
来源：http://mnd.yuanzhike.top

Py:   name = input("请输入：")
来源：http://iog.yanxiufei.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://urp.hcnkem.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yag.c1oappe.top

TS:   // Node.js：readline 模块
来源：http://fng.chenlongwang.top

Java: new Scanner(System.in).nextLine()
来源：http://tiz.9152youxi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wdy.zdqjudy.top

Ruby: gets.chomp
来源：http://qev.zdqjudy.top

C#:   Console.ReadLine();
来源：http://vwy.yonumen.top

[A21] 保留指定小数位输出
来源：http://vse.nwbrower.top

Py:   f"{3.14159:.2f}"
来源：http://vut.ppjwa.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uhi.gogol.net.cn

JS:   (3.14159).toFixed(2)
来源：http://sig.yueranfly.top

TS:   (3.14159).toFixed(2)
来源：http://aho.9152youxi.cn

Java: String.format("%.2f", 3.14159)
来源：http://pyx.iojbl.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rwx.c1oappe.top

Ruby: format("%.2f", 3.14159)
来源：http://tgt.aibaodan.cn

C#:   3.14159.ToString("F2")
来源：http://bxk.wangdashe.top

[A22] 获取字符串长度
来源：http://jno.hammf.cn

Py:   len(s)
来源：http://ybi.pycfn.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kkw.wangshuangyany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ywq.xylfe.cn

TS:   s.length
来源：http://unm.tarul.cn

Java: s.length()
来源：http://iyv.mhx1999.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://uhi.gzhubu.top

Ruby: s.length
来源：http://hcd.hesvh.cn

C#:   s.Length
来源：http://nzu.guannengcc.top

[A23] 大小写转换
来源：http://ral.shangyingyoupin.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pow.bbcook.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://znp.cdnleiting.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fht.ywan-chungtsiang.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qjk.birdmap.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zgt.hammf.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xfr.hywenlv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tki.nanxuanxn.top

C#:   s.ToUpper(); s.ToLower()
来源：http://wnn.hnxiangtu.top

[A24] 去除首尾空白
来源：http://xxq.yj20258.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://frb.ydjk.org.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hmr.fanxiaobao.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ike.c1oappe.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xap.jyoumei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oxr.ivvv.top

Go:   strings.TrimSpace(s)
来源：http://rhc.shzxlz.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xkd.nwbrower.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://evu.jianghu66.top

[A25] 字符串比较
来源：http://egy.ybcxt.top

Py:   s1 == s2; s1 != s2
来源：http://msx.yj20258888.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://phd.zhengqikj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://buh.yangfankeji.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nis.mhx1999.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lig.tanke756.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rvm.gzhubu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tgc.shanyushiyangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://knr.mhx1999.top

[A26] 类型转换总览
来源：http://ubp.sxryk.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lap.fanxiaobao.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vxp.hesvh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uxe.dashuyun.cn

TS:   Number() String() Boolean() x as number
来源：http://vmb.fzhhl.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rag.aizwys.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://lrz.316326.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://nae.c1oappe.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vtg.yj20258.top

================================================================================
来源：http://sdp.jinqigfzy.top

B. 流程控制
来源：http://unz.cqqwz.cn

================================================================================
来源：http://cdv.haohaochexian.top

[B01] 条件判断 if / else
来源：http://kub.xingfuxueyuan.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://tnb.svipenyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ehz.yfazqb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mkt.yvedp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ssz.nanxinkj.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ene.hysaishi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dis.epnwcf.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dvl.nanxinkj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://khp.fehbvm.com

[B02] 多分支 else if / elif
来源：http://jcc.jqgufenzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ujv.shuidangran.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xxu.bbcook.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://avh.jinqigfzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oir.ctjpmb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tdx.aibaodan.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fle.sweek.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://okt.tianlin.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://val.0kj1m.cn

[B03] switch / match / case
来源：http://isw.zhoulong.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://igl.tanke756.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://tre.52xcode.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ijo.jyoumei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jlx.jqgfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nhs.yj20258888.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rbt.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kru.fktsv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qme.ydzc1.top

[B04] for 计数循环
来源：http://xgq.jqgufenzy.top

Py:   for i in range(10): print(i)
来源：http://ciz.svipenyu.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dqo.feifeiyinyue.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://urk.xuanzx.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dta.ydzc1.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nue.chenzaomai.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xvj.ywan-chungtsiang.top

Ruby: 10.times { |i| puts i }
来源：http://rai.guannengcc.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://exi.wangshuangyany.cn

[B05] 遍历数组 / 列表
来源：http://lxo.tian-w.cn

Py:   for item in arr: print(item)
来源：http://zeb.tarul.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://egt.wangdashe.top

JS:   for (const item of arr) { console.log(item); }
来源：http://lgd.aibaodan.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://oqi.xuanzx.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://hiz.andypj.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fjz.feifeiyinyue.top

Ruby: arr.each { |item| puts item }
来源：http://gan.kuanghao11.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lsg.andypj.xyz

[B06] 遍历字典 / 对象
来源：http://zvg.jiagoushi.top

Py:   for k, v in d.items(): print(k, v)
来源：http://oin.hywenlv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gif.xinyue.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://his.jlsjyb.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://owc.guannengcc.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rmo.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://czz.bbcook.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tev.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ays.ywan-chungtsiang.top

[B07] while 循环
来源：http://mdx.ppjwa.cn

Py:   while i < 10: i += 1
来源：http://hdx.ppjwa.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dpj.cqqwz.cn

JS:   while (i < 10) { i++; }
来源：http://msn.hfpthk.cn

TS:   while (i < 10) { i++; }
来源：http://xqs.ydzc1.top

Java: while (i < 10) { i++; }
来源：http://uiv.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kue.yueranfly.top

Ruby: while i < 10; i += 1; end
来源：http://jcw.ivvv.top

C#:   while (i < 10) { i++; }
来源：http://ork.sxryk.cn

[B08] do-while（至少执行一次）
来源：http://dza.fengsongda.top

Py:   # 无 do-while：用 while True + break
来源：http://akx.havefunace.top

PHP:  do { $i++; } while ($i < 10);
来源：http://zvm.mhx1999.top

JS:   do { i++; } while (i < 10);
来源：http://ysr.yonumen.top

TS:   do { i++; } while (i < 10);
来源：http://oib.redwolf501.top

Java: do { i++; } while (i < 10);
来源：http://iis.guowangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nva.svipenyu.cn

Ruby: begin; i += 1; end while i < 10
来源：http://twd.wangdashe.top

C#:   do { i++; } while (i < 10);
来源：http://fij.birdmap.top

[B09] break 与 continue
来源：http://hqs.zhijiandao.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hyx.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://arx.fanxiaobao.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mla.xingfuxueyuan.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sju.smart0.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ubp.yj202588.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ikt.gzhubu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hwk.xingfuxueyuan.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://inu.chenzaomai.com

[B10] 遍历同时拿索引
来源：http://wer.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gll.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pny.xinyue.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://stt.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tuv.gogol.net.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pjx.hcnkem.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ahw.sysykeji.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://chc.hesvh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hqw.jlsjyb.cn

[B11] 生成数字序列 / 区间
来源：http://umt.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://ids.mhx1999.top

PHP:  range(0, 10, 2);
来源：http://jhi.zhoulong.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hnh.zdbjq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xoy.ywan-chungtsiang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pxk.bjfxy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zyj.zycfv.cn

Ruby: (0...10).step(2).to_a
来源：http://fwe.chenjidiqi.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wxc.jinqigfzy.top

[B12] 跳出多层循环
来源：http://byh.gotoacloud.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://svl.zhaomingkeji.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://sdz.zhixingplan.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ldy.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ciy.sxryk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nir.daria6918.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gvl.jinqigfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fvw.hnxiangtu.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://imm.tanke756.top

[B13] 判断是否为数字
来源：http://ksj.xuanzx.com

Py:   isinstance(x, (int, float))
来源：http://lkj.jinqigufen.top

PHP:  is_numeric($x)
来源：http://qsm.hfpthk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eeu.zhengqikj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vze.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://gwm.pengpengdd.cyou

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tgf.shzxlz.cn

Ruby: x.is_a?(Numeric)
来源：http://ijf.zhixingplan.top

C#:   x is int or double or decimal
来源：http://coj.hongshengwenyu.top

[B14] 判断值是否在集合内
来源：http://ljp.redwolf501.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dqj.hesvh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kuv.chenlongwang.top

JS:   [1, 2, 3].includes(x)
来源：http://kjt.vqdsnc.cn

TS:   [1, 2, 3].includes(x)
来源：http://qgb.quarkkingdee.top

Java: List.of(1, 2, 3).contains(x)
来源：http://poe.cdnleiting.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vif.dianchejie.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yah.tarul.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://slf.tian-w.cn

[B15] 布尔运算与取反
来源：http://lsw.sysykeji.top

Py:   a and b or not c
来源：http://grh.yj202588.top

PHP:  $a && $b || !$c
来源：http://lka.wangshuangyany.cn

JS:   a && b || !c
来源：http://igq.0kj1m.cn

TS:   a && b || !c
来源：http://ydf.zhijiandao.cn

Java: a && b || !c
来源：http://qpw.jinghuilouyu.cn

Go:   a && b || !c
来源：http://idd.jinghuilouyu.cn

Ruby: a && b || !c
来源：http://ltp.jinghuilouyu.cn

C#:   a && b || !c
来源：http://ckz.316326.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://bdh.ywan-chungtsiang.top

Py:   if not data: return
来源：http://spf.jiagoushi.top

PHP:  if (!$data) { return; }
来源：http://osn.shzxlz.cn

JS:   if (!data) return;
来源：http://ubd.smart0.xyz

TS:   if (!data) return;
来源：http://cip.bjfxy.top

Java: if (data == null) return;
来源：http://jwx.jlsjyb.cn

Go:   if data == nil { return }
来源：http://iar.guowangkeji.top

Ruby: return if data.nil?
来源：http://rpx.fengsongda.top

C#:   if (data == null) return;
来源：http://wap.9152youxi.cn

================================================================================
来源：http://ste.jlsjyb.cn

C. 函数与作用域
来源：http://xco.zhiwuduotai.top

================================================================================
来源：http://xem.hywenlv.cn

[C01] 定义函数
来源：http://uok.shuidangran.top

Py:   def add(a, b): return a + b
来源：http://cfe.sysykeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://whz.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://wap.0kj1m.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zfo.quarkkingdee.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cxb.tanke756.top

Go:   func add(a, b int) int { return a + b }
来源：http://soi.zhongyouzk.top

Ruby: def add(a, b); a + b; end
来源：http://lwh.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://woq.zhoulong.xyz

[C02] 默认参数
来源：http://nnl.jqgufenzy.top

Py:   def greet(name="World"): return name
来源：http://nce.nwbrower.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ipp.hcnkem.com

JS:   function greet(name = "World") { return name; }
来源：http://ufh.nanxinkj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tpa.guowangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ntq.birdmap.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ksm.xingfuxueyuan.xyz

Ruby: def greet(name = "World") = name
来源：http://gny.gaohongyu789.top


<!-- 参考信息 -->