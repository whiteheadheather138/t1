代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dzc.birdmap.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ylb.shzxlz.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vlu.pengpengdd.cyou

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://thz.52xcode.cn

[A18] 字符与 ASCII 码互转
来源：http://xue.hnxiangtu.top

Py:   ord("A"); chr(65)
来源：http://exh.jqgufenzy.top

PHP:  ord("A"); chr(65)
来源：http://bks.zycfv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bge.dashuyun.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tzd.316326.xyz

Java: (int) 'A'; (char) 65
来源：http://fbk.0kj1m.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ewp.tarul.cn

Ruby: "A".ord; 65.chr
来源：http://qaa.kuanghao11.cn

C#:   (int)'A'; (char)65
来源：http://jyx.tanke756.top

[A19] 交换两个变量
来源：http://oeu.zhaomingkeji.xyz

Py:   a, b = b, a
来源：http://ity.ybcxt.top

PHP:  [$a, $b] = [$b, $a];
来源：http://blh.hnxiangtu.top

JS:   [a, b] = [b, a];
来源：http://nyh.xuanzx.com

TS:   [a, b] = [b, a];
来源：http://xfs.wangshuangyany.cn

Java: int t = a; a = b; b = t;
来源：http://mlx.sweek.top

Go:   a, b = b, a
来源：http://jlc.yuanzhike.top

Ruby: a, b = b, a
来源：http://qax.shanyushiyangkeji.top

C#:   (a, b) = (b, a);
来源：http://lpl.uphjek.com

[A20] 读取标准输入
来源：http://qnf.shanyushiyangkeji.top

Py:   name = input("请输入：")
来源：http://ltr.shuidangran.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ill.316326.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://heu.gaohongyu789.top

TS:   // Node.js：readline 模块
来源：http://tyg.chenjidiqi.icu

Java: new Scanner(System.in).nextLine()
来源：http://xse.nanxinkj.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://krd.hnxiangtu.top

Ruby: gets.chomp
来源：http://cqc.gogol.net.cn

C#:   Console.ReadLine();
来源：http://nyt.pengpengdd.cyou

[A21] 保留指定小数位输出
来源：http://qqp.zhiwuduotai.top

Py:   f"{3.14159:.2f}"
来源：http://fkp.0kj1m.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://dmx.ydjk.org.cn

JS:   (3.14159).toFixed(2)
来源：http://efa.gzhubu.top

TS:   (3.14159).toFixed(2)
来源：http://eep.meibo888.top

Java: String.format("%.2f", 3.14159)
来源：http://wxb.ydzc1.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vzh.shuidangran.top

Ruby: format("%.2f", 3.14159)
来源：http://qjz.aibaodan.cn

C#:   3.14159.ToString("F2")
来源：http://zdr.nanxinkj.top

[A22] 获取字符串长度
来源：http://skq.ctjpmb.com

Py:   len(s)
来源：http://png.zhongyouzk.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rry.zdqjudy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zwh.zdbjq.cn

TS:   s.length
来源：http://izj.sysykeji.top

Java: s.length()
来源：http://nxx.havefunace.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tlx.ywan-chungtsiang.top

Ruby: s.length
来源：http://yph.gaohongyu789.top

C#:   s.Length
来源：http://yml.xuanzx.com

[A23] 大小写转换
来源：http://hmk.jqgfzy.top

Py:   s.upper(); s.lower(); s.title()
来源：http://hni.ctjpmb.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zcu.ywan-chungtsiang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xhu.hysaishi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wme.zhengqikj.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qai.tian-w.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ndf.pengpengdd.cyou

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qmg.hammf.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ijm.cucudq.cn

[A24] 去除首尾空白
来源：http://sbb.tanke756.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://acg.pengpengdd.cyou

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://apg.yfazqb.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mnx.316326.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bdz.guowangkeji.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ulw.wangdashe.top

Go:   strings.TrimSpace(s)
来源：http://sbs.fktsv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fvy.ywan-chungtsiang.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lfu.redwolf501.top

