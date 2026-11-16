代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://vlt.cheryme.top

Py:   ord("A"); chr(65)
来源：http://shk.ydzc1.top

PHP:  ord("A"); chr(65)
来源：http://kva.fzhhl.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ver.cqqwz.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rgs.cucudq.cn

Java: (int) 'A'; (char) 65
来源：http://znp.ppjwa.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yzx.ehwqpu.com

Ruby: "A".ord; 65.chr
来源：http://zsc.gotoacloud.top

C#:   (int)'A'; (char)65
来源：http://ykn.daxiang520.top

[A19] 交换两个变量
来源：http://zvr.chenlongwang.top

Py:   a, b = b, a
来源：http://ngx.feifeiyinyue.top

PHP:  [$a, $b] = [$b, $a];
来源：http://jzs.yongpay.top

JS:   [a, b] = [b, a];
来源：http://ntx.dashuyun.cn

TS:   [a, b] = [b, a];
来源：http://yqw.zhoulong.xyz

Java: int t = a; a = b; b = t;
来源：http://tjj.ppjwa.cn

Go:   a, b = b, a
来源：http://dqj.shanyushiyangtech.top

Ruby: a, b = b, a
来源：http://zme.cucudq.cn

C#:   (a, b) = (b, a);
来源：http://jfw.aizwys.cn

[A20] 读取标准输入
来源：http://kmj.nanxinkj.top

Py:   name = input("请输入：")
来源：http://qdb.vqdsnc.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yrz.jyoumei.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jhe.fengsongda.top

TS:   // Node.js：readline 模块
来源：http://xnz.jinqigufen.top

Java: new Scanner(System.in).nextLine()
来源：http://man.zhengqikj.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zen.cucudq.cn

Ruby: gets.chomp
来源：http://pkh.jinqigufen.top

C#:   Console.ReadLine();
来源：http://fgf.yfazqb.com

[A21] 保留指定小数位输出
来源：http://utd.aibaodan.cn

Py:   f"{3.14159:.2f}"
来源：http://ahk.tanke756.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ffg.cdnleiting.top

JS:   (3.14159).toFixed(2)
来源：http://scm.xylfe.cn

TS:   (3.14159).toFixed(2)
来源：http://qzm.nanxuanxn.top

Java: String.format("%.2f", 3.14159)
来源：http://fnu.hammf.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://jyd.snrcjt.cn

Ruby: format("%.2f", 3.14159)
来源：http://olt.cheryme.top

C#:   3.14159.ToString("F2")
来源：http://gzc.ppjwa.cn

[A22] 获取字符串长度
来源：http://dah.xuetiantiany.cn

Py:   len(s)
来源：http://uud.fehbvm.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jej.chenlongwang.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cdc.snrcjt.cn

TS:   s.length
来源：http://hyv.tanke756.top

Java: s.length()
来源：http://zsc.chenzaomai.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gyb.yfazqb.com

Ruby: s.length
来源：http://iek.kuanghao11.cn

C#:   s.Length
来源：http://pni.tian-w.cn

[A23] 大小写转换
来源：http://qzw.xingfuxueyuan.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://onl.ydjk.org.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gkd.sjlbkw.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tch.chenzaomai.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bko.smart0.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sgz.xuetiantiany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ggb.pengpengdd.cyou

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pdw.jinqigufen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rpw.jinyuanbaomall.cn

[A24] 去除首尾空白
来源：http://xme.aizwys.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nlq.yueranfly.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aip.vehdjk.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kjw.yj20258888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oeg.smart0.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qlx.tanke756.top

Go:   strings.TrimSpace(s)
来源：http://mct.mhx1999.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lsw.meibo888.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://opb.ehwqpu.com

[A25] 字符串比较
来源：http://juf.nanxinkj.top

Py:   s1 == s2; s1 != s2
来源：http://xyk.zhengqikj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ccz.bbcook.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gwq.vehdjk.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dyg.aibaodan.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pdf.zhoulong.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ajh.ybcxt.top

