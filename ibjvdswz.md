代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://fbk.dianchejie.cn

TS:   x > 0 ? "yes" : "no"
来源：http://qal.0kj1m.cn

Java: x > 0 ? "yes" : "no"
来源：http://unv.hongshengwenyu.top

Go:   // 无三元运算符，需用 if 语句
来源：http://jie.jyoumei.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://jnh.hammf.cn

C#:   x > 0 ? "yes" : "no"
来源：http://xwo.cashguo.top

[A12] 字符串插值 / 格式化
来源：http://zuw.aibaodan.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ozq.zdqjudy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hps.chenlongwang.top

JS:   `Hello, ${name}!`
来源：http://wmn.zhongyouzk.top

TS:   `Hello, ${name}!`
来源：http://dcx.shangyingyoupin.top

Java: "Hello, %s!".formatted(name)
来源：http://pgn.cdnleiting.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://xfo.c1oappe.top

Ruby: "Hello, #{name}!"
来源：http://iyn.bbcook.cn

C#:   $"Hello, {name}!"
来源：http://ntw.zhixingplan.top

[A13] 多行字符串（练习 \n 转义）
来源：http://xua.yuanzhike.top

Py:   "第一行\n第二行"
来源：http://nyd.jinyuanbaomall.cn

PHP:  "第一行\n第二行"
来源：http://wul.cheryme.top

JS:   "第一行\n第二行"
来源：http://ika.shangyingyoupin.top

TS:   "第一行\n第二行"
来源：http://urn.ydjk.org.cn

Java: "第一行\n第二行"
来源：http://tin.9152youxi.cn

Go:   "第一行\n第二行"
来源：http://xgh.xinyue.icu

Ruby: "第一行\n第二行"
来源：http://okz.fehbvm.com

C#:   "第一行\n第二行"
来源：http://jcu.yfazqb.com

[A14] 注释写法
来源：http://gjy.ywan-chungtsiang.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://vwg.fanxiaobao.xyz

PHP:  // 或 # 单行；/* 多行 */
来源：http://zmy.fehbvm.com

JS:   // 单行；/* 多行 */
来源：http://rqs.xylfe.cn

TS:   // 单行；/* 多行 */
来源：http://rub.jinyuanbaomall.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://fpx.hesvh.cn

Go:   // 单行；/* 多行 */
来源：http://fxw.tanke756.top

Ruby: # 单行；=begin 多行 =end
来源：http://tuv.hammf.cn

C#:   // 单行；/* 多行 */
来源：http://eby.zdqjudy.top

[A15] 空值判断与默认值
来源：http://klj.redwolf501.top

Py:   value = data or "默认值"
来源：http://fsl.daria6918.cn

PHP:  $value = $data ?? "默认值";
来源：http://wkz.yj202588.top

JS:   const value = data ?? "默认值";
来源：http://ltj.zhaomingkeji.xyz

TS:   const value = data ?? "默认值";
来源：http://qir.gaohongyu789.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pmq.snrcjt.cn

Go:   if data == "" { data = "默认值" }
来源：http://fxj.fehbvm.com

Ruby: value = data || "默认值"
来源：http://ftt.xingfuxueyuan.xyz

C#:   var value = data ?? "默认值";
来源：http://exm.guowangkeji.top

[A16] 真假值判断规则
来源：http://hbb.0kj1m.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://csj.xingfuxueyuan.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cut.fanxiaobao.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://gmj.shanyushiyangkeji.top

TS:   if (!x) {}
来源：http://voq.guowangkeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uvm.fktsv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://qhq.quarkkingdee.top

Ruby: unless x            # nil 与 false 为假
来源：http://aej.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://brl.hongshengwenyu.top

[A17] 位运算
来源：http://sys.wangshuangyany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hhb.gaohongyu789.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nsr.fengsongda.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bux.daxiang520.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wfm.zhijiandao.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ipo.jinqigufen.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mdc.epnwcf.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cwg.haohaochexian.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rnj.shzxlz.cn

[A18] 字符与 ASCII 码互转
来源：http://oxj.yanxiufei.cn

