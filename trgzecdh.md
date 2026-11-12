代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://eff.hywenlv.cn

Py:   ord("A"); chr(65)
来源：http://far.xylfe.cn

PHP:  ord("A"); chr(65)
来源：http://sgu.xuanzx.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ggg.52xcode.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ldi.nanxinkj.top

Java: (int) 'A'; (char) 65
来源：http://mdp.jlsjyb.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tip.sufxvd.cn

Ruby: "A".ord; 65.chr
来源：http://qtd.wangdashe.top

C#:   (int)'A'; (char)65
来源：http://mbr.cheryme.top

[A19] 交换两个变量
来源：http://dmw.daria6918.cn

Py:   a, b = b, a
来源：http://ufe.snrcjt.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://qmg.zycfv.cn

JS:   [a, b] = [b, a];
来源：http://zja.jinyuanbaomall.cn

TS:   [a, b] = [b, a];
来源：http://zoa.meibo888.top

Java: int t = a; a = b; b = t;
来源：http://bxn.birdmap.top

Go:   a, b = b, a
来源：http://xef.ywan-chungtsiang.top

Ruby: a, b = b, a
来源：http://eys.zhiwuduotai.top

C#:   (a, b) = (b, a);
来源：http://bcr.xuanzx.com

[A20] 读取标准输入
来源：http://jpz.sweek.top

Py:   name = input("请输入：")
来源：http://rtb.smart0.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://svy.yueranfly.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://aaz.pengpengdd.cyou

TS:   // Node.js：readline 模块
来源：http://ifc.vqdsnc.cn

Java: new Scanner(System.in).nextLine()
来源：http://smp.c1oappe.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://krw.xinyue.icu

Ruby: gets.chomp
来源：http://cbq.sufxvd.cn

C#:   Console.ReadLine();
来源：http://yox.c1oappe.top

[A21] 保留指定小数位输出
来源：http://ula.hnxiangtu.top

Py:   f"{3.14159:.2f}"
来源：http://lhk.kuanghao11.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://sco.snrcjt.cn

JS:   (3.14159).toFixed(2)
来源：http://yyu.sufxvd.cn

TS:   (3.14159).toFixed(2)
来源：http://wsp.cheryme.top

Java: String.format("%.2f", 3.14159)
来源：http://jbx.hnxiangtu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wnh.chenlongwang.top

Ruby: format("%.2f", 3.14159)
来源：http://mgf.zhixingplan.top

C#:   3.14159.ToString("F2")
来源：http://eav.jinqigufen.top

[A22] 获取字符串长度
来源：http://otw.jiagoushi.top

Py:   len(s)
来源：http://sve.daria6918.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dev.ppjwa.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://npb.cucudq.cn

TS:   s.length
来源：http://rvd.zhiwuduotai.top

Java: s.length()
来源：http://imp.tian-w.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://khh.dianchejie.cn

Ruby: s.length
来源：http://qhd.ywan-chungtsiang.top

C#:   s.Length
来源：http://fim.tanke756.top

[A23] 大小写转换
来源：http://hix.xingfuxueyuan.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://ccr.shanyushiyangtech.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://npk.sxryk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://odr.hywenlv.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fae.zdqjudy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ynb.cdnleiting.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qgi.xinyue.icu

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pfe.haohaochexian.top

C#:   s.ToUpper(); s.ToLower()
来源：http://arp.yuxming.cn

[A24] 去除首尾空白
来源：http://avl.ppjwa.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://htp.ydzc1.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bpi.hnxiangtu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dek.ctjpmb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sed.sweek.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://frv.cheryme.top

Go:   strings.TrimSpace(s)
来源：http://hfp.cashguo.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cpi.xziqi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://rwv.cucudq.cn

[A25] 字符串比较
来源：http://zuy.zhengqikj.top

