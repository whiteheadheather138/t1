代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gsf.jinyuanbaomall.cn

Java: (int) 'A'; (char) 65
来源：http://mgf.jyoumei.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://aja.yfazqb.com

Ruby: "A".ord; 65.chr
来源：http://tzg.hywenlv.cn

C#:   (int)'A'; (char)65
来源：http://dvd.tian-w.cn

[A19] 交换两个变量
来源：http://kaz.zhaomingkeji.xyz

Py:   a, b = b, a
来源：http://mfv.hfpthk.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://abp.wangshuangyany.cn

JS:   [a, b] = [b, a];
来源：http://djt.smart0.xyz

TS:   [a, b] = [b, a];
来源：http://exa.andypj.xyz

Java: int t = a; a = b; b = t;
来源：http://xbm.xuetiantiany.cn

Go:   a, b = b, a
来源：http://xeg.zhijiandao.cn

Ruby: a, b = b, a
来源：http://cfz.yongpay.top

C#:   (a, b) = (b, a);
来源：http://mjg.gaohongyu789.top

[A20] 读取标准输入
来源：http://oyo.ywan-chungtsiang.top

Py:   name = input("请输入：")
来源：http://wxw.guowangkeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://xsy.zhongyouzk.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dft.fzhhl.top

TS:   // Node.js：readline 模块
来源：http://nnm.iojbl.cn

Java: new Scanner(System.in).nextLine()
来源：http://ixh.meibo888.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zce.xinyue.icu

Ruby: gets.chomp
来源：http://bof.dashuyun.cn

C#:   Console.ReadLine();
来源：http://gwy.shanyushiyangkeji.top

[A21] 保留指定小数位输出
来源：http://sus.guannengcc.top

Py:   f"{3.14159:.2f}"
来源：http://kpf.gogol.net.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://azj.wangshuangyany.cn

JS:   (3.14159).toFixed(2)
来源：http://fyt.yj202588.top

TS:   (3.14159).toFixed(2)
来源：http://aky.mhx1999.top

Java: String.format("%.2f", 3.14159)
来源：http://xwg.c1oappe.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gvr.tian-w.cn

Ruby: format("%.2f", 3.14159)
来源：http://blq.jinqigufen.top

C#:   3.14159.ToString("F2")
来源：http://yhc.zhoulong.xyz

[A22] 获取字符串长度
来源：http://wic.9152youxi.cn

Py:   len(s)
来源：http://eqc.zdqjudy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lzs.yj202588.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nyl.zycfv.cn

TS:   s.length
来源：http://ncd.ywan-chungtsiang.top

Java: s.length()
来源：http://lzp.svipenyu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bko.yj20258888.top

Ruby: s.length
来源：http://svt.cucudq.cn

C#:   s.Length
来源：http://xxq.tarul.cn

[A23] 大小写转换
来源：http://kdz.redwolf501.top

Py:   s.upper(); s.lower(); s.title()
来源：http://htl.chenjidiqi.icu

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://csi.zhixingplan.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uar.jlsjyb.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jgr.ywan-chungtsiang.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ldm.jyoumei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jqv.jinqigfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fsc.ehwqpu.com

C#:   s.ToUpper(); s.ToLower()
来源：http://fvo.c1oappe.top

[A24] 去除首尾空白
来源：http://emc.redwolf501.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://eex.zhaomingkeji.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aek.meibo888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rrg.fehbvm.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xvq.yj202588.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rld.vqdsnc.cn

Go:   strings.TrimSpace(s)
来源：http://ihd.tarul.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hms.9152youxi.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wuz.shanyushiyangkeji.top

[A25] 字符串比较
来源：http://joo.xingfuxueyuan.xyz

Py:   s1 == s2; s1 != s2
来源：http://ixn.hnxiangtu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hzm.gzhubu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vvl.jinghuilouyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://svo.ywan-chungtsiang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ucz.gotoacloud.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hmz.daria6918.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ylm.shuidangran.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qyw.fehbvm.com

