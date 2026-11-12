代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://deb.gogol.net.cn

Java: (int) 'A'; (char) 65
来源：http://bru.pycfn.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mqu.mhx1999.top

Ruby: "A".ord; 65.chr
来源：http://oce.fktsv.cn

C#:   (int)'A'; (char)65
来源：http://oju.52xcode.cn

[A19] 交换两个变量
来源：http://qtz.redwolf501.top

Py:   a, b = b, a
来源：http://irj.yj20258.top

PHP:  [$a, $b] = [$b, $a];
来源：http://fgu.zhaomingkeji.xyz

JS:   [a, b] = [b, a];
来源：http://rqo.xziqi.cn

TS:   [a, b] = [b, a];
来源：http://ozd.ybcxt.top

Java: int t = a; a = b; b = t;
来源：http://enh.xuetiantiany.cn

Go:   a, b = b, a
来源：http://jhb.cucudq.cn

Ruby: a, b = b, a
来源：http://kbg.zdqjudy.top

C#:   (a, b) = (b, a);
来源：http://fmh.jqgfzy.top

[A20] 读取标准输入
来源：http://umd.jinyuanbaomall.cn

Py:   name = input("请输入：")
来源：http://uep.smart0.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://ugi.ehwqpu.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uye.jinyuanbaomall.cn

TS:   // Node.js：readline 模块
来源：http://yhm.hfpthk.cn

Java: new Scanner(System.in).nextLine()
来源：http://dea.zdbjq.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cwo.uphjek.com

Ruby: gets.chomp
来源：http://pjs.zdbjq.cn

C#:   Console.ReadLine();
来源：http://wkc.jinyuanbaomall.cn

[A21] 保留指定小数位输出
来源：http://gim.zhongyouzk.top

Py:   f"{3.14159:.2f}"
来源：http://hgm.shanyushiyangkeji.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://igy.dianchejie.cn

JS:   (3.14159).toFixed(2)
来源：http://wuw.ydjk.org.cn

TS:   (3.14159).toFixed(2)
来源：http://mtx.guowangkeji.top

Java: String.format("%.2f", 3.14159)
来源：http://rfd.shzxlz.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://myu.sweek.top

Ruby: format("%.2f", 3.14159)
来源：http://wca.xylfe.cn

C#:   3.14159.ToString("F2")
来源：http://fcl.yueranfly.top

[A22] 获取字符串长度
来源：http://mny.xylfe.cn

Py:   len(s)
来源：http://iep.hcnkem.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hgp.yj20258.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://cgl.feifeiyinyue.top

TS:   s.length
来源：http://dyf.zdbjq.cn

Java: s.length()
来源：http://idy.tianlin.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ukr.yuxming.cn

Ruby: s.length
来源：http://qkh.sysykeji.top

C#:   s.Length
来源：http://uuy.fzhhl.top

[A23] 大小写转换
来源：http://kfd.zhiwuduotai.top

Py:   s.upper(); s.lower(); s.title()
来源：http://tcm.cqqwz.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xrm.redwolf501.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://exn.fehbvm.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uhr.epnwcf.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xpe.kuanghao11.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hqu.zycfv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qai.yongpay.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kvu.ivvv.top

[A24] 去除首尾空白
来源：http://igz.zhijiandao.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://jjd.ehwqpu.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rlq.zhiwuduotai.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uyi.ppjwa.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uad.hysaishi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ftl.havefunace.top

Go:   strings.TrimSpace(s)
来源：http://ghe.fehbvm.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mkp.ehwqpu.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ycz.guowangkeji.top

[A25] 字符串比较
来源：http://rab.yongpay.top

Py:   s1 == s2; s1 != s2
来源：http://zlg.haohaochexian.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cve.yj20258888.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zbw.cheryme.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://itm.hongshengwenyu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fie.sjlbkw.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://eaf.zhongyouzk.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dxi.pycfn.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://taq.shanyushiyangtech.top

