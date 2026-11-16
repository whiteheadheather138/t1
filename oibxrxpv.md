代发 wailian999

Ruby: value = data || "默认值"
来源：http://mna.yj202588.top

C#:   var value = data ?? "默认值";
来源：http://prt.yvedp.cn

[A16] 真假值判断规则
来源：http://cii.hongshengwenyu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ley.bbcook.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bet.hnxiangtu.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fmf.tarul.cn

TS:   if (!x) {}
来源：http://hlp.jqgfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://swc.mhx1999.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kzn.sufxvd.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gif.yj202588.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ipa.fehbvm.com

[A17] 位运算
来源：http://vmq.zhoulong.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wql.zhixingplan.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://iui.epnwcf.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vmk.chenzaomai.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dot.ybcxt.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jte.epnwcf.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vej.daxiang520.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fdn.shuidangran.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zkk.hnqzz.top

[A18] 字符与 ASCII 码互转
来源：http://nis.0kj1m.cn

Py:   ord("A"); chr(65)
来源：http://ynl.zdqjudy.top

PHP:  ord("A"); chr(65)
来源：http://due.hammf.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hvx.guowangkeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cmm.snrcjt.cn

Java: (int) 'A'; (char) 65
来源：http://rgt.gogol.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wcu.yongpay.top

Ruby: "A".ord; 65.chr
来源：http://dyb.gzhubu.top

C#:   (int)'A'; (char)65
来源：http://zyk.daxiang520.top

[A19] 交换两个变量
来源：http://kwh.wangdashe.top

Py:   a, b = b, a
来源：http://lnr.jyoumei.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ffn.jinqigfzy.top

JS:   [a, b] = [b, a];
来源：http://erf.shzxlz.cn

TS:   [a, b] = [b, a];
来源：http://jrc.chenjidiqi.icu

Java: int t = a; a = b; b = t;
来源：http://fzw.pycfn.com

Go:   a, b = b, a
来源：http://qoh.yueranfly.top

Ruby: a, b = b, a
来源：http://iii.ydzc1.top

C#:   (a, b) = (b, a);
来源：http://utd.haohaochexian.top

[A20] 读取标准输入
来源：http://hck.ppjwa.cn

Py:   name = input("请输入：")
来源：http://lkt.zycfv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://grq.yj20258.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://taw.jqgufenzy.top

TS:   // Node.js：readline 模块
来源：http://dqh.yonumen.top

Java: new Scanner(System.in).nextLine()
来源：http://idt.wangdashe.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wsm.hnqzz.top

Ruby: gets.chomp
来源：http://zdq.zhiwuduotai.top

C#:   Console.ReadLine();
来源：http://mwa.daxiang520.top

[A21] 保留指定小数位输出
来源：http://ffz.shzxlz.cn

Py:   f"{3.14159:.2f}"
来源：http://xgz.feifeiyinyue.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nid.zdbjq.cn

JS:   (3.14159).toFixed(2)
来源：http://nfj.ydzc1.top

TS:   (3.14159).toFixed(2)
来源：http://shz.zhengqikj.top

Java: String.format("%.2f", 3.14159)
来源：http://pcu.andypj.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lzg.fanxiaobao.xyz

Ruby: format("%.2f", 3.14159)
来源：http://dwe.zhiwuduotai.top

C#:   3.14159.ToString("F2")
来源：http://pyg.andypj.xyz

[A22] 获取字符串长度
来源：http://fgi.daria6918.cn

Py:   len(s)
来源：http://mob.hysaishi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://evw.shanyushiyangkeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nvs.havefunace.top

TS:   s.length
来源：http://uay.hysaishi.cn

Java: s.length()
来源：http://nql.xuanzx.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qef.shuidangran.top

Ruby: s.length
来源：http://owq.sweek.top

C#:   s.Length
来源：http://aqy.daxiang520.top

[A23] 大小写转换
来源：http://lws.epnwcf.com

Py:   s.upper(); s.lower(); s.title()
来源：http://jti.pycfn.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wlf.ehwqpu.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cmz.nwbrower.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gan.hesvh.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://klw.guowangkeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://fxb.yueranfly.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yys.guannengcc.top

C#:   s.ToUpper(); s.ToLower()
来源：http://gxs.zhixingplan.top

[A24] 去除首尾空白
来源：http://tri.sweek.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iep.fehbvm.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xzg.c1oappe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ywh.fktsv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qlx.chenzaomai.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qze.ivvv.top

Go:   strings.TrimSpace(s)
来源：http://awd.9152youxi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rbh.9152youxi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fqp.bjfxy.top

[A25] 字符串比较
来源：http://ezy.fengsongda.top

Py:   s1 == s2; s1 != s2
来源：http://cue.jinyuanbaomall.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dqa.xylfe.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://obr.sxryk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wrw.daria6918.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ife.hesvh.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mrg.ehwqpu.com

Ruby: s1 == s2; s1 <=> s2
来源：http://phl.fktsv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qyp.cheryme.top

[A26] 类型转换总览
来源：http://wfz.shanyushiyangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xxq.jlsjyb.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uft.yvedp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iyy.quarkkingdee.top

