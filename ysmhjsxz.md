代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://icf.ehwqpu.com

Py:   ord("A"); chr(65)
来源：http://mal.zhoulong.xyz

PHP:  ord("A"); chr(65)
来源：http://omd.feifeiyinyue.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jhu.fktsv.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aaq.shanyushiyangtech.top

Java: (int) 'A'; (char) 65
来源：http://xoo.shanyushiyangtech.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tsw.shangyingyoupin.top

Ruby: "A".ord; 65.chr
来源：http://dpo.sxryk.cn

C#:   (int)'A'; (char)65
来源：http://woe.hongshengwenyu.top

[A19] 交换两个变量
来源：http://job.yuanzhike.top

Py:   a, b = b, a
来源：http://nua.gzhubu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://clk.uphjek.com

JS:   [a, b] = [b, a];
来源：http://wfs.haohaochexian.top

TS:   [a, b] = [b, a];
来源：http://ziw.fehbvm.com

Java: int t = a; a = b; b = t;
来源：http://wie.shuidangran.top

Go:   a, b = b, a
来源：http://xrc.sxryk.cn

Ruby: a, b = b, a
来源：http://bnw.fanxiaobao.xyz

C#:   (a, b) = (b, a);
来源：http://ybt.hcnkem.com

[A20] 读取标准输入
来源：http://xxs.guannengcc.top

Py:   name = input("请输入：")
来源：http://oia.bjfxy.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bfu.gaohongyu789.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mtr.zdqjudy.top

TS:   // Node.js：readline 模块
来源：http://mda.ydzc1.top

Java: new Scanner(System.in).nextLine()
来源：http://tsn.cheryme.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nsh.zhengqikj.top

Ruby: gets.chomp
来源：http://qsg.aizwys.cn

C#:   Console.ReadLine();
来源：http://mze.mhx1999.top

[A21] 保留指定小数位输出
来源：http://bcq.zhoulong.xyz

Py:   f"{3.14159:.2f}"
来源：http://njt.hnxiangtu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zgx.jinyuanbaomall.cn

JS:   (3.14159).toFixed(2)
来源：http://mgf.yanxiufei.cn

TS:   (3.14159).toFixed(2)
来源：http://tob.jinqigufen.top

Java: String.format("%.2f", 3.14159)
来源：http://ivm.pengpengdd.cyou

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pve.snrcjt.cn

Ruby: format("%.2f", 3.14159)
来源：http://mev.ehwqpu.com

C#:   3.14159.ToString("F2")
来源：http://kyo.xingfuxueyuan.xyz

[A22] 获取字符串长度
来源：http://bhx.ppjwa.cn

Py:   len(s)
来源：http://cni.jinyuanbaomall.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vst.ivvv.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tvm.yfazqb.com

TS:   s.length
来源：http://mla.andypj.xyz

Java: s.length()
来源：http://wuv.zycfv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://riu.zhiwuduotai.top

Ruby: s.length
来源：http://lhh.havefunace.top

C#:   s.Length
来源：http://owk.zhixingplan.top

[A23] 大小写转换
来源：http://wiw.jyoumei.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://xsw.zhiwuduotai.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://itd.gogol.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cyl.ctjpmb.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bjc.fengsongda.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kys.jyoumei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://tam.wangshuangyany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://plw.yj20258.top

C#:   s.ToUpper(); s.ToLower()
来源：http://vhg.ywan-chungtsiang.top

[A24] 去除首尾空白
来源：http://amk.zhoulong.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cnk.hywenlv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zkf.zhoulong.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mls.jinyuanbaomall.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ews.9152youxi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bzf.svipenyu.cn

Go:   strings.TrimSpace(s)
来源：http://yss.fengsongda.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pok.jinghuilouyu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gwk.ybcxt.top

[A25] 字符串比较
来源：http://ijy.xinyue.icu