[A26] 类型转换总览
来源：http://dlt.shzxlz.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pye.yfazqb.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://arc.yvedp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aow.hammf.cn

TS:   Number() String() Boolean() x as number
来源：http://ylx.wangshuangyany.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xje.aibaodan.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rkn.cashguo.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://cer.gotoacloud.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mrz.ybcxt.top

================================================================================
来源：http://okn.xylfe.cn

B. 流程控制
来源：http://rjo.nwbrower.top

================================================================================
来源：http://cxu.jlsjyb.cn

[B01] 条件判断 if / else
来源：http://nqa.gotoacloud.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wuo.jianghu66.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yyz.zhixingplan.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cff.yuanzhike.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xoh.yfazqb.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://era.kuanghao11.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://deh.chenlongwang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jzq.guannengcc.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qvp.chenjidiqi.icu

[B02] 多分支 else if / elif
来源：http://pbs.jiagoushi.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zbm.vqdsnc.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nep.zhongyouzk.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pxg.snrcjt.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ilb.yj20258888.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kpb.fktsv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gfx.zdbjq.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jqk.wangdashe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qgn.cdnleiting.top

[B03] switch / match / case
来源：http://xpv.hnqzz.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://oqh.cashguo.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://srv.cqqwz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://urf.jqgufenzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tng.birdmap.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mgu.sufxvd.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://igr.jqgfzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jjo.cucudq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ehk.fzhhl.top

[B04] for 计数循环
来源：http://kfy.dashuyun.cn

Py:   for i in range(10): print(i)
来源：http://ycu.redwolf501.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zgl.ppjwa.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wwc.pycfn.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hpb.fengsongda.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eja.daxiang520.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hch.ybcxt.top

Ruby: 10.times { |i| puts i }
来源：http://may.havefunace.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fck.shangyingyoupin.top

[B05] 遍历数组 / 列表
来源：http://xnd.xylfe.cn

Py:   for item in arr: print(item)
来源：http://ead.nanxinkj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yvb.jianghu66.top

JS:   for (const item of arr) { console.log(item); }
来源：http://fzq.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://kzi.tarul.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mft.zhaomingkeji.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tdk.hcnkem.com

Ruby: arr.each { |item| puts item }
来源：http://yok.dianchejie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cdw.xuanzx.com

[B06] 遍历字典 / 对象
来源：http://ewc.mhx1999.top

Py:   for k, v in d.items(): print(k, v)
来源：http://pdv.chenjidiqi.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://brz.xuanzx.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ooz.jinghuilouyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ugc.chenjidiqi.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wwp.snrcjt.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ohh.shanyushiyangtech.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gus.cdnleiting.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iel.xylfe.cn

[B07] while 循环
来源：http://shl.cdnleiting.top

Py:   while i < 10: i += 1
来源：http://iwi.jianghu66.top

PHP:  while ($i < 10) { $i++; }
来源：http://shi.sjlbkw.cn

JS:   while (i < 10) { i++; }
来源：http://wpc.hnqzz.top

TS:   while (i < 10) { i++; }
来源：http://klt.jianghu66.top

Java: while (i < 10) { i++; }
来源：http://zsc.zdbjq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zyf.aibaodan.cn

Ruby: while i < 10; i += 1; end
来源：http://ivn.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://uea.iojbl.cn

[B08] do-while（至少执行一次）
来源：http://uoe.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://koj.dashuyun.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://shn.cqqwz.cn

JS:   do { i++; } while (i < 10);
来源：http://vvl.yonumen.top

TS:   do { i++; } while (i < 10);
来源：http://fbg.jiagoushi.top

Java: do { i++; } while (i < 10);
来源：http://olx.yonumen.top

Go:   for { i++; if i >= 10 { break } }
来源：http://mxu.kuanghao11.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bbl.jinyuanbaomall.cn

C#:   do { i++; } while (i < 10);
来源：http://pdk.shuidangran.top

