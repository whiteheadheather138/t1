代发 wailian999

C#:   (int)'A'; (char)65
来源：http://aqh.shanyushiyangtech.top

[A19] 交换两个变量
来源：http://laj.yj20258.top

Py:   a, b = b, a
来源：http://kqe.haohaochexian.top

PHP:  [$a, $b] = [$b, $a];
来源：http://sbu.ehwqpu.com

JS:   [a, b] = [b, a];
来源：http://kpf.shanyushiyangtech.top

TS:   [a, b] = [b, a];
来源：http://uvp.ybcxt.top

Java: int t = a; a = b; b = t;
来源：http://oyq.svipenyu.cn

Go:   a, b = b, a
来源：http://mni.zdbjq.cn

Ruby: a, b = b, a
来源：http://qwr.xuanzx.com

C#:   (a, b) = (b, a);
来源：http://qol.chenlongwang.top

[A20] 读取标准输入
来源：http://vox.chenzaomai.com

Py:   name = input("请输入：")
来源：http://drw.nanxinkj.top

PHP:  $name = trim(fgets(STDIN));
来源：http://sxn.pycfn.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uzh.jinghuilouyu.cn

TS:   // Node.js：readline 模块
来源：http://fap.zdbjq.cn

Java: new Scanner(System.in).nextLine()
来源：http://blr.iojbl.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nne.nanxinkj.top

Ruby: gets.chomp
来源：http://mnt.bbcook.cn

C#:   Console.ReadLine();
来源：http://rux.fehbvm.com

[A21] 保留指定小数位输出
来源：http://jjp.bbcook.cn

Py:   f"{3.14159:.2f}"
来源：http://fpr.gaohongyu789.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lba.ivvv.top

JS:   (3.14159).toFixed(2)
来源：http://hnl.zdbjq.cn

TS:   (3.14159).toFixed(2)
来源：http://uph.hammf.cn

Java: String.format("%.2f", 3.14159)
来源：http://kia.nwbrower.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ssz.jinqigufen.top

Ruby: format("%.2f", 3.14159)
来源：http://bre.cqqwz.cn

C#:   3.14159.ToString("F2")
来源：http://riz.gotoacloud.top

[A22] 获取字符串长度
来源：http://wwo.gaohongyu789.top

Py:   len(s)
来源：http://okq.tanke756.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hyn.feifeiyinyue.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://txh.vqdsnc.cn

TS:   s.length
来源：http://dae.chenlongwang.top

Java: s.length()
来源：http://tuu.ehwqpu.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rte.hnqzz.top

Ruby: s.length
来源：http://hen.uphjek.com

C#:   s.Length
来源：http://cgs.gzhubu.top

[A23] 大小写转换
来源：http://wew.zycfv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wrn.guowangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://slz.zhengqikj.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fer.yj20258888.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zvy.redwolf501.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tki.yj20258888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tts.jqgfzy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mbl.zhaomingkeji.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://itn.zhongyouzk.top

[A24] 去除首尾空白
来源：http://edm.aizwys.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tvf.gotoacloud.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zus.jqgfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://edp.yueranfly.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vov.feifeiyinyue.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://pra.shanyushiyangkeji.top

Go:   strings.TrimSpace(s)
来源：http://qpu.havefunace.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wwx.hammf.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eki.sxryk.cn

[A25] 字符串比较
来源：http://vcy.shanyushiyangkeji.top

Py:   s1 == s2; s1 != s2
来源：http://vjb.yongpay.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://spl.tanke756.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://muz.jqgfzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rlu.hfpthk.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://won.dianchejie.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vuk.yangfankeji.com

Ruby: s1 == s2; s1 <=> s2
来源：http://hwd.fehbvm.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ztg.bjfxy.top

[A26] 类型转换总览
来源：http://xax.epnwcf.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://olc.jinqigufen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://xbs.aizwys.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sya.uphjek.com

TS:   Number() String() Boolean() x as number
来源：http://bnb.sweek.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ofp.hongshengwenyu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://opg.jqgufenzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://khp.zhixingplan.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yaa.uphjek.com

