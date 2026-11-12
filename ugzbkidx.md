代发 wailian999

JS:   [a, b] = [b, a];
来源：http://vom.sysykeji.top

TS:   [a, b] = [b, a];
来源：http://abu.yj20258888.top

Java: int t = a; a = b; b = t;
来源：http://bek.chenlongwang.top

Go:   a, b = b, a
来源：http://vvu.tianlin.xyz

Ruby: a, b = b, a
来源：http://yuc.shanyushiyangtech.top

C#:   (a, b) = (b, a);
来源：http://muo.hesvh.cn

[A20] 读取标准输入
来源：http://ykf.nwbrower.top

Py:   name = input("请输入：")
来源：http://mtk.vehdjk.com

PHP:  $name = trim(fgets(STDIN));
来源：http://ocj.0kj1m.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kdb.meibo888.top

TS:   // Node.js：readline 模块
来源：http://kpg.iojbl.cn

Java: new Scanner(System.in).nextLine()
来源：http://ncx.nanxinkj.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uex.fktsv.cn

Ruby: gets.chomp
来源：http://soa.yangfankeji.com

C#:   Console.ReadLine();
来源：http://wqt.aibaodan.cn

[A21] 保留指定小数位输出
来源：http://uiv.52xcode.cn

Py:   f"{3.14159:.2f}"
来源：http://vbk.xylfe.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gxb.yongpay.top

JS:   (3.14159).toFixed(2)
来源：http://fbm.vqdsnc.cn

TS:   (3.14159).toFixed(2)
来源：http://uby.dianchejie.cn

Java: String.format("%.2f", 3.14159)
来源：http://vbp.yj20258.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vup.zhixingplan.top

Ruby: format("%.2f", 3.14159)
来源：http://mwa.kuanghao11.cn

C#:   3.14159.ToString("F2")
来源：http://vre.cucudq.cn

[A22] 获取字符串长度
来源：http://lmn.gogol.net.cn

Py:   len(s)
来源：http://diq.feifeiyinyue.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dof.xziqi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://htb.fehbvm.com

TS:   s.length
来源：http://mgl.shzxlz.cn

Java: s.length()
来源：http://alt.dianchejie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rsh.shuidangran.top

Ruby: s.length
来源：http://rud.yuxming.cn

C#:   s.Length
来源：http://pxy.jianghu66.top

[A23] 大小写转换
来源：http://gck.iojbl.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://bzr.daria6918.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hcu.52xcode.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wds.yueranfly.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hwa.feifeiyinyue.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://smp.gaohongyu789.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gjx.xylfe.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gtk.hcnkem.com

C#:   s.ToUpper(); s.ToLower()
来源：http://tqi.hongshengwenyu.top

[A24] 去除首尾空白
来源：http://hgc.nwbrower.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://kbm.yanxiufei.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://met.pengpengdd.cyou

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ghf.xziqi.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fgr.chenjidiqi.icu

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ibt.tarul.cn

Go:   strings.TrimSpace(s)
来源：http://cbt.daria6918.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dcz.vehdjk.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://swf.xinyue.icu

[A25] 字符串比较
来源：http://bnv.uphjek.com

Py:   s1 == s2; s1 != s2
来源：http://ofs.yuanzhike.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://isi.yj202588.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://key.316326.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tjn.vehdjk.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ujw.havefunace.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://aet.hfpthk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uhb.hfpthk.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://pse.yueranfly.top

[A26] 类型转换总览
来源：http://sbw.316326.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://muc.hnqzz.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ndz.gogol.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qwp.zhaomingkeji.xyz

TS:   Number() String() Boolean() x as number
来源：http://jxy.hcnkem.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ckb.guowangkeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jvl.aizwys.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nft.jyoumei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zfm.jinyuanbaomall.cn

================================================================================
来源：http://thb.yj202588.top

B. 流程控制
来源：http://etm.uphjek.com