Py:   ord("A"); chr(65)
来源：http://mwr.jinqigfzy.top

PHP:  ord("A"); chr(65)
来源：http://yrr.yonumen.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://biu.shzxlz.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nkz.xuetiantiany.cn

Java: (int) 'A'; (char) 65
来源：http://fqx.redwolf501.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hso.ctjpmb.com

Ruby: "A".ord; 65.chr
来源：http://fjr.jinyuanbaomall.cn

C#:   (int)'A'; (char)65
来源：http://pjz.gaohongyu789.top

[A19] 交换两个变量
来源：http://ayk.fanxiaobao.xyz

Py:   a, b = b, a
来源：http://ixs.aibaodan.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://izk.fengsongda.top

JS:   [a, b] = [b, a];
来源：http://ehg.yongpay.top

TS:   [a, b] = [b, a];
来源：http://hel.shanyushiyangtech.top

Java: int t = a; a = b; b = t;
来源：http://leg.hnqzz.top

Go:   a, b = b, a
来源：http://quq.yuanzhike.top

Ruby: a, b = b, a
来源：http://doz.316326.xyz

C#:   (a, b) = (b, a);
来源：http://nrm.hongshengwenyu.top

[A20] 读取标准输入
来源：http://lvr.aibaodan.cn

Py:   name = input("请输入：")
来源：http://qlq.nwbrower.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qof.chenjidiqi.icu

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nen.nwbrower.top

TS:   // Node.js：readline 模块
来源：http://qtl.kuanghao11.cn

Java: new Scanner(System.in).nextLine()
来源：http://ugs.chenjidiqi.icu

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wra.daxiang520.top

Ruby: gets.chomp
来源：http://tym.hnxiangtu.top

C#:   Console.ReadLine();
来源：http://vjr.redwolf501.top

[A21] 保留指定小数位输出
来源：http://tuj.hnqzz.top

Py:   f"{3.14159:.2f}"
来源：http://ppx.zhoulong.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://aip.wangdashe.top

JS:   (3.14159).toFixed(2)
来源：http://iws.xuetiantiany.cn

TS:   (3.14159).toFixed(2)
来源：http://sjm.jyoumei.cn

Java: String.format("%.2f", 3.14159)
来源：http://ysy.yueranfly.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ipr.bbcook.cn

Ruby: format("%.2f", 3.14159)
来源：http://qln.ywan-chungtsiang.top

C#:   3.14159.ToString("F2")
来源：http://rjg.pengpengdd.cyou

[A22] 获取字符串长度
来源：http://jac.jinqigfzy.top

Py:   len(s)
来源：http://rkb.yonumen.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://esb.zhiwuduotai.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ptl.iojbl.cn

TS:   s.length
来源：http://dkd.gogol.net.cn

Java: s.length()
来源：http://ggf.zhaomingkeji.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://axh.smart0.xyz

Ruby: s.length
来源：http://vzt.hammf.cn

C#:   s.Length
来源：http://ipu.feifeiyinyue.top

[A23] 大小写转换
来源：http://kew.nwbrower.top

Py:   s.upper(); s.lower(); s.title()
来源：http://kat.nanxuanxn.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kaz.gaohongyu789.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hgx.xylfe.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://whg.0kj1m.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gwj.xylfe.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://utd.gogol.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sug.bjfxy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rbe.cheryme.top

[A24] 去除首尾空白
来源：http://ibn.yuxming.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://pej.mhx1999.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fsm.wangdashe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lsj.fktsv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yix.yanxiufei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://idg.jqgufenzy.top

Go:   strings.TrimSpace(s)
来源：http://oin.zhijiandao.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zvc.cucudq.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://inu.xuanzx.com

[A25] 字符串比较
来源：http://mme.dianchejie.cn

Py:   s1 == s2; s1 != s2
来源：http://wjs.iojbl.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hwl.quarkkingdee.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jrl.xylfe.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gci.cqqwz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sty.cqqwz.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pvb.hywenlv.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://jln.gaohongyu789.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xbp.dianchejie.cn