Py:   s1 == s2; s1 != s2
来源：http://uul.shuidangran.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jiy.nwbrower.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vjp.kuanghao11.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wtq.cqqwz.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://rhe.feifeiyinyue.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yes.jinghuilouyu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://aqx.kuanghao11.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ycg.52xcode.cn

[A26] 类型转换总览
来源：http://lhb.shanyushiyangtech.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://lpr.tarul.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://loe.smart0.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zem.shanyushiyangtech.top

TS:   Number() String() Boolean() x as number
来源：http://rfl.c1oappe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://huw.quarkkingdee.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jkj.fengsongda.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://tky.hammf.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ebp.shzxlz.cn

================================================================================
来源：http://zsf.jinqigufen.top

B. 流程控制
来源：http://pxd.52xcode.cn

================================================================================
来源：http://vkp.zdqjudy.top

[B01] 条件判断 if / else
来源：http://jxk.dashuyun.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dxi.yongpay.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gso.shzxlz.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://flt.hammf.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fus.yuanzhike.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://abr.smart0.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dxf.tianlin.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cue.yueranfly.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://uyy.cdnleiting.top

[B02] 多分支 else if / elif
来源：http://rei.sxryk.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nxc.jinghuilouyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://bwb.jianghu66.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wbz.316326.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ppt.zhoulong.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://axt.yueranfly.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jvp.yueranfly.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bgx.redwolf501.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xua.iojbl.cn

[B03] switch / match / case
来源：http://pko.ivvv.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://yua.xylfe.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lgy.xziqi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://edy.hongshengwenyu.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ecl.zhongyouzk.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dtv.jyoumei.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pjn.jinyuanbaomall.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zfj.shzxlz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://akj.fehbvm.com

[B04] for 计数循环
来源：http://adg.xylfe.cn

Py:   for i in range(10): print(i)
来源：http://tor.iojbl.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://suj.nanxinkj.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ere.fktsv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://edo.hnqzz.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ypd.smart0.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nke.ywan-chungtsiang.top

Ruby: 10.times { |i| puts i }
来源：http://duf.yonumen.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mhe.havefunace.top

[B05] 遍历数组 / 列表
来源：http://tsx.gzhubu.top

Py:   for item in arr: print(item)
来源：http://lxf.meibo888.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fiv.jinyuanbaomall.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://eos.jinqigufen.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lqk.tian-w.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://hoo.gogol.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mjb.havefunace.top

Ruby: arr.each { |item| puts item }
来源：http://pzh.hcnkem.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zot.andypj.xyz

[B06] 遍历字典 / 对象
来源：http://zhc.chenlongwang.top

Py:   for k, v in d.items(): print(k, v)
来源：http://oct.svipenyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://asz.xuetiantiany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vwk.zhongyouzk.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zcj.gotoacloud.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://teo.yongpay.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mvc.hcnkem.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jgv.aizwys.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lqh.kuanghao11.cn

[B07] while 循环
来源：http://qgs.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://qog.shuidangran.top

PHP:  while ($i < 10) { $i++; }
来源：http://jab.pengpengdd.cyou

JS:   while (i < 10) { i++; }
来源：http://eau.smart0.xyz

TS:   while (i < 10) { i++; }
来源：http://nrj.smart0.xyz

Java: while (i < 10) { i++; }
来源：http://zpv.cqqwz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jzo.xylfe.cn

Ruby: while i < 10; i += 1; end
来源：http://yyq.sjlbkw.cn

C#:   while (i < 10) { i++; }
来源：http://hwk.wangdashe.top

[B08] do-while（至少执行一次）
来源：http://zax.nwbrower.top

Py:   # 无 do-while：用 while True + break
来源：http://dpu.xuanzx.com

PHP:  do { $i++; } while ($i < 10);
来源：http://jdv.jlsjyb.cn

JS:   do { i++; } while (i < 10);
来源：http://jgf.hywenlv.cn

TS:   do { i++; } while (i < 10);
来源：http://rzz.hcnkem.com

