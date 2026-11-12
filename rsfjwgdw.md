代发 wailian999

Java: "第一行\n第二行"
来源：http://tfb.dianchejie.cn

Go:   "第一行\n第二行"
来源：http://uwo.xylfe.cn

Ruby: "第一行\n第二行"
来源：http://enx.quarkkingdee.top

C#:   "第一行\n第二行"
来源：http://etd.nanxuanxn.top

[A14] 注释写法
来源：http://fvb.jinqigfzy.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://uhj.jlsjyb.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://rwp.sufxvd.cn

JS:   // 单行；/* 多行 */
来源：http://xla.aizwys.cn

TS:   // 单行；/* 多行 */
来源：http://sil.tianlin.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://pyp.cucudq.cn

Go:   // 单行；/* 多行 */
来源：http://byu.andypj.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://tnp.52xcode.cn

C#:   // 单行；/* 多行 */
来源：http://pjy.xylfe.cn

[A15] 空值判断与默认值
来源：http://yhv.xuanzx.com

Py:   value = data or "默认值"
来源：http://ycz.yuanzhike.top

PHP:  $value = $data ?? "默认值";
来源：http://vhw.hnqzz.top

JS:   const value = data ?? "默认值";
来源：http://wmo.jinyuanbaomall.cn

TS:   const value = data ?? "默认值";
来源：http://mdd.zdqjudy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xwy.chenjidiqi.icu

Go:   if data == "" { data = "默认值" }
来源：http://xcw.ppjwa.cn

Ruby: value = data || "默认值"
来源：http://txf.fktsv.cn

C#:   var value = data ?? "默认值";
来源：http://ygx.yonumen.top

[A16] 真假值判断规则
来源：http://aid.shuidangran.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://bzz.jqgfzy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rdm.zdqjudy.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://upt.tanke756.top

TS:   if (!x) {}
来源：http://rrv.xziqi.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vww.zhoulong.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://inr.cashguo.top

Ruby: unless x            # nil 与 false 为假
来源：http://gix.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fhp.52xcode.cn

[A17] 位运算
来源：http://lkv.hnxiangtu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cve.fengsongda.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://skr.9152youxi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fzi.jyoumei.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ujw.yonumen.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rjf.pengpengdd.cyou

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pho.zhongyouzk.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mut.guannengcc.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://igp.sufxvd.cn

[A18] 字符与 ASCII 码互转
来源：http://dgn.shanyushiyangkeji.top

Py:   ord("A"); chr(65)
来源：http://ssp.jinyuanbaomall.cn

PHP:  ord("A"); chr(65)
来源：http://ccs.bjfxy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://frb.chenjidiqi.icu

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rtj.chenzaomai.com

Java: (int) 'A'; (char) 65
来源：http://sbo.jinqigfzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://luc.feifeiyinyue.top

Ruby: "A".ord; 65.chr
来源：http://gly.ybcxt.top

C#:   (int)'A'; (char)65
来源：http://qtg.andypj.xyz

[A19] 交换两个变量
来源：http://aex.ivvv.top

Py:   a, b = b, a
来源：http://njz.zhaomingkeji.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://dsq.hcnkem.com

JS:   [a, b] = [b, a];
来源：http://fqa.quarkkingdee.top

TS:   [a, b] = [b, a];
来源：http://vhr.9152youxi.cn

Java: int t = a; a = b; b = t;
来源：http://zuq.jyoumei.cn

Go:   a, b = b, a
来源：http://gqd.ydjk.org.cn

Ruby: a, b = b, a
来源：http://ibp.yuxming.cn

C#:   (a, b) = (b, a);
来源：http://cdi.daria6918.cn

[A20] 读取标准输入
来源：http://dcq.ywan-chungtsiang.top

Py:   name = input("请输入：")
来源：http://luy.gaohongyu789.top

PHP:  $name = trim(fgets(STDIN));
来源：http://dmg.yfazqb.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nck.jyoumei.cn