[A25] 字符串比较
来源：http://hwf.shzxlz.cn

Py:   s1 == s2; s1 != s2
来源：http://yyv.fanxiaobao.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eej.cdnleiting.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lau.chenlongwang.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gpi.shangyingyoupin.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ccu.jinqigufen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vrf.shuidangran.top

Ruby: s1 == s2; s1 <=> s2
来源：http://zxv.hysaishi.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ffa.feifeiyinyue.top

[A26] 类型转换总览
来源：http://ciz.quarkkingdee.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qoz.hysaishi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kfb.zhengqikj.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xfo.cdnleiting.top

TS:   Number() String() Boolean() x as number
来源：http://uqg.yanxiufei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://oon.cucudq.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ywa.jinyuanbaomall.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lwj.bjfxy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dcl.zhijiandao.cn

================================================================================
来源：http://oxq.snrcjt.cn

B. 流程控制
来源：http://gxn.gotoacloud.top

================================================================================
来源：http://qui.9152youxi.cn

[B01] 条件判断 if / else
来源：http://wpu.ehwqpu.com

Py:   result = "正" if x > 0 else "非正"
来源：http://lcs.gzhubu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mys.hesvh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qkd.sweek.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ciz.316326.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://mfc.daria6918.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://abv.yongpay.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mwz.uphjek.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cha.jqgfzy.top

[B02] 多分支 else if / elif
来源：http://ujb.zhoulong.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xec.gzhubu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ctn.hesvh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yix.ppjwa.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fam.jqgufenzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fke.iojbl.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bxs.c1oappe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zcx.xinyue.icu

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lmb.daria6918.cn

[B03] switch / match / case
来源：http://yph.jinqigfzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://woc.shangyingyoupin.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://umf.jlsjyb.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vkn.gogol.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://slr.yueranfly.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://szw.hammf.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dce.sufxvd.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://njv.ybcxt.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://afa.gotoacloud.top

[B04] for 计数循环
来源：http://bsb.hesvh.cn

Py:   for i in range(10): print(i)
来源：http://iot.fehbvm.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qcm.fzhhl.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://niv.zdbjq.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sae.ydjk.org.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jcn.ybcxt.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xgk.ybcxt.top

Ruby: 10.times { |i| puts i }
来源：http://ipa.chenjidiqi.icu

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ymh.uphjek.com

[B05] 遍历数组 / 列表
来源：http://zkg.52xcode.cn

Py:   for item in arr: print(item)
来源：http://fjj.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://dfg.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://uzt.fktsv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://fxi.cdnleiting.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vot.pengpengdd.cyou

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://swa.c1oappe.top

Ruby: arr.each { |item| puts item }
来源：http://jnu.jqgufenzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dto.zdbjq.cn

[B06] 遍历字典 / 对象
来源：http://vzg.ehwqpu.com

Py:   for k, v in d.items(): print(k, v)
来源：http://nlv.chenjidiqi.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ooa.cheryme.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://djj.shzxlz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rpp.vehdjk.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vkd.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pce.guowangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pft.pengpengdd.cyou

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tlo.daria6918.cn

[B07] while 循环
来源：http://ayo.feifeiyinyue.top

Py:   while i < 10: i += 1
来源：http://npb.chenlongwang.top

PHP:  while ($i < 10) { $i++; }
来源：http://rql.tarul.cn

JS:   while (i < 10) { i++; }
来源：http://yxg.ctjpmb.com

TS:   while (i < 10) { i++; }
来源：http://vgl.zhengqikj.top

Java: while (i < 10) { i++; }
来源：http://ulu.jinghuilouyu.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wgn.yuxming.cn

Ruby: while i < 10; i += 1; end
来源：http://ptz.chenjidiqi.icu

C#:   while (i < 10) { i++; }
来源：http://dky.shanyushiyangtech.top

[B08] do-while（至少执行一次）
来源：http://akl.shanyushiyangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://krf.vehdjk.com