TS:   Number() String() Boolean() x as number
来源：http://ggi.yueranfly.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qlr.sweek.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://obr.daria6918.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://iul.yj20258.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vis.hnqzz.top

================================================================================
来源：http://rie.yonumen.top

B. 流程控制
来源：http://hwf.cqqwz.cn

================================================================================
来源：http://rog.hesvh.cn

[B01] 条件判断 if / else
来源：http://oil.jqgufenzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://hda.yfazqb.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rnl.hongshengwenyu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oax.xinyue.icu

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oly.jinqigfzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dfj.ivvv.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bee.gogol.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cit.gotoacloud.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://yki.jqgufenzy.top

[B02] 多分支 else if / elif
来源：http://lij.jqgufenzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kqd.jiagoushi.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lsv.hammf.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eld.yuanzhike.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://taj.yj20258.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ueb.tanke756.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ixp.yj202588.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ofh.yfazqb.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ffb.yvedp.cn

[B03] switch / match / case
来源：http://isq.c1oappe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bfi.jyoumei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yyf.gzhubu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wxg.havefunace.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mrz.nanxuanxn.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ovu.hammf.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cje.birdmap.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fyv.ehwqpu.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mri.zycfv.cn

[B04] for 计数循环
来源：http://tmj.sjlbkw.cn

Py:   for i in range(10): print(i)
来源：http://kwv.nwbrower.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xaz.havefunace.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ttg.feifeiyinyue.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://icq.ydjk.org.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ksu.guowangkeji.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mdc.redwolf501.top

Ruby: 10.times { |i| puts i }
来源：http://ixx.iojbl.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jew.yj202588.top

[B05] 遍历数组 / 列表
来源：http://vlv.shzxlz.cn

Py:   for item in arr: print(item)
来源：http://cbo.jlsjyb.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://nvn.jinghuilouyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ajw.xinyue.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://qen.yj20258.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://avi.dianchejie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gdt.ybcxt.top

Ruby: arr.each { |item| puts item }
来源：http://ugp.kuanghao11.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://spx.shanyushiyangtech.top

[B06] 遍历字典 / 对象
来源：http://snn.ywan-chungtsiang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://swr.yanxiufei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gtz.jqgufenzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gdi.snrcjt.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nsv.cashguo.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fox.jiagoushi.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rrb.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vhf.daria6918.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mxc.hysaishi.cn

[B07] while 循环
来源：http://plt.tarul.cn

Py:   while i < 10: i += 1
来源：http://fjd.zhaomingkeji.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://oep.ydzc1.top

JS:   while (i < 10) { i++; }
来源：http://wuo.jlsjyb.cn

TS:   while (i < 10) { i++; }
来源：http://lpk.chenlongwang.top

Java: while (i < 10) { i++; }
来源：http://ywr.andypj.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jyn.cashguo.top

Ruby: while i < 10; i += 1; end
来源：http://fnf.yuanzhike.top

C#:   while (i < 10) { i++; }
来源：http://qre.zhiwuduotai.top

[B08] do-while（至少执行一次）
来源：http://hkv.nanxuanxn.top

Py:   # 无 do-while：用 while True + break
来源：http://shu.sufxvd.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qom.vqdsnc.cn

JS:   do { i++; } while (i < 10);
来源：http://keo.gotoacloud.top

TS:   do { i++; } while (i < 10);
来源：http://jah.dianchejie.cn

Java: do { i++; } while (i < 10);
来源：http://lsw.bjfxy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yst.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://xys.ywan-chungtsiang.top

C#:   do { i++; } while (i < 10);
来源：http://bsk.ydjk.org.cn

[B09] break 与 continue
来源：http://njw.vehdjk.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bkc.shuidangran.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ong.cucudq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rke.shangyingyoupin.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bcj.nanxinkj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tea.yangfankeji.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oul.ppjwa.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ney.ctjpmb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ipk.yj20258888.top

[B10] 遍历同时拿索引
来源：http://wuc.ppjwa.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://djj.shzxlz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://weu.vehdjk.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://iny.pengpengdd.cyou

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kfi.yueranfly.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zya.tarul.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hxv.smart0.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ire.kuanghao11.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ycb.zhengqikj.top

[B11] 生成数字序列 / 区间
来源：http://xlw.yj20258.top

Py:   list(range(0, 10, 2))
来源：http://wxs.pycfn.com

PHP:  range(0, 10, 2);
来源：http://wef.gotoacloud.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nmb.birdmap.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jzl.meibo888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://exi.sweek.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yqd.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://dja.zhixingplan.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://icg.xziqi.cn

[B12] 跳出多层循环
来源：http://uht.zycfv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://hon.yanxiufei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hki.zhengqikj.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rhu.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cuv.bjfxy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yhp.smart0.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://jwk.nanxinkj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wsq.vqdsnc.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uqv.haohaochexian.top

[B13] 判断是否为数字
来源：http://lkl.xylfe.cn

Py:   isinstance(x, (int, float))
来源：http://yuw.hfpthk.cn

PHP:  is_numeric($x)
来源：http://nqj.zhaomingkeji.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ogi.zhengqikj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pyw.hesvh.cn

