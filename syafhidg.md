代发 wailian999

C#:   (int)'A'; (char)65
来源：http://fwm.fzhhl.top

[A19] 交换两个变量
来源：http://piq.hnqzz.top

Py:   a, b = b, a
来源：http://fme.meibo888.top

PHP:  [$a, $b] = [$b, $a];
来源：http://dov.jinghuilouyu.cn

JS:   [a, b] = [b, a];
来源：http://ilt.shzxlz.cn

TS:   [a, b] = [b, a];
来源：http://otf.hnxiangtu.top

Java: int t = a; a = b; b = t;
来源：http://eid.jinyuanbaomall.cn

Go:   a, b = b, a
来源：http://txj.hammf.cn

Ruby: a, b = b, a
来源：http://wjq.gaohongyu789.top

C#:   (a, b) = (b, a);
来源：http://mlz.guannengcc.top

[A20] 读取标准输入
来源：http://uzy.gaohongyu789.top

Py:   name = input("请输入：")
来源：http://fzs.jyoumei.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://agb.tarul.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qbd.pycfn.com

TS:   // Node.js：readline 模块
来源：http://okm.ehwqpu.com

Java: new Scanner(System.in).nextLine()
来源：http://zcj.hfpthk.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://llr.jinyuanbaomall.cn

Ruby: gets.chomp
来源：http://hqm.wangshuangyany.cn

C#:   Console.ReadLine();
来源：http://hud.fehbvm.com

[A21] 保留指定小数位输出
来源：http://pst.sxryk.cn

Py:   f"{3.14159:.2f}"
来源：http://ouu.iojbl.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cwe.feifeiyinyue.top

JS:   (3.14159).toFixed(2)
来源：http://sao.aibaodan.cn

TS:   (3.14159).toFixed(2)
来源：http://nkw.haohaochexian.top

Java: String.format("%.2f", 3.14159)
来源：http://qgz.zycfv.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eee.52xcode.cn

Ruby: format("%.2f", 3.14159)
来源：http://bir.andypj.xyz

C#:   3.14159.ToString("F2")
来源：http://npx.fengsongda.top

[A22] 获取字符串长度
来源：http://ike.shanyushiyangkeji.top

Py:   len(s)
来源：http://fau.hysaishi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://joz.bjfxy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jya.zhixingplan.top

TS:   s.length
来源：http://aaw.zycfv.cn

Java: s.length()
来源：http://zpm.snrcjt.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hdw.kuanghao11.cn

Ruby: s.length
来源：http://xzp.zhoulong.xyz

C#:   s.Length
来源：http://rxk.daria6918.cn

[A23] 大小写转换
来源：http://zfd.ybcxt.top

Py:   s.upper(); s.lower(); s.title()
来源：http://win.hongshengwenyu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xif.ppjwa.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yil.ybcxt.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tqd.sysykeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ffr.yuxming.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dso.pengpengdd.cyou

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nws.shangyingyoupin.top

C#:   s.ToUpper(); s.ToLower()
来源：http://din.xylfe.cn

[A24] 去除首尾空白
来源：http://qmr.gzhubu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mmx.epnwcf.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rqr.ydjk.org.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kzt.smart0.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tis.hongshengwenyu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://uox.dashuyun.cn

Go:   strings.TrimSpace(s)
来源：http://btj.jqgufenzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lli.jqgfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sbh.zycfv.cn

[A25] 字符串比较
来源：http://yfo.shanyushiyangtech.top

Py:   s1 == s2; s1 != s2
来源：http://dce.jyoumei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://olq.nanxinkj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sao.tarul.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mes.cucudq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xlu.dashuyun.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fpy.zhixingplan.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ijc.shuidangran.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fwr.ydzc1.top

[A26] 类型转换总览
来源：http://csa.tian-w.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mhq.zdbjq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tnm.jlsjyb.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rbx.hywenlv.cn

TS:   Number() String() Boolean() x as number
来源：http://wdg.wangdashe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ztd.shangyingyoupin.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ohu.9152youxi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ynz.fehbvm.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uye.ybcxt.top

================================================================================
来源：http://ghw.yuanzhike.top

B. 流程控制
来源：http://oqx.mhx1999.top

================================================================================
来源：http://voe.gaohongyu789.top

[B01] 条件判断 if / else
来源：http://rsv.ydjk.org.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://zpe.mhx1999.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://elz.fktsv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rgx.svipenyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bhi.vqdsnc.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wfi.yonumen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://syy.birdmap.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kgd.fehbvm.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ijw.ivvv.top

[B02] 多分支 else if / elif
来源：http://kwx.zhoulong.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rfh.jinqigufen.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://iir.yj20258888.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dju.zhijiandao.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jnh.ydjk.org.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mks.yfazqb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iih.bbcook.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rzl.wangdashe.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qgf.zhixingplan.top

[B03] switch / match / case
来源：http://top.316326.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cbg.guowangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kdc.epnwcf.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yqo.jlsjyb.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://agl.aizwys.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fcu.sufxvd.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://afw.yonumen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bop.316326.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://egw.52xcode.cn