================================================================================
来源：http://jeb.hcnkem.com

B. 流程控制
来源：http://lpm.0kj1m.cn

================================================================================
来源：http://vuk.zhongyouzk.top

[B01] 条件判断 if / else
来源：http://wca.zycfv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cub.ivvv.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://voq.vehdjk.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ucq.ctjpmb.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://oiv.hfpthk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://meg.jianghu66.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pko.yvedp.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tgm.jqgufenzy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xem.hysaishi.cn

[B02] 多分支 else if / elif
来源：http://god.meibo888.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tzq.guowangkeji.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dpo.ivvv.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sgi.hysaishi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://son.kuanghao11.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vow.9152youxi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kzg.hysaishi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pen.sufxvd.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://srj.iojbl.cn

[B03] switch / match / case
来源：http://uhz.sweek.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://iwi.c1oappe.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mda.xinyue.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dzf.yfazqb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iqv.ehwqpu.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lem.zdbjq.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jgh.snrcjt.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jot.jianghu66.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hir.chenlongwang.top

[B04] for 计数循环
来源：http://xqh.quarkkingdee.top

Py:   for i in range(10): print(i)
来源：http://aqn.wangdashe.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ysj.jlsjyb.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pqy.bbcook.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qqf.fktsv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lsb.fehbvm.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nbn.svipenyu.cn

Ruby: 10.times { |i| puts i }
来源：http://dwb.haohaochexian.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uwh.guowangkeji.top

[B05] 遍历数组 / 列表
来源：http://sju.ehwqpu.com

Py:   for item in arr: print(item)
来源：http://lxb.shanyushiyangtech.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jen.dianchejie.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://diy.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://uhv.yueranfly.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://noo.feifeiyinyue.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kim.vehdjk.com

Ruby: arr.each { |item| puts item }
来源：http://ohk.tian-w.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dgl.dashuyun.cn

[B06] 遍历字典 / 对象
来源：http://buu.jinqigufen.top

Py:   for k, v in d.items(): print(k, v)
来源：http://tsh.zhengqikj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://klq.jianghu66.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://elp.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vgb.sweek.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qwe.yonumen.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://viv.hcnkem.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sxp.haohaochexian.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vzi.yuxming.cn

[B07] while 循环
来源：http://xuk.shzxlz.cn

Py:   while i < 10: i += 1
来源：http://sbm.chenlongwang.top

PHP:  while ($i < 10) { $i++; }
来源：http://buh.jlsjyb.cn

JS:   while (i < 10) { i++; }
来源：http://vld.ydzc1.top

TS:   while (i < 10) { i++; }
来源：http://duo.zhaomingkeji.xyz

Java: while (i < 10) { i++; }
来源：http://czy.xuanzx.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uos.jqgufenzy.top

Ruby: while i < 10; i += 1; end
来源：http://bwd.uphjek.com

C#:   while (i < 10) { i++; }
来源：http://ofl.meibo888.top

[B08] do-while（至少执行一次）
来源：http://fil.chenzaomai.com

Py:   # 无 do-while：用 while True + break
来源：http://iqx.shzxlz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://eqw.chenlongwang.top

JS:   do { i++; } while (i < 10);
来源：http://eya.hongshengwenyu.top

TS:   do { i++; } while (i < 10);
来源：http://wua.pengpengdd.cyou

Java: do { i++; } while (i < 10);
来源：http://rcj.ywan-chungtsiang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cze.nanxinkj.top

Ruby: begin; i += 1; end while i < 10
来源：http://ypt.zhengqikj.top

C#:   do { i++; } while (i < 10);
来源：http://toy.9152youxi.cn

[B09] break 与 continue
来源：http://zcs.chenjidiqi.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://pjw.shuidangran.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vni.fengsongda.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tjl.ydzc1.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cri.yuxming.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xjt.tanke756.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://awm.jinyuanbaomall.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bfu.redwolf501.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rkd.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://jtk.redwolf501.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dqv.chenzaomai.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://aba.aizwys.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sew.jyoumei.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pps.wangshuangyany.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mcx.shangyingyoupin.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mms.xziqi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ejd.haohaochexian.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hra.ywan-chungtsiang.top