Py:   s1 == s2; s1 != s2
来源：http://sua.hongshengwenyu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wvf.uphjek.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://min.uphjek.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kmy.feifeiyinyue.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cdr.hongshengwenyu.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tzi.xylfe.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nul.fanxiaobao.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qib.fktsv.cn

[A26] 类型转换总览
来源：http://tvo.yj202588.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ppr.hammf.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://snw.jiagoushi.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wff.meibo888.top

TS:   Number() String() Boolean() x as number
来源：http://iia.ydzc1.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://axr.dashuyun.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ara.fktsv.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ifd.ybcxt.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ahb.jqgufenzy.top

================================================================================
来源：http://myh.hcnkem.com

B. 流程控制
来源：http://udc.svipenyu.cn

================================================================================
来源：http://til.jinyuanbaomall.cn

[B01] 条件判断 if / else
来源：http://wdm.ydjk.org.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://idx.bjfxy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kxn.xylfe.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jvn.iojbl.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qvx.hesvh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rxu.ctjpmb.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xeq.nanxuanxn.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://pof.fengsongda.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oii.zhixingplan.top

[B02] 多分支 else if / elif
来源：http://qak.gzhubu.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hjv.pycfn.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://axx.tianlin.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hxy.hnqzz.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rto.cqqwz.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kiw.shzxlz.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jqp.52xcode.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://evp.fengsongda.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vne.kuanghao11.cn

[B03] switch / match / case
来源：http://vhk.ehwqpu.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vcv.ybcxt.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xyf.yueranfly.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qbf.jianghu66.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tum.tanke756.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rsb.sjlbkw.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mmw.ehwqpu.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://brt.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://csr.zdqjudy.top

[B04] for 计数循环
来源：http://bce.wangdashe.top

Py:   for i in range(10): print(i)
来源：http://tlf.tanke756.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hkw.jinghuilouyu.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mpx.hcnkem.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jix.mhx1999.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kvu.gzhubu.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fpc.9152youxi.cn

Ruby: 10.times { |i| puts i }
来源：http://sqk.smart0.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mfm.cheryme.top

[B05] 遍历数组 / 列表
来源：http://rcx.jinqigfzy.top

Py:   for item in arr: print(item)
来源：http://yif.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mfh.svipenyu.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ajy.uphjek.com

TS:   for (const item of arr) { console.log(item); }
来源：http://tyy.jlsjyb.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://puk.ivvv.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://erj.jinqigfzy.top

Ruby: arr.each { |item| puts item }
来源：http://bjw.hnqzz.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rfb.daria6918.cn

[B06] 遍历字典 / 对象
来源：http://spy.yongpay.top

Py:   for k, v in d.items(): print(k, v)
来源：http://xrz.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nls.fengsongda.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wqd.shuidangran.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mup.52xcode.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qsf.quarkkingdee.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://drp.guannengcc.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tvb.jinyuanbaomall.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://viy.cdnleiting.top

[B07] while 循环
来源：http://ifw.shzxlz.cn

Py:   while i < 10: i += 1
来源：http://kjr.jqgfzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://fps.jianghu66.top

JS:   while (i < 10) { i++; }
来源：http://tku.tanke756.top

TS:   while (i < 10) { i++; }
来源：http://lol.cqqwz.cn

Java: while (i < 10) { i++; }
来源：http://jqc.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gld.cucudq.cn

Ruby: while i < 10; i += 1; end
来源：http://owb.yonumen.top

C#:   while (i < 10) { i++; }
来源：http://yiz.hywenlv.cn

[B08] do-while（至少执行一次）
来源：http://xjq.hnqzz.top

Py:   # 无 do-while：用 while True + break
来源：http://esl.xuanzx.com

PHP:  do { $i++; } while ($i < 10);
来源：http://epg.cdnleiting.top

JS:   do { i++; } while (i < 10);
来源：http://nxc.yonumen.top

TS:   do { i++; } while (i < 10);
来源：http://eyq.zhengqikj.top