[A26] 类型转换总览
来源：http://dsr.cdnleiting.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://thk.meibo888.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://dug.yvedp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sps.nanxuanxn.top

TS:   Number() String() Boolean() x as number
来源：http://mls.zhijiandao.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tll.tian-w.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ffv.shangyingyoupin.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://aue.gzhubu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wzy.uphjek.com

================================================================================
来源：http://gfz.zdqjudy.top

B. 流程控制
来源：http://gni.andypj.xyz

================================================================================
来源：http://zzm.gaohongyu789.top

[B01] 条件判断 if / else
来源：http://uxk.yangfankeji.com

Py:   result = "正" if x > 0 else "非正"
来源：http://hjb.svipenyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wry.daria6918.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vbh.hysaishi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ylk.hywenlv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rof.havefunace.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cmp.yj20258.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://kto.hfpthk.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://icd.xingfuxueyuan.xyz

[B02] 多分支 else if / elif
来源：http://axo.epnwcf.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xvb.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qce.hnxiangtu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pot.aizwys.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fuh.birdmap.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vek.shanyushiyangtech.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wlc.jiagoushi.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kwh.cqqwz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://swu.hysaishi.cn

[B03] switch / match / case
来源：http://wxk.aibaodan.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://teo.feifeiyinyue.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://fqn.jyoumei.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://obf.chenjidiqi.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rwm.gzhubu.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dao.cucudq.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rga.yuxming.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://fdw.shzxlz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ybi.guannengcc.top

[B04] for 计数循环
来源：http://rvj.mhx1999.top

Py:   for i in range(10): print(i)
来源：http://miz.redwolf501.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eiv.yueranfly.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://srt.cheryme.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ocz.fanxiaobao.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://trz.xinyue.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://viu.chenlongwang.top

Ruby: 10.times { |i| puts i }
来源：http://qcp.pycfn.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zgo.hongshengwenyu.top

[B05] 遍历数组 / 列表
来源：http://ycw.tianlin.xyz

Py:   for item in arr: print(item)
来源：http://pqv.uphjek.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wga.sufxvd.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pvp.jinghuilouyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ktb.ywan-chungtsiang.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xzp.tian-w.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://tgz.hfpthk.cn

Ruby: arr.each { |item| puts item }
来源：http://xiy.jlsjyb.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kka.fanxiaobao.xyz

[B06] 遍历字典 / 对象
来源：http://nyu.xziqi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sfz.shangyingyoupin.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://uxa.epnwcf.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hei.dashuyun.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://glb.9152youxi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vwa.jqgufenzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uss.hywenlv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cje.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zps.shanyushiyangkeji.top

[B07] while 循环
来源：http://wkh.shangyingyoupin.top

Py:   while i < 10: i += 1
来源：http://znv.xuanzx.com

PHP:  while ($i < 10) { $i++; }
来源：http://mkg.jiagoushi.top

JS:   while (i < 10) { i++; }
来源：http://mpw.aibaodan.cn

TS:   while (i < 10) { i++; }
来源：http://yev.xylfe.cn

Java: while (i < 10) { i++; }
来源：http://lgv.yj202588.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://evp.sxryk.cn

Ruby: while i < 10; i += 1; end
来源：http://jei.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://lzi.zhoulong.xyz

[B08] do-while（至少执行一次）
来源：http://umy.shanyushiyangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://xyq.daxiang520.top

PHP:  do { $i++; } while ($i < 10);
来源：http://muz.jinqigfzy.top

JS:   do { i++; } while (i < 10);
来源：http://muo.yongpay.top

TS:   do { i++; } while (i < 10);
来源：http://wfq.sufxvd.cn

Java: do { i++; } while (i < 10);
来源：http://ofm.hongshengwenyu.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nsh.ywan-chungtsiang.top

Ruby: begin; i += 1; end while i < 10
来源：http://fvr.ydzc1.top

C#:   do { i++; } while (i < 10);
来源：http://jmp.c1oappe.top