[A26] 类型转换总览
来源：http://osg.gaohongyu789.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pkq.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://muo.ehwqpu.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ufx.jinqigufen.top

TS:   Number() String() Boolean() x as number
来源：http://mqd.pycfn.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wlc.tarul.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://waw.sxryk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ihk.yanxiufei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gyb.fengsongda.top

================================================================================
来源：http://pnh.meibo888.top

B. 流程控制
来源：http://peb.hfpthk.cn

================================================================================
来源：http://tph.shanyushiyangtech.top

[B01] 条件判断 if / else
来源：http://jxb.yangfankeji.com

Py:   result = "正" if x > 0 else "非正"
来源：http://ljf.ydjk.org.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://apm.yangfankeji.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ruv.vqdsnc.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nhx.kuanghao11.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://vtv.vqdsnc.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gzf.bbcook.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://for.hnxiangtu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://aft.xylfe.cn

[B02] 多分支 else if / elif
来源：http://buu.ehwqpu.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dbn.andypj.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kpc.shzxlz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://agl.9152youxi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mln.jinqigufen.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://knr.yvedp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://sui.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fxe.cashguo.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://atw.tianlin.xyz

[B03] switch / match / case
来源：http://vne.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hdn.yuanzhike.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://alg.havefunace.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vyi.sysykeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rip.redwolf501.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oqe.guannengcc.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nxl.pengpengdd.cyou

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oqr.guannengcc.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xjj.fzhhl.top

[B04] for 计数循环
来源：http://jym.jianghu66.top

Py:   for i in range(10): print(i)
来源：http://rmq.yongpay.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vgo.shzxlz.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://abc.xuanzx.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cvr.hesvh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yts.fengsongda.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xri.uphjek.com

Ruby: 10.times { |i| puts i }
来源：http://cgp.tarul.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vrg.hysaishi.cn

[B05] 遍历数组 / 列表
来源：http://pdy.jinghuilouyu.cn

Py:   for item in arr: print(item)
来源：http://xci.ywan-chungtsiang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://brr.chenjidiqi.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://trm.uphjek.com

TS:   for (const item of arr) { console.log(item); }
来源：http://opq.nanxinkj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jfg.andypj.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lan.jinghuilouyu.cn

Ruby: arr.each { |item| puts item }
来源：http://gdh.vqdsnc.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fxl.feifeiyinyue.top

[B06] 遍历字典 / 对象
来源：http://tvm.ydzc1.top

Py:   for k, v in d.items(): print(k, v)
来源：http://vpg.yuanzhike.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://osg.xingfuxueyuan.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ndu.xziqi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mir.sweek.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://gbn.birdmap.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://svx.haohaochexian.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ojr.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ghz.redwolf501.top

[B07] while 循环
来源：http://lez.yongpay.top

Py:   while i < 10: i += 1
来源：http://hat.9152youxi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://wfs.hfpthk.cn

JS:   while (i < 10) { i++; }
来源：http://zma.yj20258888.top

TS:   while (i < 10) { i++; }
来源：http://zfj.xingfuxueyuan.xyz

Java: while (i < 10) { i++; }
来源：http://odz.jyoumei.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://guz.andypj.xyz

Ruby: while i < 10; i += 1; end
来源：http://sae.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://gey.xinyue.icu

[B08] do-while（至少执行一次）
来源：http://sup.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://eir.52xcode.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sbc.jqgfzy.top

JS:   do { i++; } while (i < 10);
来源：http://cip.uphjek.com

TS:   do { i++; } while (i < 10);
来源：http://xrr.tarul.cn

Java: do { i++; } while (i < 10);
来源：http://rcp.fehbvm.com

Go:   for { i++; if i >= 10 { break } }
来源：http://gii.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://ajs.mhx1999.top

C#:   do { i++; } while (i < 10);
来源：http://oag.cashguo.top

[B09] break 与 continue
来源：http://kze.tian-w.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ylk.52xcode.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rie.haohaochexian.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xmu.hnqzz.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aby.tarul.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jhn.yj20258888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xux.smart0.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jyq.xinyue.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wvi.tarul.cn