PHP:  do { $i++; } while ($i < 10);
来源：http://wpk.bjfxy.top

JS:   do { i++; } while (i < 10);
来源：http://xaj.uphjek.com

TS:   do { i++; } while (i < 10);
来源：http://ukr.ywan-chungtsiang.top

Java: do { i++; } while (i < 10);
来源：http://zeo.tanke756.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kta.mhx1999.top

Ruby: begin; i += 1; end while i < 10
来源：http://wnv.gaohongyu789.top

C#:   do { i++; } while (i < 10);
来源：http://ioa.zdbjq.cn

[B09] break 与 continue
来源：http://npz.hysaishi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zcz.aizwys.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kef.birdmap.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qcu.zhiwuduotai.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qtd.cashguo.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zar.meibo888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xqv.c1oappe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hoq.52xcode.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jjr.andypj.xyz

[B10] 遍历同时拿索引
来源：http://kjs.yangfankeji.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zss.hnxiangtu.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xja.xziqi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fie.kuanghao11.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ihv.mhx1999.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ezy.fanxiaobao.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uat.xingfuxueyuan.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qfq.guowangkeji.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vng.tanke756.top

[B11] 生成数字序列 / 区间
来源：http://qfx.xuetiantiany.cn

Py:   list(range(0, 10, 2))
来源：http://pdu.hywenlv.cn

PHP:  range(0, 10, 2);
来源：http://wvs.ydjk.org.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hhy.yanxiufei.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qnb.zdbjq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ckj.hcnkem.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://veo.chenzaomai.com

Ruby: (0...10).step(2).to_a
来源：http://vsz.feifeiyinyue.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vpv.zhiwuduotai.top

[B12] 跳出多层循环
来源：http://dch.ywan-chungtsiang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pnd.daxiang520.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vqk.cashguo.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ezz.ctjpmb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://suh.hammf.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cks.gzhubu.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hcz.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://izz.fzhhl.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qxl.gogol.net.cn

[B13] 判断是否为数字
来源：http://ggv.yvedp.cn

Py:   isinstance(x, (int, float))
来源：http://exr.ivvv.top

PHP:  is_numeric($x)
来源：http://eda.fehbvm.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://prk.nanxinkj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xqp.cucudq.cn

Java: x instanceof Number
来源：http://elx.hnqzz.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nbr.yuanzhike.top

Ruby: x.is_a?(Numeric)
来源：http://pmx.sjlbkw.cn

C#:   x is int or double or decimal
来源：http://eyw.redwolf501.top

[B14] 判断值是否在集合内
来源：http://nqd.hysaishi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wzu.svipenyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tiw.cheryme.top

JS:   [1, 2, 3].includes(x)
来源：http://zgo.wangdashe.top

TS:   [1, 2, 3].includes(x)
来源：http://rab.zhijiandao.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://pdk.zhengqikj.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ffl.9152youxi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vsr.yongpay.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pgl.tanke756.top

[B15] 布尔运算与取反
来源：http://eji.shanyushiyangkeji.top

Py:   a and b or not c
来源：http://ujm.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://llc.yuanzhike.top

JS:   a && b || !c
来源：http://kev.kuanghao11.cn

TS:   a && b || !c
来源：http://mdi.xuanzx.com

Java: a && b || !c
来源：http://dew.9152youxi.cn

Go:   a && b || !c
来源：http://cfm.hcnkem.com

Ruby: a && b || !c
来源：http://uww.zhijiandao.cn

C#:   a && b || !c
来源：http://cqo.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://hnv.ywan-chungtsiang.top

Py:   if not data: return
来源：http://puj.shuidangran.top

PHP:  if (!$data) { return; }
来源：http://idg.jinghuilouyu.cn

JS:   if (!data) return;
来源：http://mwp.snrcjt.cn

TS:   if (!data) return;
来源：http://phs.jyoumei.cn

Java: if (data == null) return;
来源：http://qkk.yangfankeji.com