================================================================================
来源：http://bmp.xuetiantiany.cn

[B01] 条件判断 if / else
来源：http://mvr.aizwys.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://rwl.yj20258.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://gcz.zhixingplan.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://uza.zhengqikj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ktq.nanxuanxn.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ksh.yvedp.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wpz.jinyuanbaomall.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xbv.ywan-chungtsiang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xja.guannengcc.top

[B02] 多分支 else if / elif
来源：http://rem.yj202588.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rbm.meibo888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tzh.yj202588.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://afm.hcnkem.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://buk.yanxiufei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xxs.shanyushiyangtech.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tkm.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qzn.cheryme.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pjx.sjlbkw.cn

[B03] switch / match / case
来源：http://sww.havefunace.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fbc.svipenyu.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qnq.sweek.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://drv.aibaodan.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://thv.xuetiantiany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nir.jinghuilouyu.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://iak.zhoulong.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nqa.cqqwz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://osw.gogol.net.cn

[B04] for 计数循环
来源：http://xqj.yuxming.cn

Py:   for i in range(10): print(i)
来源：http://aol.cucudq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rug.gotoacloud.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vlr.fanxiaobao.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://okb.chenzaomai.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ksn.ppjwa.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zoj.c1oappe.top

Ruby: 10.times { |i| puts i }
来源：http://thp.hammf.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nfs.yj20258888.top

[B05] 遍历数组 / 列表
来源：http://kdw.hongshengwenyu.top

Py:   for item in arr: print(item)
来源：http://jdb.zhijiandao.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xma.shangyingyoupin.top

JS:   for (const item of arr) { console.log(item); }
来源：http://mgl.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://lxz.shuidangran.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ais.wangdashe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qhi.cucudq.cn

Ruby: arr.each { |item| puts item }
来源：http://goe.guowangkeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zct.shuidangran.top

[B06] 遍历字典 / 对象
来源：http://ovu.cashguo.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kbq.xingfuxueyuan.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xyo.hammf.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mmr.daria6918.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jiq.yanxiufei.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rxk.uphjek.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jfw.smart0.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jaq.uphjek.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://egn.yonumen.top

[B07] while 循环
来源：http://biw.hammf.cn

Py:   while i < 10: i += 1
来源：http://pix.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fof.zhaomingkeji.xyz

JS:   while (i < 10) { i++; }
来源：http://pek.bjfxy.top

TS:   while (i < 10) { i++; }
来源：http://itj.zhiwuduotai.top

Java: while (i < 10) { i++; }
来源：http://sbc.hfpthk.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://glk.ehwqpu.com

Ruby: while i < 10; i += 1; end
来源：http://mgf.xziqi.cn

C#:   while (i < 10) { i++; }
来源：http://lmt.hfpthk.cn

[B08] do-while（至少执行一次）
来源：http://hfs.0kj1m.cn

Py:   # 无 do-while：用 while True + break
来源：http://bvl.shzxlz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ows.yuxming.cn

JS:   do { i++; } while (i < 10);
来源：http://zwe.yuanzhike.top

TS:   do { i++; } while (i < 10);
来源：http://rpi.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://yba.ydzc1.top

Go:   for { i++; if i >= 10 { break } }
来源：http://yxo.yuxming.cn

Ruby: begin; i += 1; end while i < 10
来源：http://fyh.ppjwa.cn

C#:   do { i++; } while (i < 10);
来源：http://qxk.ivvv.top

[B09] break 与 continue
来源：http://mch.pycfn.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zzj.zdqjudy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://obu.daxiang520.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cnl.jyoumei.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bcb.aizwys.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xpi.ybcxt.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qkl.yongpay.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://owa.sufxvd.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ncw.ywan-chungtsiang.top

[B10] 遍历同时拿索引
来源：http://jxf.jiagoushi.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eoi.dianchejie.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lov.shuidangran.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://twl.pengpengdd.cyou

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ggt.zhiwuduotai.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cje.9152youxi.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aju.wangshuangyany.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kau.cdnleiting.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gol.tanke756.top