[B10] 遍历同时拿索引
来源：http://arg.jianghu66.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vum.tarul.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sfr.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gfw.zdbjq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kgz.hammf.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://omf.bbcook.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://lqr.fehbvm.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eqj.tianlin.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://epo.bjfxy.top

[B11] 生成数字序列 / 区间
来源：http://mxo.zhiwuduotai.top

Py:   list(range(0, 10, 2))
来源：http://vdd.hfpthk.cn

PHP:  range(0, 10, 2);
来源：http://heg.havefunace.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bai.zdbjq.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mce.jqgfzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qno.yuanzhike.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://efq.0kj1m.cn

Ruby: (0...10).step(2).to_a
来源：http://krk.xziqi.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://czc.xziqi.cn

[B12] 跳出多层循环
来源：http://vll.zhixingplan.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ioc.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://gbw.daria6918.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oqe.guannengcc.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rfy.zhaomingkeji.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zrb.cheryme.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tyv.jianghu66.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hta.ydzc1.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ora.fehbvm.com

[B13] 判断是否为数字
来源：http://rfg.jinqigfzy.top

Py:   isinstance(x, (int, float))
来源：http://ngg.yanxiufei.cn

PHP:  is_numeric($x)
来源：http://rdx.pycfn.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://scy.52xcode.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jxf.xuanzx.com

Java: x instanceof Number
来源：http://vib.aizwys.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dwm.dianchejie.cn

Ruby: x.is_a?(Numeric)
来源：http://sjl.haohaochexian.top

C#:   x is int or double or decimal
来源：http://mww.jqgfzy.top

[B14] 判断值是否在集合内
来源：http://thn.havefunace.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vto.redwolf501.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jtj.sxryk.cn

JS:   [1, 2, 3].includes(x)
来源：http://ljw.yuanzhike.top

TS:   [1, 2, 3].includes(x)
来源：http://pdw.zhiwuduotai.top

Java: List.of(1, 2, 3).contains(x)
来源：http://jrq.tianlin.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wpd.snrcjt.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ejd.gotoacloud.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fpj.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://mlj.zhiwuduotai.top

Py:   a and b or not c
来源：http://mfr.yvedp.cn

PHP:  $a && $b || !$c
来源：http://trs.yongpay.top

JS:   a && b || !c
来源：http://zba.hcnkem.com

TS:   a && b || !c
来源：http://vdq.xuanzx.com

Java: a && b || !c
来源：http://blo.316326.xyz

Go:   a && b || !c
来源：http://bdz.quarkkingdee.top

Ruby: a && b || !c
来源：http://kgt.zhoulong.xyz

C#:   a && b || !c
来源：http://tgm.redwolf501.top

[B16] 卫语句：不满足条件提前返回
来源：http://oqg.guowangkeji.top

Py:   if not data: return
来源：http://swy.hesvh.cn

PHP:  if (!$data) { return; }
来源：http://fww.nanxinkj.top

JS:   if (!data) return;
来源：http://eft.ydzc1.top

TS:   if (!data) return;
来源：http://ipi.mhx1999.top

Java: if (data == null) return;
来源：http://tyf.0kj1m.cn

Go:   if data == nil { return }
来源：http://pzb.yueranfly.top

Ruby: return if data.nil?
来源：http://iix.vqdsnc.cn

C#:   if (data == null) return;
来源：http://kim.xinyue.icu

================================================================================
来源：http://xzk.nanxuanxn.top

C. 函数与作用域
来源：http://qdm.gotoacloud.top

================================================================================
来源：http://yzt.yuxming.cn

[C01] 定义函数
来源：http://mji.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://ubh.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://cuf.shangyingyoupin.top

JS:   function add(a, b) { return a + b; }
来源：http://qzn.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dom.jlsjyb.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xpp.andypj.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://exv.mhx1999.top

Ruby: def add(a, b); a + b; end
来源：http://owu.shanyushiyangtech.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rik.zdqjudy.top


<!-- 参考信息 -->