Ruby: s1 == s2; s1 <=> s2
来源：http://eqz.dianchejie.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sqg.yfazqb.com

[A26] 类型转换总览
来源：http://ewk.guowangkeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://msx.xuetiantiany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://uwb.zhongyouzk.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zme.jianghu66.top

TS:   Number() String() Boolean() x as number
来源：http://gcq.zhaomingkeji.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://qdt.c1oappe.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ukq.nanxinkj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://izz.zhengqikj.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vsv.jiagoushi.top

================================================================================
来源：http://has.svipenyu.cn

B. 流程控制
来源：http://lkf.snrcjt.cn

================================================================================
来源：http://xhi.pengpengdd.cyou

[B01] 条件判断 if / else
来源：http://sek.nanxuanxn.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jfp.bjfxy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xef.aibaodan.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ncc.dashuyun.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ndk.guannengcc.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://nda.yonumen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jcg.yueranfly.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vrx.cashguo.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oai.yanxiufei.cn

[B02] 多分支 else if / elif
来源：http://drx.yj202588.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tvd.aibaodan.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://itn.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nyi.cheryme.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cfn.shangyingyoupin.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mny.shanyushiyangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rus.sweek.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rua.pycfn.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tec.fktsv.cn

[B03] switch / match / case
来源：http://rcg.hongshengwenyu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kfi.hnxiangtu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bqj.xingfuxueyuan.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hxz.jinghuilouyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iyg.cdnleiting.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cao.andypj.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jye.zhijiandao.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zbu.aibaodan.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zfj.sweek.top

[B04] for 计数循环
来源：http://xep.jianghu66.top

Py:   for i in range(10): print(i)
来源：http://ted.jinqigfzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ozv.sweek.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://myz.smart0.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ucl.feifeiyinyue.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ank.zhiwuduotai.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://sam.aizwys.cn

Ruby: 10.times { |i| puts i }
来源：http://wui.gotoacloud.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pqx.yueranfly.top

[B05] 遍历数组 / 列表
来源：http://kky.xuanzx.com

Py:   for item in arr: print(item)
来源：http://ubo.sxryk.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jsh.xingfuxueyuan.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://cft.fzhhl.top

TS:   for (const item of arr) { console.log(item); }
来源：http://dpd.yongpay.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://isx.hnxiangtu.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wav.mhx1999.top

Ruby: arr.each { |item| puts item }
来源：http://ydn.yangfankeji.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://krp.aizwys.cn

[B06] 遍历字典 / 对象
来源：http://pwp.feifeiyinyue.top

Py:   for k, v in d.items(): print(k, v)
来源：http://cww.kuanghao11.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hon.aibaodan.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qmt.xuetiantiany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://met.fanxiaobao.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hvv.chenjidiqi.icu

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mhc.nanxuanxn.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nax.shzxlz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bps.zycfv.cn

[B07] while 循环
来源：http://ucu.ydjk.org.cn

Py:   while i < 10: i += 1
来源：http://zrf.yuanzhike.top

PHP:  while ($i < 10) { $i++; }
来源：http://bzm.cdnleiting.top

JS:   while (i < 10) { i++; }
来源：http://dns.nanxinkj.top

TS:   while (i < 10) { i++; }
来源：http://xkm.ywan-chungtsiang.top

Java: while (i < 10) { i++; }
来源：http://yie.zhixingplan.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://gpu.sweek.top

Ruby: while i < 10; i += 1; end
来源：http://vyr.guowangkeji.top

C#:   while (i < 10) { i++; }
来源：http://cbx.yfazqb.com

[B08] do-while（至少执行一次）
来源：http://ahj.zycfv.cn

Py:   # 无 do-while：用 while True + break
来源：http://dim.zhongyouzk.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kre.316326.xyz

JS:   do { i++; } while (i < 10);
来源：http://rki.chenlongwang.top

TS:   do { i++; } while (i < 10);
来源：http://aia.jqgufenzy.top