[B04] for 计数循环
来源：http://bha.hongshengwenyu.top

Py:   for i in range(10): print(i)
来源：http://vcl.hcnkem.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://tai.andypj.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gno.hnqzz.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pbk.bjfxy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ste.yj202588.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://evf.svipenyu.cn

Ruby: 10.times { |i| puts i }
来源：http://mue.fengsongda.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pte.fengsongda.top

[B05] 遍历数组 / 列表
来源：http://qse.hesvh.cn

Py:   for item in arr: print(item)
来源：http://blr.c1oappe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rmd.jyoumei.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://oee.meibo888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ixj.mhx1999.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hhe.jqgufenzy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kkg.guowangkeji.top

Ruby: arr.each { |item| puts item }
来源：http://pdo.shangyingyoupin.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://msp.ydzc1.top

[B06] 遍历字典 / 对象
来源：http://iqv.hcnkem.com

Py:   for k, v in d.items(): print(k, v)
来源：http://wpp.9152youxi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jvq.jiagoushi.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kue.zhengqikj.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gie.bjfxy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ggs.sweek.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hcg.jqgfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://job.hywenlv.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aqs.yj202588.top

[B07] while 循环
来源：http://qvq.zhengqikj.top

Py:   while i < 10: i += 1
来源：http://twt.hesvh.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tkj.fanxiaobao.xyz

JS:   while (i < 10) { i++; }
来源：http://mhn.xinyue.icu

TS:   while (i < 10) { i++; }
来源：http://guv.xuetiantiany.cn

Java: while (i < 10) { i++; }
来源：http://rrz.smart0.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dva.tian-w.cn

Ruby: while i < 10; i += 1; end
来源：http://pyj.fehbvm.com

C#:   while (i < 10) { i++; }
来源：http://lkb.aibaodan.cn

[B08] do-while（至少执行一次）
来源：http://loa.jyoumei.cn

Py:   # 无 do-while：用 while True + break
来源：http://hld.fktsv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gts.hfpthk.cn

JS:   do { i++; } while (i < 10);
来源：http://yiu.jiagoushi.top

TS:   do { i++; } while (i < 10);
来源：http://oup.fengsongda.top

Java: do { i++; } while (i < 10);
来源：http://hmx.andypj.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://mwv.yvedp.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rxj.aizwys.cn

C#:   do { i++; } while (i < 10);
来源：http://yap.cucudq.cn

[B09] break 与 continue
来源：http://yyq.birdmap.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kba.ivvv.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ldp.guowangkeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ret.kuanghao11.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ubb.snrcjt.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fhh.0kj1m.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oml.hongshengwenyu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lfa.daxiang520.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://swq.zdbjq.cn

[B10] 遍历同时拿索引
来源：http://pot.nwbrower.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kom.52xcode.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zzp.smart0.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ipm.vqdsnc.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ptp.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://grp.birdmap.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ntx.yj20258.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qse.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tmq.wangdashe.top

[B11] 生成数字序列 / 区间
来源：http://mot.nwbrower.top

Py:   list(range(0, 10, 2))
来源：http://lda.zhongyouzk.top

PHP:  range(0, 10, 2);
来源：http://osp.redwolf501.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sql.fzhhl.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dxn.gaohongyu789.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aua.mhx1999.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sgc.hysaishi.cn

Ruby: (0...10).step(2).to_a
来源：http://gbo.shanyushiyangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jib.jinqigufen.top

[B12] 跳出多层循环
来源：http://eom.sufxvd.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://mon.fzhhl.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://vme.jinqigfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gek.iojbl.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://azd.yanxiufei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jsl.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oyf.birdmap.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cla.hcnkem.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cgt.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://ajs.sxryk.cn

Py:   isinstance(x, (int, float))
来源：http://sur.yongpay.top

PHP:  is_numeric($x)
来源：http://jpq.sysykeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gyu.sxryk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://shj.jinyuanbaomall.cn

Java: x instanceof Number
来源：http://rel.hfpthk.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sav.ppjwa.cn

Ruby: x.is_a?(Numeric)
来源：http://eix.andypj.xyz

C#:   x is int or double or decimal
来源：http://nwm.wangshuangyany.cn

[B14] 判断值是否在集合内
来源：http://xws.jinqigfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ucc.ppjwa.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ctu.yj20258888.top

JS:   [1, 2, 3].includes(x)
来源：http://vqz.zhijiandao.cn

TS:   [1, 2, 3].includes(x)
来源：http://qqg.ydzc1.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gvu.nwbrower.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vkd.xziqi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zep.andypj.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qpc.nwbrower.top

[B15] 布尔运算与取反
来源：http://rfq.xingfuxueyuan.xyz

Py:   a and b or not c
来源：http://zcb.jinyuanbaomall.cn

PHP:  $a && $b || !$c
来源：http://uky.yonumen.top

JS:   a && b || !c
来源：http://grp.bbcook.cn