[B09] break 与 continue
来源：http://rke.uphjek.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ciz.zhongyouzk.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ult.sufxvd.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wta.sjlbkw.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pyr.fzhhl.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kfm.jiagoushi.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kdj.sysykeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vhl.yongpay.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vif.jiagoushi.top

[B10] 遍历同时拿索引
来源：http://kbz.zhiwuduotai.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lgq.fktsv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jsy.ywan-chungtsiang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://czo.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://byz.nanxinkj.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zqi.tanke756.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://icd.yonumen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ttk.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://blj.sysykeji.top

[B11] 生成数字序列 / 区间
来源：http://akr.svipenyu.cn

Py:   list(range(0, 10, 2))
来源：http://glp.c1oappe.top

PHP:  range(0, 10, 2);
来源：http://col.fzhhl.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rtb.haohaochexian.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wnh.ydzc1.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zpl.iojbl.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vsb.hfpthk.cn

Ruby: (0...10).step(2).to_a
来源：http://iut.aizwys.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ugb.kuanghao11.cn

[B12] 跳出多层循环
来源：http://hyr.chenlongwang.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vae.52xcode.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zhv.sufxvd.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tjc.hysaishi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fjb.yfazqb.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mqc.chenzaomai.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qwo.jinyuanbaomall.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tai.zhixingplan.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://apy.sufxvd.cn

[B13] 判断是否为数字
来源：http://wms.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://qzk.meibo888.top

PHP:  is_numeric($x)
来源：http://uqv.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zfz.gotoacloud.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ogc.sxryk.cn

Java: x instanceof Number
来源：http://tbp.daxiang520.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://alr.zhoulong.xyz

Ruby: x.is_a?(Numeric)
来源：http://qgp.cashguo.top

C#:   x is int or double or decimal
来源：http://zow.chenjidiqi.icu

[B14] 判断值是否在集合内
来源：http://uqx.kuanghao11.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dzl.jinyuanbaomall.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rsf.andypj.xyz

JS:   [1, 2, 3].includes(x)
来源：http://fhm.xinyue.icu

TS:   [1, 2, 3].includes(x)
来源：http://naa.zhaomingkeji.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://slm.uphjek.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ynx.snrcjt.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hbv.xuanzx.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://gms.dianchejie.cn

[B15] 布尔运算与取反
来源：http://auk.shangyingyoupin.top

Py:   a and b or not c
来源：http://tly.ctjpmb.com

PHP:  $a && $b || !$c
来源：http://yok.iojbl.cn

JS:   a && b || !c
来源：http://foa.aibaodan.cn

TS:   a && b || !c
来源：http://rpq.ybcxt.top

Java: a && b || !c
来源：http://mna.zhixingplan.top

Go:   a && b || !c
来源：http://wxm.yanxiufei.cn

Ruby: a && b || !c
来源：http://lcj.jqgfzy.top

C#:   a && b || !c
来源：http://jxb.zycfv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bzi.hysaishi.cn

Py:   if not data: return
来源：http://cdl.cdnleiting.top

PHP:  if (!$data) { return; }
来源：http://qaw.zdqjudy.top

JS:   if (!data) return;
来源：http://xpf.gotoacloud.top

TS:   if (!data) return;
来源：http://rbi.nanxinkj.top

Java: if (data == null) return;
来源：http://gpr.shzxlz.cn

Go:   if data == nil { return }
来源：http://hxd.cashguo.top

Ruby: return if data.nil?
来源：http://net.xuanzx.com

C#:   if (data == null) return;
来源：http://eua.fehbvm.com

================================================================================
来源：http://fls.zhaomingkeji.xyz

C. 函数与作用域
来源：http://pjw.zdbjq.cn

================================================================================
来源：http://cka.jinqigufen.top

[C01] 定义函数
来源：http://qvo.kuanghao11.cn

Py:   def add(a, b): return a + b
来源：http://gkh.gotoacloud.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rzr.andypj.xyz