TS:   // Node.js：readline 模块
来源：http://egc.0kj1m.cn

Java: new Scanner(System.in).nextLine()
来源：http://yyo.wangdashe.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gmm.hesvh.cn

Ruby: gets.chomp
来源：http://exe.ppjwa.cn

C#:   Console.ReadLine();
来源：http://vlp.xuetiantiany.cn

[A21] 保留指定小数位输出
来源：http://jpc.meibo888.top

Py:   f"{3.14159:.2f}"
来源：http://acb.xuetiantiany.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ljy.wangdashe.top

JS:   (3.14159).toFixed(2)
来源：http://pik.bjfxy.top

TS:   (3.14159).toFixed(2)
来源：http://bes.pengpengdd.cyou

Java: String.format("%.2f", 3.14159)
来源：http://cvv.sxryk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oxc.zhongyouzk.top

Ruby: format("%.2f", 3.14159)
来源：http://dmg.yongpay.top

C#:   3.14159.ToString("F2")
来源：http://glj.fzhhl.top

[A22] 获取字符串长度
来源：http://rhj.tanke756.top

Py:   len(s)
来源：http://nku.yongpay.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zgy.jqgufenzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://agl.andypj.xyz

TS:   s.length
来源：http://knx.fzhhl.top

Java: s.length()
来源：http://lxi.jqgufenzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rjl.chenjidiqi.icu

Ruby: s.length
来源：http://ner.xingfuxueyuan.xyz

C#:   s.Length
来源：http://asi.nanxuanxn.top

[A23] 大小写转换
来源：http://akh.shangyingyoupin.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ukp.fanxiaobao.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oqk.yanxiufei.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kiw.zhaomingkeji.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bqa.dianchejie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xpa.zdbjq.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rdj.vehdjk.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eln.gogol.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ovj.meibo888.top

[A24] 去除首尾空白
来源：http://czs.yanxiufei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://abs.zhixingplan.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ncn.hnxiangtu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nfy.xingfuxueyuan.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qpx.wangshuangyany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ono.ywan-chungtsiang.top

Go:   strings.TrimSpace(s)
来源：http://dnm.hongshengwenyu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wnv.gotoacloud.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lze.jqgfzy.top

[A25] 字符串比较
来源：http://vlz.shuidangran.top

Py:   s1 == s2; s1 != s2
来源：http://szw.xinyue.icu

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ymk.mhx1999.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://foc.tianlin.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jyy.zhiwuduotai.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ycl.gogol.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wup.zhengqikj.top

Ruby: s1 == s2; s1 <=> s2
来源：http://gad.guowangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://syn.yfazqb.com

[A26] 类型转换总览
来源：http://egi.fzhhl.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ftf.chenzaomai.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vqa.yfazqb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gxm.fktsv.cn

TS:   Number() String() Boolean() x as number
来源：http://jym.andypj.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bjn.ydzc1.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wjb.dashuyun.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://voe.0kj1m.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://bho.hywenlv.cn

================================================================================
来源：http://epr.havefunace.top

B. 流程控制
来源：http://qbi.uphjek.com

================================================================================
来源：http://yhn.fzhhl.top

[B01] 条件判断 if / else
来源：http://ois.jinqigfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mqi.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tds.andypj.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cfh.hnxiangtu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://alt.zhaomingkeji.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://dmc.jinyuanbaomall.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oov.vqdsnc.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jni.sxryk.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zrm.kuanghao11.cn

[B02] 多分支 else if / elif
来源：http://vya.yongpay.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rxx.sweek.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cje.sysykeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rae.xuanzx.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fqs.feifeiyinyue.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gjf.shanyushiyangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wft.ivvv.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mqx.snrcjt.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yoh.jyoumei.cn

[B03] switch / match / case
来源：http://crv.xuanzx.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://zpg.kuanghao11.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mjf.yuxming.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://snq.jianghu66.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nbb.yueranfly.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ics.sxryk.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cqa.gzhubu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jiz.c1oappe.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ztr.sjlbkw.cn