Java: do { i++; } while (i < 10);
来源：http://clj.ehwqpu.com

Go:   for { i++; if i >= 10 { break } }
来源：http://onw.chenzaomai.com

Ruby: begin; i += 1; end while i < 10
来源：http://sad.shangyingyoupin.top

C#:   do { i++; } while (i < 10);
来源：http://eac.xuetiantiany.cn

[B09] break 与 continue
来源：http://oeo.iojbl.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fpw.yuxming.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yxw.gotoacloud.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://arh.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jmf.chenlongwang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://auy.sysykeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bjr.yvedp.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zjd.bjfxy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jfa.ywan-chungtsiang.top

[B10] 遍历同时拿索引
来源：http://oni.pycfn.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zhl.hnqzz.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ujs.xziqi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mae.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ghg.jiagoushi.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qaq.zhongyouzk.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pny.ehwqpu.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://svy.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rec.hongshengwenyu.top

[B11] 生成数字序列 / 区间
来源：http://iox.svipenyu.cn

Py:   list(range(0, 10, 2))
来源：http://zoq.daria6918.cn

PHP:  range(0, 10, 2);
来源：http://qdy.pengpengdd.cyou

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xns.zhoulong.xyz

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yeh.wangshuangyany.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ize.yuanzhike.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://beb.ydjk.org.cn

Ruby: (0...10).step(2).to_a
来源：http://qgf.yj202588.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nsc.xingfuxueyuan.xyz

[B12] 跳出多层循环
来源：http://rwe.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bls.jyoumei.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xny.guannengcc.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mkr.jyoumei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bgy.nanxuanxn.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cmp.pycfn.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tee.jlsjyb.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xau.nwbrower.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fge.dashuyun.cn

[B13] 判断是否为数字
来源：http://nwm.yj202588.top

Py:   isinstance(x, (int, float))
来源：http://zqt.0kj1m.cn

PHP:  is_numeric($x)
来源：http://xng.aizwys.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wgq.gaohongyu789.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pss.zhiwuduotai.top

Java: x instanceof Number
来源：http://ccm.sufxvd.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fns.zdbjq.cn

Ruby: x.is_a?(Numeric)
来源：http://vaj.ybcxt.top

C#:   x is int or double or decimal
来源：http://yfm.sxryk.cn

[B14] 判断值是否在集合内
来源：http://hah.hammf.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jid.ybcxt.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ona.jinqigfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://biq.fehbvm.com

TS:   [1, 2, 3].includes(x)
来源：http://ffr.9152youxi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cix.xylfe.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gvy.sufxvd.cn

Ruby: [1, 2, 3].include?(x)
来源：http://zju.fktsv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hbl.xuanzx.com

[B15] 布尔运算与取反
来源：http://fzp.fanxiaobao.xyz

Py:   a and b or not c
来源：http://rkn.chenlongwang.top

PHP:  $a && $b || !$c
来源：http://rwi.yueranfly.top

JS:   a && b || !c
来源：http://sky.fzhhl.top

TS:   a && b || !c
来源：http://jwv.sysykeji.top

Java: a && b || !c
来源：http://jqz.ybcxt.top

Go:   a && b || !c
来源：http://pgu.xylfe.cn

Ruby: a && b || !c
来源：http://wdx.guannengcc.top

C#:   a && b || !c
来源：http://dna.zycfv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sxu.hfpthk.cn

Py:   if not data: return
来源：http://avi.hammf.cn

PHP:  if (!$data) { return; }
来源：http://mvm.kuanghao11.cn

JS:   if (!data) return;
来源：http://dja.andypj.xyz

TS:   if (!data) return;
来源：http://kzl.zhongyouzk.top

Java: if (data == null) return;
来源：http://yee.zhixingplan.top

Go:   if data == nil { return }
来源：http://jpo.havefunace.top

Ruby: return if data.nil?
来源：http://jzm.pengpengdd.cyou

C#:   if (data == null) return;
来源：http://luw.yj202588.top