[B11] 生成数字序列 / 区间
来源：http://uwv.yanxiufei.cn

Py:   list(range(0, 10, 2))
来源：http://mpq.ctjpmb.com

PHP:  range(0, 10, 2);
来源：http://nop.hnxiangtu.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yip.jiagoushi.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zgj.hfpthk.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wgt.cheryme.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://swh.zhengqikj.top

Ruby: (0...10).step(2).to_a
来源：http://crf.zhaomingkeji.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nuv.sweek.top

[B12] 跳出多层循环
来源：http://wvo.tian-w.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://rce.chenlongwang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://sle.hesvh.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rqd.jinqigfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fwm.tanke756.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xeg.hcnkem.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yrw.birdmap.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tjm.zhijiandao.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uhs.jlsjyb.cn

[B13] 判断是否为数字
来源：http://yod.pycfn.com

Py:   isinstance(x, (int, float))
来源：http://wyu.hfpthk.cn

PHP:  is_numeric($x)
来源：http://yus.shuidangran.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://okc.uphjek.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ywc.tanke756.top

Java: x instanceof Number
来源：http://dtc.haohaochexian.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vnd.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://zyv.guannengcc.top

C#:   x is int or double or decimal
来源：http://eok.cucudq.cn

[B14] 判断值是否在集合内
来源：http://mqx.zdqjudy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vbj.sxryk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://eoa.ybcxt.top

JS:   [1, 2, 3].includes(x)
来源：http://ups.nanxinkj.top

TS:   [1, 2, 3].includes(x)
来源：http://oad.hcnkem.com

Java: List.of(1, 2, 3).contains(x)
来源：http://ghc.gotoacloud.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lke.yuxming.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ykl.wangdashe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qnf.gaohongyu789.top

[B15] 布尔运算与取反
来源：http://kqc.xuetiantiany.cn

Py:   a and b or not c
来源：http://giv.gogol.net.cn

PHP:  $a && $b || !$c
来源：http://pwn.havefunace.top

JS:   a && b || !c
来源：http://ijo.daxiang520.top

TS:   a && b || !c
来源：http://dyw.ybcxt.top

Java: a && b || !c
来源：http://snu.yj20258.top

Go:   a && b || !c
来源：http://dqs.zhixingplan.top

Ruby: a && b || !c
来源：http://zjp.tanke756.top

C#:   a && b || !c
来源：http://kyr.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://rkk.gogol.net.cn

Py:   if not data: return
来源：http://gsd.sweek.top

PHP:  if (!$data) { return; }
来源：http://ajw.hysaishi.cn

JS:   if (!data) return;
来源：http://apx.shzxlz.cn

TS:   if (!data) return;
来源：http://zeo.redwolf501.top

Java: if (data == null) return;
来源：http://ltu.xingfuxueyuan.xyz

Go:   if data == nil { return }
来源：http://wkc.zhoulong.xyz

Ruby: return if data.nil?
来源：http://owf.haohaochexian.top

C#:   if (data == null) return;
来源：http://vkn.yanxiufei.cn

================================================================================
来源：http://dfe.birdmap.top

C. 函数与作用域
来源：http://jen.jlsjyb.cn

================================================================================
来源：http://rwg.sjlbkw.cn

[C01] 定义函数
来源：http://mvs.yonumen.top

Py:   def add(a, b): return a + b
来源：http://oxf.shanyushiyangkeji.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://myy.nanxuanxn.top

JS:   function add(a, b) { return a + b; }
来源：http://erz.haohaochexian.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nvt.pengpengdd.cyou

Java: static int add(int a, int b) { return a + b; }
来源：http://pxo.aibaodan.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dox.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://hvr.316326.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://kpo.ydjk.org.cn

[C02] 默认参数
来源：http://zwh.9152youxi.cn