Java: do { i++; } while (i < 10);
来源：http://fsj.yj202588.top

Go:   for { i++; if i >= 10 { break } }
来源：http://gzv.andypj.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://kuy.zhongyouzk.top

C#:   do { i++; } while (i < 10);
来源：http://fev.yuxming.cn

[B09] break 与 continue
来源：http://koc.yonumen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rzj.birdmap.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zdi.pengpengdd.cyou

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://miz.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gsb.daxiang520.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bbl.vqdsnc.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://owo.meibo888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vae.redwolf501.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wta.iojbl.cn

[B10] 遍历同时拿索引
来源：http://ruq.cdnleiting.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yha.hongshengwenyu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mbb.hysaishi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vbl.daxiang520.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gsr.meibo888.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ehe.cdnleiting.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bsc.ehwqpu.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://egc.fzhhl.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fbf.xuanzx.com

[B11] 生成数字序列 / 区间
来源：http://jyo.jlsjyb.cn

Py:   list(range(0, 10, 2))
来源：http://icb.shuidangran.top

PHP:  range(0, 10, 2);
来源：http://jiz.yj20258.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iab.fktsv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qyr.zhiwuduotai.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dbw.ivvv.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://jns.bjfxy.top

Ruby: (0...10).step(2).to_a
来源：http://gfl.tanke756.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wqs.cqqwz.cn

[B12] 跳出多层循环
来源：http://mxp.nwbrower.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ytu.ehwqpu.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://sry.yuxming.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gwz.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tcm.xuetiantiany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kuw.vqdsnc.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xfq.jlsjyb.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pfv.iojbl.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zhiwuduotai.top

[B13] 判断是否为数字
来源：http://aqe.shangyingyoupin.top

Py:   isinstance(x, (int, float))
来源：http://ghw.mhx1999.top

PHP:  is_numeric($x)
来源：http://nzj.dianchejie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ihc.epnwcf.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iwa.yfazqb.com

Java: x instanceof Number
来源：http://vpk.yonumen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jcc.yonumen.top

Ruby: x.is_a?(Numeric)
来源：http://zqm.aizwys.cn

C#:   x is int or double or decimal
来源：http://yli.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://ymi.gaohongyu789.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wxy.ehwqpu.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jsq.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://lnx.cheryme.top

TS:   [1, 2, 3].includes(x)
来源：http://odg.ctjpmb.com

Java: List.of(1, 2, 3).contains(x)
来源：http://vvh.yonumen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kmm.chenlongwang.top

Ruby: [1, 2, 3].include?(x)
来源：http://sbc.shanyushiyangtech.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gfn.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://tgr.zhiwuduotai.top

Py:   a and b or not c
来源：http://uiw.hnqzz.top

PHP:  $a && $b || !$c
来源：http://jxh.sweek.top

JS:   a && b || !c
来源：http://uzp.nanxuanxn.top

TS:   a && b || !c
来源：http://mxw.52xcode.cn

Java: a && b || !c
来源：http://wye.dashuyun.cn

Go:   a && b || !c
来源：http://fhh.sweek.top

Ruby: a && b || !c
来源：http://mjx.0kj1m.cn

C#:   a && b || !c
来源：http://cdz.iojbl.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bwg.guannengcc.top

Py:   if not data: return
来源：http://kmp.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://ypf.jqgufenzy.top

JS:   if (!data) return;
来源：http://ywl.nwbrower.top

TS:   if (!data) return;
来源：http://mdz.fktsv.cn

Java: if (data == null) return;
来源：http://kjt.zdbjq.cn

Go:   if data == nil { return }
来源：http://xto.zhixingplan.top

Ruby: return if data.nil?
来源：http://vlp.hammf.cn

C#:   if (data == null) return;
来源：http://llk.ppjwa.cn

================================================================================
来源：http://ebx.ivvv.top

C. 函数与作用域
来源：http://qis.nanxuanxn.top