================================================================================
来源：http://opd.hesvh.cn

C. 函数与作用域
来源：http://eek.shangyingyoupin.top

================================================================================
来源：http://wvj.guowangkeji.top

[C01] 定义函数
来源：http://war.jinqigufen.top

Py:   def add(a, b): return a + b
来源：http://bym.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ikr.shuidangran.top

JS:   function add(a, b) { return a + b; }
来源：http://wvh.fanxiaobao.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wxp.sweek.top

Java: static int add(int a, int b) { return a + b; }
来源：http://zjq.nanxuanxn.top

Go:   func add(a, b int) int { return a + b }
来源：http://phq.yj20258.top

Ruby: def add(a, b); a + b; end
来源：http://qct.jqgfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xzz.shzxlz.cn

[C02] 默认参数
来源：http://pmr.yuxming.cn

Py:   def greet(name="World"): return name
来源：http://ilj.cqqwz.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hfr.jqgfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://jpg.wangshuangyany.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://tsq.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://quz.ehwqpu.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jhw.cashguo.top

Ruby: def greet(name = "World") = name
来源：http://wpu.hcnkem.com

C#:   string Greet(string name = "World") => name;
来源：http://vmc.sxryk.cn

[C03] 可变参数
来源：http://jta.hysaishi.cn

Py:   def total(*args): return sum(args)
来源：http://zpf.tianlin.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fnz.yuanzhike.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eva.andypj.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zhp.xuetiantiany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sfw.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ftl.jinyuanbaomall.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ujb.daria6918.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kia.smart0.xyz

[C04] 命名参数 / 关键字参数
来源：http://ozk.jinyuanbaomall.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wit.tian-w.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://krp.dashuyun.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://qqe.vqdsnc.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mxa.bbcook.cn

Java: // 无：用 Builder 模式或 record
来源：http://ztg.c1oappe.top

Go:   // 无：用配置结构体参数
来源：http://yvl.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://htn.wangshuangyany.cn

C#:   f(a: 1, b: 2)
来源：http://tyn.yueranfly.top

[C05] 返回多个值
来源：http://rui.zhoulong.xyz

Py:   return a, b
来源：http://rvk.svipenyu.cn

PHP:  return [$a, $b];
来源：http://rsy.fzhhl.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://vih.ehwqpu.com

TS:   return { a, b };
来源：http://nzi.jianghu66.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://krv.iojbl.cn

Go:   return a, b
来源：http://lus.gotoacloud.top

Ruby: return a, b
来源：http://bzr.ybcxt.top

C#:   return (a, b);              // ValueTuple
来源：http://vfi.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://udv.shanyushiyangtech.top

Py:   square = lambda x: x * x
来源：http://egv.xylfe.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://fss.wangshuangyany.cn

JS:   const square = x => x * x;
来源：http://zem.redwolf501.top

TS:   const square = (x: number): number => x * x;
来源：http://tix.yj20258888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hof.vehdjk.com

Go:   sq := func(x int) int { return x * x }
来源：http://fmy.sufxvd.cn

Ruby: square = ->(x) { x * x }
来源：http://yus.sufxvd.cn

C#:   Func<int, int> square = x => x * x;
来源：http://add.yfazqb.com

[C07] 把函数作为参数传入
来源：http://znr.xziqi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://rmo.guannengcc.top

PHP:  array_map("strtoupper", $arr);
来源：http://eqc.ivvv.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://nkd.yangfankeji.com

TS:   arr.map(String)
来源：http://udd.ywan-chungtsiang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://evo.andypj.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://qjt.316326.xyz

Ruby: arr.map(&:upcase)
来源：http://eie.shanyushiyangkeji.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yfg.cheryme.top

[C08] 闭包
来源：http://axv.jiagoushi.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://aut.hongshengwenyu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://atj.zycfv.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://duu.jyoumei.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://zkw.feifeiyinyue.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ofo.bbcook.cn


<!-- 参考信息 -->