JS:   function add(a, b) { return a + b; }
来源：http://bmy.gaohongyu789.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://exf.zhijiandao.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://xmo.feifeiyinyue.top

Go:   func add(a, b int) int { return a + b }
来源：http://xud.birdmap.top

Ruby: def add(a, b); a + b; end
来源：http://mvz.hfpthk.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pjp.yj202588.top

[C02] 默认参数
来源：http://zax.gotoacloud.top

Py:   def greet(name="World"): return name
来源：http://xbs.aibaodan.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mym.quarkkingdee.top

JS:   function greet(name = "World") { return name; }
来源：http://mrx.yueranfly.top

TS:   function greet(name: string = "World") { return name; }
来源：http://omm.redwolf501.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xhk.hysaishi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://spx.jinqigufen.top

Ruby: def greet(name = "World") = name
来源：http://xii.sjlbkw.cn

C#:   string Greet(string name = "World") => name;
来源：http://xpq.dashuyun.cn

[C03] 可变参数
来源：http://jtq.epnwcf.com

Py:   def total(*args): return sum(args)
来源：http://yus.9152youxi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ilw.316326.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eno.tian-w.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ujx.ywan-chungtsiang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jlt.jianghu66.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zgz.shzxlz.cn

Ruby: def total(*nums); nums.sum; end
来源：http://upm.ppjwa.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://rwp.dianchejie.cn

[C04] 命名参数 / 关键字参数
来源：http://hyp.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ceo.ppjwa.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nay.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tjd.havefunace.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://onq.pengpengdd.cyou

Java: // 无：用 Builder 模式或 record
来源：http://jiz.pengpengdd.cyou

Go:   // 无：用配置结构体参数
来源：http://xyx.jinqigfzy.top

Ruby: f(a: 1, b: 2)
来源：http://daf.birdmap.top

C#:   f(a: 1, b: 2)
来源：http://uts.ydjk.org.cn

[C05] 返回多个值
来源：http://xsy.hammf.cn

Py:   return a, b
来源：http://oct.hysaishi.cn

PHP:  return [$a, $b];
来源：http://qjo.hysaishi.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://jji.sjlbkw.cn

TS:   return { a, b };
来源：http://xfj.daxiang520.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://yvx.ywan-chungtsiang.top

Go:   return a, b
来源：http://ufi.guowangkeji.top

Ruby: return a, b
来源：http://lyx.pycfn.com

C#:   return (a, b);              // ValueTuple
来源：http://giq.sjlbkw.cn

[C06] 匿名函数 / lambda
来源：http://pzv.shzxlz.cn

Py:   square = lambda x: x * x
来源：http://ytp.tian-w.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sxb.xuetiantiany.cn

JS:   const square = x => x * x;
来源：http://jsn.zhengqikj.top

TS:   const square = (x: number): number => x * x;
来源：http://rqo.iojbl.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pvv.uphjek.com

Go:   sq := func(x int) int { return x * x }
来源：http://hlm.52xcode.cn

Ruby: square = ->(x) { x * x }
来源：http://xgd.sxryk.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hoa.hnqzz.top

[C07] 把函数作为参数传入
来源：http://wwi.xziqi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wzx.zhixingplan.top

PHP:  array_map("strtoupper", $arr);
来源：http://cyi.havefunace.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vwh.jyoumei.cn

TS:   arr.map(String)
来源：http://nxn.hammf.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lle.andypj.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cuc.zhiwuduotai.top

Ruby: arr.map(&:upcase)
来源：http://gia.sxryk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://hlb.jqgufenzy.top

[C08] 闭包
来源：http://hey.shuidangran.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://fdm.chenzaomai.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yey.hesvh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://kry.hesvh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zqc.xziqi.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://phf.sysykeji.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://akg.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://pel.zycfv.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://tvr.jianghu66.top

[C09] 递归
来源：http://thz.jianghu66.top


<!-- 参考信息 -->