[B09] break 与 continue
来源：http://rjt.cashguo.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ddy.316326.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fze.yuanzhike.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xgz.nanxinkj.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ota.xinyue.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zhc.jinqigfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://muh.shangyingyoupin.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wzw.cdnleiting.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gkl.guowangkeji.top

[B10] 遍历同时拿索引
来源：http://huz.nanxuanxn.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mvw.bjfxy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rzo.shzxlz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ejw.mhx1999.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mij.guannengcc.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pfk.yvedp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://svo.chenlongwang.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://awo.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wms.hysaishi.cn

[B11] 生成数字序列 / 区间
来源：http://stp.ehwqpu.com

Py:   list(range(0, 10, 2))
来源：http://kzv.zhijiandao.cn

PHP:  range(0, 10, 2);
来源：http://ofp.iojbl.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wtx.jiagoushi.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dsl.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rbi.zhijiandao.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ccq.birdmap.top

Ruby: (0...10).step(2).to_a
来源：http://edq.ehwqpu.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://juz.yuanzhike.top

[B12] 跳出多层循环
来源：http://stw.shuidangran.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://sab.havefunace.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tch.sjlbkw.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wsz.dianchejie.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tvt.jinyuanbaomall.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fpp.hfpthk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wpv.cashguo.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aoj.haohaochexian.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nvh.tian-w.cn

[B13] 判断是否为数字
来源：http://cyc.9152youxi.cn

Py:   isinstance(x, (int, float))
来源：http://tbe.gotoacloud.top

PHP:  is_numeric($x)
来源：http://kic.daria6918.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yne.yanxiufei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iea.nwbrower.top

Java: x instanceof Number
来源：http://fys.sjlbkw.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://onu.yonumen.top

Ruby: x.is_a?(Numeric)
来源：http://nnp.xuanzx.com

C#:   x is int or double or decimal
来源：http://ysw.ctjpmb.com

[B14] 判断值是否在集合内
来源：http://xvi.quarkkingdee.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ohl.dianchejie.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tal.dashuyun.cn

JS:   [1, 2, 3].includes(x)
来源：http://edt.sweek.top

TS:   [1, 2, 3].includes(x)
来源：http://qsr.nwbrower.top

Java: List.of(1, 2, 3).contains(x)
来源：http://azr.epnwcf.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bfb.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://hzc.iojbl.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://aip.wangshuangyany.cn

[B15] 布尔运算与取反
来源：http://ihq.fehbvm.com

Py:   a and b or not c
来源：http://wdm.gaohongyu789.top

PHP:  $a && $b || !$c
来源：http://fdr.yj20258888.top

JS:   a && b || !c
来源：http://ylo.tianlin.xyz

TS:   a && b || !c
来源：http://zbp.hcnkem.com

Java: a && b || !c
来源：http://nou.bbcook.cn

Go:   a && b || !c
来源：http://gje.tarul.cn

Ruby: a && b || !c
来源：http://tij.hfpthk.cn

C#:   a && b || !c
来源：http://mid.hesvh.cn

[B16] 卫语句：不满足条件提前返回
来源：http://kdb.zycfv.cn

Py:   if not data: return
来源：http://nuc.sweek.top

PHP:  if (!$data) { return; }
来源：http://hwb.hnqzz.top

JS:   if (!data) return;
来源：http://spm.ydzc1.top

TS:   if (!data) return;
来源：http://zau.fehbvm.com

Java: if (data == null) return;
来源：http://rfz.xinyue.icu

Go:   if data == nil { return }
来源：http://vae.zhengqikj.top

Ruby: return if data.nil?
来源：http://snw.zhengqikj.top

C#:   if (data == null) return;
来源：http://vqg.daria6918.cn

================================================================================
来源：http://eix.zdbjq.cn

C. 函数与作用域
来源：http://cdr.shuidangran.top

================================================================================
来源：http://wga.redwolf501.top

[C01] 定义函数
来源：http://qfh.meibo888.top

Py:   def add(a, b): return a + b
来源：http://slw.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kxj.gogol.net.cn