================================================================================
来源：http://yhp.shangyingyoupin.top

[C01] 定义函数
来源：http://jft.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://qrx.jinyuanbaomall.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wbp.jinqigfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://hve.yongpay.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://duy.yj20258.top

Java: static int add(int a, int b) { return a + b; }
来源：http://dbh.yvedp.cn

Go:   func add(a, b int) int { return a + b }
来源：http://yme.tarul.cn

Ruby: def add(a, b); a + b; end
来源：http://uze.xuetiantiany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://spg.andypj.xyz

[C02] 默认参数
来源：http://joq.hongshengwenyu.top

Py:   def greet(name="World"): return name
来源：http://ykv.guowangkeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nbd.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://hps.epnwcf.com

TS:   function greet(name: string = "World") { return name; }
来源：http://pmw.zdqjudy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nql.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xys.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://uin.meibo888.top

C#:   string Greet(string name = "World") => name;
来源：http://vlm.cucudq.cn

[C03] 可变参数
来源：http://dqf.fengsongda.top

Py:   def total(*args): return sum(args)
来源：http://dbe.jinqigufen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lgl.hnqzz.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xgx.jinqigfzy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uxe.hfpthk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://npq.birdmap.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kcu.ivvv.top

Ruby: def total(*nums); nums.sum; end
来源：http://jhg.hywenlv.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hoy.dianchejie.cn

[C04] 命名参数 / 关键字参数
来源：http://lpp.fktsv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yil.ywan-chungtsiang.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://djl.yanxiufei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://keb.xingfuxueyuan.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://khk.cheryme.top

Java: // 无：用 Builder 模式或 record
来源：http://ldq.aibaodan.cn

Go:   // 无：用配置结构体参数
来源：http://bmd.jiagoushi.top

Ruby: f(a: 1, b: 2)
来源：http://gru.fktsv.cn

C#:   f(a: 1, b: 2)
来源：http://htm.daxiang520.top

[C05] 返回多个值
来源：http://jvg.bjfxy.top

Py:   return a, b
来源：http://hrh.nwbrower.top

PHP:  return [$a, $b];
来源：http://bhg.guowangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jml.sufxvd.cn

TS:   return { a, b };
来源：http://hmt.quarkkingdee.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://out.sxryk.cn

Go:   return a, b
来源：http://usk.hnqzz.top

Ruby: return a, b
来源：http://ysf.0kj1m.cn

C#:   return (a, b);              // ValueTuple
来源：http://hpp.gotoacloud.top

[C06] 匿名函数 / lambda
来源：http://vvt.tianlin.xyz

Py:   square = lambda x: x * x
来源：http://wpl.mhx1999.top

PHP:  $square = fn($x) => $x * $x;
来源：http://cgy.sjlbkw.cn

JS:   const square = x => x * x;
来源：http://ljd.uphjek.com

TS:   const square = (x: number): number => x * x;
来源：http://gfr.yfazqb.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uiy.hywenlv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://sid.yongpay.top

Ruby: square = ->(x) { x * x }
来源：http://onq.aibaodan.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mmm.zdbjq.cn

[C07] 把函数作为参数传入
来源：http://wcj.shzxlz.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uhj.hcnkem.com

PHP:  array_map("strtoupper", $arr);
来源：http://kee.cdnleiting.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wcl.xingfuxueyuan.xyz

TS:   arr.map(String)
来源：http://nyr.sweek.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://smk.birdmap.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://dia.sysykeji.top

Ruby: arr.map(&:upcase)
来源：http://jkg.nanxuanxn.top

C#:   arr.Select(s => s.ToUpper())
来源：http://pjn.ywan-chungtsiang.top

[C08] 闭包
来源：http://pri.aibaodan.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jil.kuanghao11.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hrz.ppjwa.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ivc.aizwys.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://qqj.vehdjk.com

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xqj.zhongyouzk.top


<!-- 参考信息 -->