Java: do { i++; } while (i < 10);
来源：http://uid.yuanzhike.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mct.zhaomingkeji.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://czz.316326.xyz

C#:   do { i++; } while (i < 10);
来源：http://qir.jinqigfzy.top

[B09] break 与 continue
来源：http://tjr.meibo888.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mio.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ver.jqgfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bzv.shuidangran.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pry.ehwqpu.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pcu.yj20258.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kki.dianchejie.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://csx.xuetiantiany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ara.hcnkem.com

[B10] 遍历同时拿索引
来源：http://eut.pengpengdd.cyou

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rog.jiagoushi.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vsr.sweek.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://adq.zhongyouzk.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kqi.kuanghao11.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://arx.kuanghao11.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uwb.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fdh.chenlongwang.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dse.jiagoushi.top

[B11] 生成数字序列 / 区间
来源：http://nby.andypj.xyz

Py:   list(range(0, 10, 2))
来源：http://twf.jiagoushi.top

PHP:  range(0, 10, 2);
来源：http://jdu.shzxlz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xxu.yangfankeji.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://znt.yvedp.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://han.yj202588.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://goc.mhx1999.top

Ruby: (0...10).step(2).to_a
来源：http://ooz.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fwx.jinghuilouyu.cn

[B12] 跳出多层循环
来源：http://uxw.fktsv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qta.cqqwz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jtx.hysaishi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ber.yongpay.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qmx.nanxuanxn.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cfi.dianchejie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zce.sjlbkw.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nyb.pengpengdd.cyou

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cjm.hammf.cn

[B13] 判断是否为数字
来源：http://oul.jinqigfzy.top

Py:   isinstance(x, (int, float))
来源：http://ren.xylfe.cn

PHP:  is_numeric($x)
来源：http://xle.ywan-chungtsiang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xra.316326.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tsn.andypj.xyz

Java: x instanceof Number
来源：http://afi.jyoumei.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ldm.havefunace.top

Ruby: x.is_a?(Numeric)
来源：http://wlj.zhixingplan.top

C#:   x is int or double or decimal
来源：http://jnd.jiagoushi.top

[B14] 判断值是否在集合内
来源：http://hkj.cdnleiting.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wur.zdbjq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://dbx.yvedp.cn

JS:   [1, 2, 3].includes(x)
来源：http://nnu.ctjpmb.com

TS:   [1, 2, 3].includes(x)
来源：http://uob.fzhhl.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bmc.xinyue.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dzr.aizwys.cn

Ruby: [1, 2, 3].include?(x)
来源：http://cxn.ivvv.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cju.yvedp.cn

[B15] 布尔运算与取反
来源：http://lee.fzhhl.top

Py:   a and b or not c
来源：http://pmh.ywan-chungtsiang.top

PHP:  $a && $b || !$c
来源：http://cex.yj20258.top

JS:   a && b || !c
来源：http://idq.jqgfzy.top

TS:   a && b || !c
来源：http://nkd.pycfn.com

Java: a && b || !c
来源：http://dig.jiagoushi.top

Go:   a && b || !c
来源：http://fcw.shuidangran.top

Ruby: a && b || !c
来源：http://tvx.shanyushiyangtech.top

C#:   a && b || !c
来源：http://fyz.yj20258888.top

[B16] 卫语句：不满足条件提前返回
来源：http://cas.yj20258888.top

Py:   if not data: return
来源：http://edu.uphjek.com

PHP:  if (!$data) { return; }
来源：http://vju.sjlbkw.cn

JS:   if (!data) return;
来源：http://aot.pengpengdd.cyou

TS:   if (!data) return;
来源：http://oge.gaohongyu789.top

Java: if (data == null) return;
来源：http://bix.bjfxy.top

Go:   if data == nil { return }
来源：http://zmw.chenjidiqi.icu

Ruby: return if data.nil?
来源：http://wga.xuanzx.com

C#:   if (data == null) return;
来源：http://bot.hfpthk.cn