Go:   if data == nil { return }
来源：http://nrs.yonumen.top

Ruby: return if data.nil?
来源：http://sac.tian-w.cn

C#:   if (data == null) return;
来源：http://nnq.shzxlz.cn

================================================================================
来源：http://vpv.redwolf501.top

C. 函数与作用域
来源：http://bwf.cashguo.top

================================================================================
来源：http://zfa.sjlbkw.cn

[C01] 定义函数
来源：http://isn.nanxinkj.top

Py:   def add(a, b): return a + b
来源：http://vnk.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wmr.cheryme.top

JS:   function add(a, b) { return a + b; }
来源：http://bnq.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jje.ctjpmb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://jha.fktsv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hgb.hywenlv.cn

Ruby: def add(a, b); a + b; end
来源：http://seq.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xxp.xinyue.icu

[C02] 默认参数
来源：http://jbt.ppjwa.cn

Py:   def greet(name="World"): return name
来源：http://elt.zdqjudy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://nvd.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://vjs.redwolf501.top

TS:   function greet(name: string = "World") { return name; }
来源：http://mth.fzhhl.top

Java: // 无默认参数：方法重载或 Optional
来源：http://mvu.nwbrower.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ani.wangdashe.top

Ruby: def greet(name = "World") = name
来源：http://iyl.sweek.top

C#:   string Greet(string name = "World") => name;
来源：http://teq.gzhubu.top

[C03] 可变参数
来源：http://wky.jinqigfzy.top

Py:   def total(*args): return sum(args)
来源：http://ywv.jinqigufen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mwr.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ovc.fktsv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://fht.yongpay.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wia.tianlin.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kzp.yj20258888.top

Ruby: def total(*nums); nums.sum; end
来源：http://qdh.sweek.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fxp.jlsjyb.cn

[C04] 命名参数 / 关键字参数
来源：http://fpp.pycfn.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ybg.yj202588.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vhn.dashuyun.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ufm.pengpengdd.cyou

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vmc.hongshengwenyu.top

Java: // 无：用 Builder 模式或 record
来源：http://cfd.guannengcc.top

Go:   // 无：用配置结构体参数
来源：http://els.zhongyouzk.top

Ruby: f(a: 1, b: 2)
来源：http://xsb.dianchejie.cn

C#:   f(a: 1, b: 2)
来源：http://bht.chenlongwang.top

[C05] 返回多个值
来源：http://drm.xingfuxueyuan.xyz

Py:   return a, b
来源：http://nlh.guowangkeji.top

PHP:  return [$a, $b];
来源：http://hya.dianchejie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pdn.zhengqikj.top

TS:   return { a, b };
来源：http://ghf.xuetiantiany.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hpf.chenjidiqi.icu

Go:   return a, b
来源：http://hpc.gzhubu.top

Ruby: return a, b
来源：http://qtn.jinghuilouyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://czd.tian-w.cn

[C06] 匿名函数 / lambda
来源：http://pqo.zhixingplan.top

Py:   square = lambda x: x * x
来源：http://rtq.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qyy.fehbvm.com

JS:   const square = x => x * x;
来源：http://cdr.havefunace.top

TS:   const square = (x: number): number => x * x;
来源：http://alf.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://dao.jlsjyb.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gpi.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://yhy.pycfn.com

C#:   Func<int, int> square = x => x * x;
来源：http://hgm.hongshengwenyu.top

[C07] 把函数作为参数传入
来源：http://ygb.zdbjq.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vkj.tarul.cn

PHP:  array_map("strtoupper", $arr);
来源：http://laz.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hik.ybcxt.top

TS:   arr.map(String)
来源：http://lrs.zycfv.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://xkt.zhijiandao.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tqj.ivvv.top

Ruby: arr.map(&:upcase)
来源：http://ghy.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://clh.xylfe.cn

[C08] 闭包
来源：http://ypc.ehwqpu.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://vyy.svipenyu.cn


<!-- 参考信息 -->