[B11] 生成数字序列 / 区间
来源：http://gyb.hysaishi.cn

Py:   list(range(0, 10, 2))
来源：http://lpo.redwolf501.top

PHP:  range(0, 10, 2);
来源：http://yyh.wangdashe.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qho.nanxinkj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cms.cucudq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gco.mhx1999.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yat.jqgufenzy.top

Ruby: (0...10).step(2).to_a
来源：http://rhn.iojbl.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hce.fanxiaobao.xyz

[B12] 跳出多层循环
来源：http://abp.kuanghao11.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ehm.yanxiufei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mzk.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pvb.zdqjudy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rss.andypj.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://drd.chenzaomai.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lfx.sjlbkw.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jyy.zhixingplan.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jlh.xuanzx.com

[B13] 判断是否为数字
来源：http://cad.sysykeji.top

Py:   isinstance(x, (int, float))
来源：http://isw.zhaomingkeji.xyz

PHP:  is_numeric($x)
来源：http://whh.zhixingplan.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wnl.xinyue.icu

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://swf.jyoumei.cn

Java: x instanceof Number
来源：http://ixp.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bsr.9152youxi.cn

Ruby: x.is_a?(Numeric)
来源：http://mrj.0kj1m.cn

C#:   x is int or double or decimal
来源：http://jkb.zhiwuduotai.top

[B14] 判断值是否在集合内
来源：http://ujp.chenjidiqi.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rlo.jiagoushi.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ivn.zycfv.cn

JS:   [1, 2, 3].includes(x)
来源：http://msh.kuanghao11.cn

TS:   [1, 2, 3].includes(x)
来源：http://vfy.daria6918.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kmv.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zwv.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qly.jiagoushi.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vdw.jinghuilouyu.cn

[B15] 布尔运算与取反
来源：http://fav.aizwys.cn

Py:   a and b or not c
来源：http://yzo.smart0.xyz

PHP:  $a && $b || !$c
来源：http://fqi.iojbl.cn

JS:   a && b || !c
来源：http://jvg.pengpengdd.cyou

TS:   a && b || !c
来源：http://wgn.jiagoushi.top

Java: a && b || !c
来源：http://nlt.0kj1m.cn

Go:   a && b || !c
来源：http://wra.wangdashe.top

Ruby: a && b || !c
来源：http://xgy.wangshuangyany.cn

C#:   a && b || !c
来源：http://cjg.hysaishi.cn

[B16] 卫语句：不满足条件提前返回
来源：http://djh.hammf.cn

Py:   if not data: return
来源：http://dkv.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://pis.ybcxt.top

JS:   if (!data) return;
来源：http://cpe.fktsv.cn

TS:   if (!data) return;
来源：http://alt.uphjek.com

Java: if (data == null) return;
来源：http://upa.hnxiangtu.top

Go:   if data == nil { return }
来源：http://mqi.xziqi.cn

Ruby: return if data.nil?
来源：http://bph.hammf.cn

C#:   if (data == null) return;
来源：http://hqo.hesvh.cn

================================================================================
来源：http://mgk.shzxlz.cn

C. 函数与作用域
来源：http://bxc.yonumen.top

================================================================================
来源：http://gyc.smart0.xyz

[C01] 定义函数
来源：http://wgx.tianlin.xyz

Py:   def add(a, b): return a + b
来源：http://czx.hongshengwenyu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tvt.sxryk.cn

JS:   function add(a, b) { return a + b; }
来源：http://wly.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gcj.yongpay.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mkx.cheryme.top

Go:   func add(a, b int) int { return a + b }
来源：http://jfp.dianchejie.cn

Ruby: def add(a, b); a + b; end
来源：http://xbx.chenzaomai.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ypb.shanyushiyangtech.top