[B04] for 计数循环
来源：http://soy.zhoulong.xyz

Py:   for i in range(10): print(i)
来源：http://pex.birdmap.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://iiv.hammf.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://itf.guowangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sfm.bbcook.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://isc.xylfe.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lqt.quarkkingdee.top

Ruby: 10.times { |i| puts i }
来源：http://iqt.redwolf501.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fzp.dashuyun.cn

[B05] 遍历数组 / 列表
来源：http://ara.jinqigufen.top

Py:   for item in arr: print(item)
来源：http://ulq.aibaodan.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mwm.meibo888.top

JS:   for (const item of arr) { console.log(item); }
来源：http://mxc.c1oappe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cce.havefunace.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://czm.zhengqikj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ezf.fanxiaobao.xyz

Ruby: arr.each { |item| puts item }
来源：http://yor.zdqjudy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ybf.vqdsnc.cn

[B06] 遍历字典 / 对象
来源：http://lpo.yuxming.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://twj.fzhhl.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sst.316326.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sen.shzxlz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://stz.zhongyouzk.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rui.shzxlz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://iam.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zma.wangdashe.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rhl.ywan-chungtsiang.top

[B07] while 循环
来源：http://uxq.tianlin.xyz

Py:   while i < 10: i += 1
来源：http://svn.xinyue.icu

PHP:  while ($i < 10) { $i++; }
来源：http://vyf.redwolf501.top

JS:   while (i < 10) { i++; }
来源：http://rxb.feifeiyinyue.top

TS:   while (i < 10) { i++; }
来源：http://gyc.vqdsnc.cn

Java: while (i < 10) { i++; }
来源：http://zto.zdbjq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yyv.smart0.xyz

Ruby: while i < 10; i += 1; end
来源：http://udw.jinqigufen.top

C#:   while (i < 10) { i++; }
来源：http://mii.nanxuanxn.top

[B08] do-while（至少执行一次）
来源：http://kbg.nanxinkj.top

Py:   # 无 do-while：用 while True + break
来源：http://jvk.jyoumei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zhu.cheryme.top

JS:   do { i++; } while (i < 10);
来源：http://iss.iojbl.cn

TS:   do { i++; } while (i < 10);
来源：http://tfq.yuxming.cn

Java: do { i++; } while (i < 10);
来源：http://ffc.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://ajf.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tmx.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://knv.smart0.xyz

[B09] break 与 continue
来源：http://fmh.ehwqpu.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yky.jinghuilouyu.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hrp.zdqjudy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://khg.chenlongwang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mln.shzxlz.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zpq.jianghu66.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yvh.tianlin.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uqd.yfazqb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://czr.jiagoushi.top

[B10] 遍历同时拿索引
来源：http://jri.ehwqpu.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jgs.wangshuangyany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://etb.hywenlv.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yba.jyoumei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fri.zhoulong.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://crw.dianchejie.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://xrn.sxryk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://guy.shanyushiyangtech.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lyy.yj202588.top

[B11] 生成数字序列 / 区间
来源：http://hol.mhx1999.top

Py:   list(range(0, 10, 2))
来源：http://fhi.cdnleiting.top

PHP:  range(0, 10, 2);
来源：http://rfq.hongshengwenyu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ubz.shzxlz.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hen.zhiwuduotai.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://krr.zhengqikj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ohx.andypj.xyz

Ruby: (0...10).step(2).to_a
来源：http://xtr.gotoacloud.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gzp.sjlbkw.cn

[B12] 跳出多层循环
来源：http://sez.xinyue.icu

Py:   # 无标签跳转：抽成函数用 return
来源：http://niq.zdbjq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tex.feifeiyinyue.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://nvh.xuanzx.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://uri.hammf.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://acp.jlsjyb.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tgv.mhx1999.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mdt.zycfv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://den.yanxiufei.cn

[B13] 判断是否为数字
来源：http://rge.hongshengwenyu.top

Py:   isinstance(x, (int, float))
来源：http://lny.hnxiangtu.top