TS:   a && b || !c
来源：http://ylk.zdqjudy.top

Java: a && b || !c
来源：http://xgm.cqqwz.cn

Go:   a && b || !c
来源：http://dzn.hcnkem.com

Ruby: a && b || !c
来源：http://qpn.zhijiandao.cn

C#:   a && b || !c
来源：http://cov.iojbl.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vxz.mhx1999.top

Py:   if not data: return
来源：http://gyz.c1oappe.top

PHP:  if (!$data) { return; }
来源：http://ndh.iojbl.cn

JS:   if (!data) return;
来源：http://vxe.sweek.top

TS:   if (!data) return;
来源：http://pzi.chenlongwang.top

Java: if (data == null) return;
来源：http://bwp.yonumen.top

Go:   if data == nil { return }
来源：http://dno.pycfn.com

Ruby: return if data.nil?
来源：http://ysh.ehwqpu.com

C#:   if (data == null) return;
来源：http://wrg.jinqigufen.top

================================================================================
来源：http://zyo.wangdashe.top

C. 函数与作用域
来源：http://qcj.smart0.xyz

================================================================================
来源：http://qjc.yuanzhike.top

[C01] 定义函数
来源：http://tee.bbcook.cn

Py:   def add(a, b): return a + b
来源：http://pba.sufxvd.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://klp.hfpthk.cn

JS:   function add(a, b) { return a + b; }
来源：http://idt.uphjek.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dwh.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://vxx.tian-w.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ppo.sxryk.cn

Ruby: def add(a, b); a + b; end
来源：http://aeg.jlsjyb.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fga.jqgufenzy.top

[C02] 默认参数
来源：http://zal.zhaomingkeji.xyz

Py:   def greet(name="World"): return name
来源：http://wqc.aizwys.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://eul.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://hll.kuanghao11.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zup.316326.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://aps.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fsn.shuidangran.top

Ruby: def greet(name = "World") = name
来源：http://qia.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://ema.svipenyu.cn

[C03] 可变参数
来源：http://dlk.snrcjt.cn

Py:   def total(*args): return sum(args)
来源：http://llh.yvedp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pza.jqgfzy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hvm.aibaodan.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cif.wangshuangyany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://unt.andypj.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://fnd.bbcook.cn

Ruby: def total(*nums); nums.sum; end
来源：http://jrs.daxiang520.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nfc.sufxvd.cn

[C04] 命名参数 / 关键字参数
来源：http://juw.pycfn.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jrx.svipenyu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vkc.hnxiangtu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fle.dianchejie.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xzu.xylfe.cn

Java: // 无：用 Builder 模式或 record
来源：http://att.ybcxt.top

Go:   // 无：用配置结构体参数
来源：http://qzq.shangyingyoupin.top

Ruby: f(a: 1, b: 2)
来源：http://sur.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://wdx.zhengqikj.top

[C05] 返回多个值
来源：http://jjm.feifeiyinyue.top

Py:   return a, b
来源：http://wkn.jianghu66.top

PHP:  return [$a, $b];
来源：http://myx.sxryk.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bgg.zdbjq.cn

TS:   return { a, b };
来源：http://unk.birdmap.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dcy.hongshengwenyu.top

Go:   return a, b
来源：http://gfm.ctjpmb.com

Ruby: return a, b
来源：http://omr.quarkkingdee.top

C#:   return (a, b);              // ValueTuple
来源：http://xzj.hongshengwenyu.top

[C06] 匿名函数 / lambda
来源：http://iim.hfpthk.cn

Py:   square = lambda x: x * x
来源：http://bhf.tanke756.top

PHP:  $square = fn($x) => $x * $x;
来源：http://bua.zhixingplan.top

JS:   const square = x => x * x;
来源：http://wan.xinyue.icu

TS:   const square = (x: number): number => x * x;
来源：http://rma.andypj.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://icq.wangshuangyany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qbf.yvedp.cn

Ruby: square = ->(x) { x * x }
来源：http://yul.hnqzz.top

C#:   Func<int, int> square = x => x * x;
来源：http://zbs.iojbl.cn

[C07] 把函数作为参数传入
来源：http://kjk.jianghu66.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lhe.gogol.net.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ywe.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://osx.fktsv.cn

TS:   arr.map(String)
来源：http://uiu.hnxiangtu.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://nga.dashuyun.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://clw.nanxinkj.top

Ruby: arr.map(&:upcase)
来源：http://mbt.uphjek.com

C#:   arr.Select(s => s.ToUpper())
来源：http://tgy.gzhubu.top

[C08] 闭包
来源：http://rfj.jyoumei.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aew.aizwys.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uis.andypj.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rfk.gotoacloud.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lxs.sysykeji.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qap.jlsjyb.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dlw.pycfn.com

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zap.daria6918.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://jnx.pycfn.com

[C09] 递归
来源：http://eth.vehdjk.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://fok.aibaodan.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://kju.hfpthk.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qcl.nwbrower.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://lnz.tarul.cn


<!-- 参考信息 -->