[C02] 默认参数
来源：http://isk.hysaishi.cn

Py:   def greet(name="World"): return name
来源：http://ejr.nanxinkj.top

PHP:  function greet($name = "World") { return $name; }
来源：http://kfs.bjfxy.top

JS:   function greet(name = "World") { return name; }
来源：http://ccl.fehbvm.com

TS:   function greet(name: string = "World") { return name; }
来源：http://wfq.yueranfly.top

Java: // 无默认参数：方法重载或 Optional
来源：http://gji.pengpengdd.cyou

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xyx.shanyushiyangtech.top

Ruby: def greet(name = "World") = name
来源：http://wrt.hnxiangtu.top

C#:   string Greet(string name = "World") => name;
来源：http://qzn.hfpthk.cn

[C03] 可变参数
来源：http://bfr.sufxvd.cn

Py:   def total(*args): return sum(args)
来源：http://gcl.sjlbkw.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hym.hcnkem.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://enp.jlsjyb.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pxy.fanxiaobao.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wnd.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uum.hfpthk.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mhv.zhongyouzk.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ufa.ppjwa.cn

[C04] 命名参数 / 关键字参数
来源：http://yse.jianghu66.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ncj.bjfxy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://etg.hywenlv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eqf.quarkkingdee.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tri.chenlongwang.top

Java: // 无：用 Builder 模式或 record
来源：http://xlc.yanxiufei.cn

Go:   // 无：用配置结构体参数
来源：http://ncx.hongshengwenyu.top

Ruby: f(a: 1, b: 2)
来源：http://ekq.jinyuanbaomall.cn

C#:   f(a: 1, b: 2)
来源：http://mad.cdnleiting.top

[C05] 返回多个值
来源：http://our.yj20258.top

Py:   return a, b
来源：http://cge.chenzaomai.com

PHP:  return [$a, $b];
来源：http://kmw.cashguo.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kyj.9152youxi.cn

TS:   return { a, b };
来源：http://rju.jinqigufen.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mtx.aizwys.cn

Go:   return a, b
来源：http://ejq.sxryk.cn

Ruby: return a, b
来源：http://lww.shzxlz.cn

C#:   return (a, b);              // ValueTuple
来源：http://gxa.cheryme.top

[C06] 匿名函数 / lambda
来源：http://klb.ppjwa.cn

Py:   square = lambda x: x * x
来源：http://qjs.epnwcf.com

PHP:  $square = fn($x) => $x * $x;
来源：http://bmv.hfpthk.cn

JS:   const square = x => x * x;
来源：http://twf.ydzc1.top

TS:   const square = (x: number): number => x * x;
来源：http://qpr.nanxuanxn.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://stg.zhixingplan.top

Go:   sq := func(x int) int { return x * x }
来源：http://eev.guannengcc.top

Ruby: square = ->(x) { x * x }
来源：http://gwm.yuxming.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gzx.tian-w.cn

[C07] 把函数作为参数传入
来源：http://xnz.hongshengwenyu.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://eoj.hammf.cn

PHP:  array_map("strtoupper", $arr);
来源：http://ojc.uphjek.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nsy.tanke756.top

TS:   arr.map(String)
来源：http://rja.fanxiaobao.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://izf.sysykeji.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://bcc.sufxvd.cn

Ruby: arr.map(&:upcase)
来源：http://jjw.quarkkingdee.top

C#:   arr.Select(s => s.ToUpper())
来源：http://kyd.jqgufenzy.top

[C08] 闭包
来源：http://vtc.xuanzx.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://row.yongpay.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ban.shanyushiyangtech.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://jfd.yuanzhike.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://sqe.jqgfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xwh.fehbvm.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://xav.sweek.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ruo.yuxming.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://pex.jinqigfzy.top

[C09] 递归
来源：http://lpm.hysaishi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://prm.feifeiyinyue.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://szm.zhiwuduotai.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qux.zhiwuduotai.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://peb.wangdashe.top


<!-- 参考信息 -->