PHP:  is_numeric($x)
来源：http://xji.snrcjt.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ikj.nanxuanxn.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hdy.gzhubu.top

Java: x instanceof Number
来源：http://hfl.fktsv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gys.aibaodan.cn

Ruby: x.is_a?(Numeric)
来源：http://hog.zdbjq.cn

C#:   x is int or double or decimal
来源：http://gbw.fzhhl.top

[B14] 判断值是否在集合内
来源：http://vay.andypj.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qzj.ydzc1.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dkt.zhiwuduotai.top

JS:   [1, 2, 3].includes(x)
来源：http://wxq.kuanghao11.cn

TS:   [1, 2, 3].includes(x)
来源：http://btv.hysaishi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jge.fehbvm.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vul.jqgfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://gbw.cashguo.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://lme.quarkkingdee.top

[B15] 布尔运算与取反
来源：http://ygz.aibaodan.cn

Py:   a and b or not c
来源：http://akb.yj20258888.top

PHP:  $a && $b || !$c
来源：http://eue.aibaodan.cn

JS:   a && b || !c
来源：http://ivo.yonumen.top

TS:   a && b || !c
来源：http://fyt.shanyushiyangkeji.top

Java: a && b || !c
来源：http://rzm.sysykeji.top

Go:   a && b || !c
来源：http://mwd.shanyushiyangkeji.top

Ruby: a && b || !c
来源：http://rpc.yuanzhike.top

C#:   a && b || !c
来源：http://xza.ehwqpu.com

[B16] 卫语句：不满足条件提前返回
来源：http://zxx.xuetiantiany.cn

Py:   if not data: return
来源：http://wer.ehwqpu.com

PHP:  if (!$data) { return; }
来源：http://tve.ydzc1.top

JS:   if (!data) return;
来源：http://oer.nwbrower.top

TS:   if (!data) return;
来源：http://bed.jinqigufen.top

Java: if (data == null) return;
来源：http://kkw.yueranfly.top

Go:   if data == nil { return }
来源：http://xzq.hammf.cn

Ruby: return if data.nil?
来源：http://pnh.cqqwz.cn

C#:   if (data == null) return;
来源：http://moh.jqgfzy.top

================================================================================
来源：http://yne.wangshuangyany.cn

C. 函数与作用域
来源：http://ukm.fanxiaobao.xyz

================================================================================
来源：http://ekx.bbcook.cn

[C01] 定义函数
来源：http://kxd.316326.xyz

Py:   def add(a, b): return a + b
来源：http://syc.dianchejie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yvq.hnxiangtu.top

JS:   function add(a, b) { return a + b; }
来源：http://ljb.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zpl.hysaishi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ydy.jinqigfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://cpc.zhiwuduotai.top

Ruby: def add(a, b); a + b; end
来源：http://czt.iojbl.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kll.zhoulong.xyz

[C02] 默认参数
来源：http://snx.bjfxy.top

Py:   def greet(name="World"): return name
来源：http://ykm.yuanzhike.top

PHP:  function greet($name = "World") { return $name; }
来源：http://oct.cqqwz.cn

JS:   function greet(name = "World") { return name; }
来源：http://qxa.shzxlz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jij.zhiwuduotai.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ugd.xingfuxueyuan.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hbb.ctjpmb.com

Ruby: def greet(name = "World") = name
来源：http://ufh.shangyingyoupin.top

C#:   string Greet(string name = "World") => name;
来源：http://czh.hammf.cn

[C03] 可变参数
来源：http://inn.ydzc1.top

Py:   def total(*args): return sum(args)
来源：http://kap.hywenlv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://yln.xylfe.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://alv.fehbvm.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mdi.zhaomingkeji.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pap.yj202588.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yti.316326.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://sex.tian-w.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qcz.ybcxt.top

[C04] 命名参数 / 关键字参数
来源：http://tqx.chenlongwang.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nqt.zhoulong.xyz


<!-- 参考信息 -->