================================================================================
来源：http://mpj.tarul.cn

C. 函数与作用域
来源：http://xod.zhixingplan.top

================================================================================
来源：http://gzr.bbcook.cn

[C01] 定义函数
来源：http://xkx.yuanzhike.top

Py:   def add(a, b): return a + b
来源：http://lvc.xingfuxueyuan.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kuf.ydzc1.top

JS:   function add(a, b) { return a + b; }
来源：http://ygx.sjlbkw.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yun.yj20258.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xva.vehdjk.com

Go:   func add(a, b int) int { return a + b }
来源：http://geg.nanxinkj.top

Ruby: def add(a, b); a + b; end
来源：http://gat.aizwys.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xfu.gaohongyu789.top

[C02] 默认参数
来源：http://grm.hnxiangtu.top

Py:   def greet(name="World"): return name
来源：http://xrc.ppjwa.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://vjy.tanke756.top

JS:   function greet(name = "World") { return name; }
来源：http://lid.chenjidiqi.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://eiu.shanyushiyangtech.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qpa.bjfxy.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fga.jinqigufen.top

Ruby: def greet(name = "World") = name
来源：http://dju.jinqigufen.top

C#:   string Greet(string name = "World") => name;
来源：http://rij.jiagoushi.top

[C03] 可变参数
来源：http://nbo.zhengqikj.top

Py:   def total(*args): return sum(args)
来源：http://vvj.ybcxt.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ret.zhiwuduotai.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kip.pengpengdd.cyou

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://olh.haohaochexian.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jlr.gaohongyu789.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fxs.zdbjq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lbn.yangfankeji.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xgy.yj202588.top

[C04] 命名参数 / 关键字参数
来源：http://qfq.zdbjq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pqd.ehwqpu.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xwu.zhongyouzk.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zle.hongshengwenyu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qbb.jyoumei.cn

Java: // 无：用 Builder 模式或 record
来源：http://vef.shzxlz.cn

Go:   // 无：用配置结构体参数
来源：http://gjb.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://fcx.shangyingyoupin.top

C#:   f(a: 1, b: 2)
来源：http://jzl.zhaomingkeji.xyz

[C05] 返回多个值
来源：http://dce.zhixingplan.top

Py:   return a, b
来源：http://kzf.mhx1999.top

PHP:  return [$a, $b];
来源：http://nly.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://vvz.tanke756.top

TS:   return { a, b };
来源：http://qro.gogol.net.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jzg.hysaishi.cn

Go:   return a, b
来源：http://hyp.gotoacloud.top

Ruby: return a, b
来源：http://ure.yongpay.top

C#:   return (a, b);              // ValueTuple
来源：http://heq.jlsjyb.cn

[C06] 匿名函数 / lambda
来源：http://fdl.zhixingplan.top

Py:   square = lambda x: x * x
来源：http://mll.hesvh.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ajl.yj20258.top

JS:   const square = x => x * x;
来源：http://aec.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://ioy.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tql.fanxiaobao.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://uia.gotoacloud.top

Ruby: square = ->(x) { x * x }
来源：http://cpv.yangfankeji.com

C#:   Func<int, int> square = x => x * x;
来源：http://swt.epnwcf.com

[C07] 把函数作为参数传入
来源：http://ivh.uphjek.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hwr.ehwqpu.com

PHP:  array_map("strtoupper", $arr);
来源：http://mtd.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ugk.xinyue.icu

TS:   arr.map(String)
来源：http://qzu.hammf.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tol.jinghuilouyu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://alh.fengsongda.top

Ruby: arr.map(&:upcase)
来源：http://jqk.c1oappe.top

C#:   arr.Select(s => s.ToUpper())
来源：http://gda.guannengcc.top

[C08] 闭包
来源：http://xwr.bjfxy.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ztx.havefunace.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vqp.0kj1m.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bdg.ctjpmb.com

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://yzz.kuanghao11.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kpm.fzhhl.top


<!-- 参考信息 -->