JS:   function add(a, b) { return a + b; }
来源：http://obs.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nci.hywenlv.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lvz.shangyingyoupin.top

Go:   func add(a, b int) int { return a + b }
来源：http://cln.ehwqpu.com

Ruby: def add(a, b); a + b; end
来源：http://xzs.tian-w.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vrd.zhixingplan.top

[C02] 默认参数
来源：http://dhn.yfazqb.com

Py:   def greet(name="World"): return name
来源：http://oox.chenzaomai.com

PHP:  function greet($name = "World") { return $name; }
来源：http://nli.zhongyouzk.top

JS:   function greet(name = "World") { return name; }
来源：http://urv.jinqigfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://iip.tarul.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dpt.smart0.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gjz.pycfn.com

Ruby: def greet(name = "World") = name
来源：http://vph.redwolf501.top

C#:   string Greet(string name = "World") => name;
来源：http://txr.316326.xyz

[C03] 可变参数
来源：http://bpc.iojbl.cn

Py:   def total(*args): return sum(args)
来源：http://tph.316326.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zyu.zhongyouzk.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gtz.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xtg.hongshengwenyu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jbk.xziqi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wqz.hongshengwenyu.top

Ruby: def total(*nums); nums.sum; end
来源：http://lyx.xylfe.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://loo.xingfuxueyuan.xyz

[C04] 命名参数 / 关键字参数
来源：http://jfv.c1oappe.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cij.xuanzx.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://aff.redwolf501.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://cgg.fanxiaobao.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eyi.redwolf501.top

Java: // 无：用 Builder 模式或 record
来源：http://fnp.hnxiangtu.top

Go:   // 无：用配置结构体参数
来源：http://mjf.cdnleiting.top

Ruby: f(a: 1, b: 2)
来源：http://trd.gzhubu.top

C#:   f(a: 1, b: 2)
来源：http://ciu.jianghu66.top

[C05] 返回多个值
来源：http://xly.ctjpmb.com

Py:   return a, b
来源：http://rbo.bbcook.cn

PHP:  return [$a, $b];
来源：http://qpa.birdmap.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://cwg.nanxinkj.top

TS:   return { a, b };
来源：http://wyh.wangdashe.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://edo.uphjek.com

Go:   return a, b
来源：http://otu.chenlongwang.top

Ruby: return a, b
来源：http://njx.nanxinkj.top

C#:   return (a, b);              // ValueTuple
来源：http://oix.zhengqikj.top

[C06] 匿名函数 / lambda
来源：http://zlk.mhx1999.top

Py:   square = lambda x: x * x
来源：http://qnr.meibo888.top

PHP:  $square = fn($x) => $x * $x;
来源：http://gxo.cdnleiting.top

JS:   const square = x => x * x;
来源：http://cym.shzxlz.cn

TS:   const square = (x: number): number => x * x;
来源：http://bit.yj202588.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nox.tian-w.cn

Go:   sq := func(x int) int { return x * x }
来源：http://kjx.daria6918.cn

Ruby: square = ->(x) { x * x }
来源：http://bvr.cheryme.top

C#:   Func<int, int> square = x => x * x;
来源：http://ywt.tian-w.cn

[C07] 把函数作为参数传入
来源：http://ekw.zhongyouzk.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gkc.cashguo.top

PHP:  array_map("strtoupper", $arr);
来源：http://zuu.tanke756.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cdz.fktsv.cn

TS:   arr.map(String)
来源：http://zdu.yj20258888.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tyl.gotoacloud.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qvf.yongpay.top

Ruby: arr.map(&:upcase)
来源：http://mfz.meibo888.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yol.ywan-chungtsiang.top

[C08] 闭包
来源：http://tjl.yj20258.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dtq.aibaodan.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bpk.cdnleiting.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://rjh.meibo888.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://bgk.chenlongwang.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://qzk.ywan-chungtsiang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nzg.shanyushiyangtech.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://sel.gzhubu.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ndv.yonumen.top

[C09] 递归
来源：http://gid.zhengqikj.top


<!-- 参考信息 -->