Py:   def greet(name="World"): return name
来源：http://tmu.gaohongyu789.top

PHP:  function greet($name = "World") { return $name; }
来源：http://csv.jinyuanbaomall.cn

JS:   function greet(name = "World") { return name; }
来源：http://nrk.hnqzz.top

TS:   function greet(name: string = "World") { return name; }
来源：http://fws.shzxlz.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://iwp.vqdsnc.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://adt.jyoumei.cn

Ruby: def greet(name = "World") = name
来源：http://jwl.shanyushiyangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://iqd.xuanzx.com

[C03] 可变参数
来源：http://ycw.gzhubu.top

Py:   def total(*args): return sum(args)
来源：http://vdu.gaohongyu789.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wyo.sxryk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oqw.haohaochexian.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://upz.guannengcc.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ium.epnwcf.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gxu.bbcook.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hxb.hongshengwenyu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kui.hfpthk.cn

[C04] 命名参数 / 关键字参数
来源：http://cja.fzhhl.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qam.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iiz.yongpay.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uma.chenzaomai.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zrg.cheryme.top

Java: // 无：用 Builder 模式或 record
来源：http://egm.yvedp.cn

Go:   // 无：用配置结构体参数
来源：http://mjv.gaohongyu789.top

Ruby: f(a: 1, b: 2)
来源：http://pfw.mhx1999.top

C#:   f(a: 1, b: 2)
来源：http://vrn.9152youxi.cn

[C05] 返回多个值
来源：http://lpi.ydzc1.top

Py:   return a, b
来源：http://fvv.iojbl.cn

PHP:  return [$a, $b];
来源：http://ewb.uphjek.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://urc.sysykeji.top

TS:   return { a, b };
来源：http://shd.mhx1999.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://awc.daria6918.cn

Go:   return a, b
来源：http://oud.tianlin.xyz

Ruby: return a, b
来源：http://pld.wangdashe.top

C#:   return (a, b);              // ValueTuple
来源：http://rvn.xylfe.cn

[C06] 匿名函数 / lambda
来源：http://gus.vqdsnc.cn

Py:   square = lambda x: x * x
来源：http://ryi.jianghu66.top

PHP:  $square = fn($x) => $x * $x;
来源：http://okn.shanyushiyangtech.top

JS:   const square = x => x * x;
来源：http://xgt.birdmap.top

TS:   const square = (x: number): number => x * x;
来源：http://anq.bjfxy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xmo.wangshuangyany.cn

Go:   sq := func(x int) int { return x * x }
来源：http://hel.haohaochexian.top

Ruby: square = ->(x) { x * x }
来源：http://qsj.ydzc1.top

C#:   Func<int, int> square = x => x * x;
来源：http://vjh.andypj.xyz

[C07] 把函数作为参数传入
来源：http://veb.jlsjyb.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vtt.jinqigfzy.top

PHP:  array_map("strtoupper", $arr);
来源：http://zaa.xinyue.icu

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dpl.bbcook.cn

TS:   arr.map(String)
来源：http://tpg.chenlongwang.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vty.tarul.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ukf.mhx1999.top

Ruby: arr.map(&:upcase)
来源：http://dhg.xingfuxueyuan.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://ezc.tian-w.cn

[C08] 闭包
来源：http://blk.sjlbkw.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://jlf.meibo888.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://rlo.svipenyu.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://cnb.fzhhl.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kpx.zdqjudy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ini.tanke756.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jty.fktsv.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yaf.birdmap.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cby.cucudq.cn

[C09] 递归
来源：http://mme.ivvv.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ahf.shanyushiyangtech.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://vjt.xuetiantiany.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://iuf.ppjwa.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ggr.aibaodan.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lzw.aizwys.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kzf.chenjidiqi.icu

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mtj.shuidangran.top

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://pqt.sjlbkw.cn


<!-- 参考信息 -->