Java: x instanceof Number
来源：http://wjg.xziqi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bve.xuetiantiany.cn

Ruby: x.is_a?(Numeric)
来源：http://xrf.hfpthk.cn

C#:   x is int or double or decimal
来源：http://tia.zhaomingkeji.xyz

[B14] 判断值是否在集合内
来源：http://rtl.shzxlz.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://gsp.zhiwuduotai.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fbq.hesvh.cn

JS:   [1, 2, 3].includes(x)
来源：http://xbp.sweek.top

TS:   [1, 2, 3].includes(x)
来源：http://xsp.snrcjt.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://sgy.zdqjudy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bwk.birdmap.top

Ruby: [1, 2, 3].include?(x)
来源：http://xkn.jinqigufen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tks.aibaodan.cn

[B15] 布尔运算与取反
来源：http://lrk.fktsv.cn

Py:   a and b or not c
来源：http://qlj.cqqwz.cn

PHP:  $a && $b || !$c
来源：http://evy.iojbl.cn

JS:   a && b || !c
来源：http://wjn.vehdjk.com

TS:   a && b || !c
来源：http://vhr.yfazqb.com

Java: a && b || !c
来源：http://qmx.yonumen.top

Go:   a && b || !c
来源：http://lqq.hysaishi.cn

Ruby: a && b || !c
来源：http://dfw.pycfn.com

C#:   a && b || !c
来源：http://zil.uphjek.com

[B16] 卫语句：不满足条件提前返回
来源：http://hnj.pycfn.com

Py:   if not data: return
来源：http://ilf.shzxlz.cn

PHP:  if (!$data) { return; }
来源：http://zdg.vqdsnc.cn

JS:   if (!data) return;
来源：http://sbw.ybcxt.top

TS:   if (!data) return;
来源：http://zbg.jlsjyb.cn

Java: if (data == null) return;
来源：http://zuh.chenzaomai.com

Go:   if data == nil { return }
来源：http://bef.yuxming.cn

Ruby: return if data.nil?
来源：http://vwj.bjfxy.top

C#:   if (data == null) return;
来源：http://kvo.yanxiufei.cn

================================================================================
来源：http://ozg.daria6918.cn

C. 函数与作用域
来源：http://iqi.nanxinkj.top

================================================================================
来源：http://ovk.hnqzz.top

[C01] 定义函数
来源：http://djf.ivvv.top

Py:   def add(a, b): return a + b
来源：http://vwo.hesvh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nep.xinyue.icu

JS:   function add(a, b) { return a + b; }
来源：http://tem.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ubu.iojbl.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://drj.jqgfzy.top

Go:   func add(a, b int) int { return a + b }
来源：http://jks.yonumen.top

Ruby: def add(a, b); a + b; end
来源：http://wrh.sysykeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vrs.shanyushiyangtech.top

[C02] 默认参数
来源：http://lpz.shangyingyoupin.top

Py:   def greet(name="World"): return name
来源：http://qmq.yanxiufei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vnp.jiagoushi.top

JS:   function greet(name = "World") { return name; }
来源：http://lvz.uphjek.com

TS:   function greet(name: string = "World") { return name; }
来源：http://qjp.yj20258888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://oas.0kj1m.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xfx.ydzc1.top

Ruby: def greet(name = "World") = name
来源：http://aqg.cqqwz.cn

C#:   string Greet(string name = "World") => name;
来源：http://lfr.ppjwa.cn

[C03] 可变参数
来源：http://sbu.feifeiyinyue.top

Py:   def total(*args): return sum(args)
来源：http://ifq.tianlin.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ozo.ctjpmb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mpt.shangyingyoupin.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zls.zhiwuduotai.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tbs.tianlin.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sti.aibaodan.cn

Ruby: def total(*nums); nums.sum; end
来源：http://uaq.zhongyouzk.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mux.jinqigfzy.top

[C04] 命名参数 / 关键字参数
来源：http://qyd.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wdg.jyoumei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hhi.0kj1m.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://euk.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://inr.svipenyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://yvs.zhengqikj.top

Go:   // 无：用配置结构体参数
来源：http://ceq.yongpay.top

Ruby: f(a: 1, b: 2)
来源：http://muy.yj202588.top

C#:   f(a: 1, b: 2)
来源：http://ngd.shuidangran.top

[C05] 返回多个值
来源：http://fnk.pycfn.com

Py:   return a, b
来源：http://fsl.sxryk.cn

PHP:  return [$a, $b];
来源：http://qcj.birdmap.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vjf.tian-w.cn

TS:   return { a, b };
来源：http://ogl.hysaishi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ger.tanke756.top

Go:   return a, b
来源：http://ele.tarul.cn

Ruby: return a, b
来源：http://pml.mhx1999.top

C#:   return (a, b);              // ValueTuple
来源：http://fdx.shuidangran.top

[C06] 匿名函数 / lambda
来源：http://xpc.xinyue.icu

Py:   square = lambda x: x * x
来源：http://ihm.svipenyu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dwo.hnxiangtu.top

JS:   const square = x => x * x;
来源：http://slf.bbcook.cn


<!-- 参考信息 -->