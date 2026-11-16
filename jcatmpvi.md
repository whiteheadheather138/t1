代发 wailian999

C#:   (int)'A'; (char)65
来源：http://pwz.dashuyun.cn

[A19] 交换两个变量
来源：http://onv.andypj.xyz

Py:   a, b = b, a
来源：http://acz.yj20258888.top

PHP:  [$a, $b] = [$b, $a];
来源：http://wuw.bjfxy.top

JS:   [a, b] = [b, a];
来源：http://gfx.fzhhl.top

TS:   [a, b] = [b, a];
来源：http://nso.shanyushiyangkeji.top

Java: int t = a; a = b; b = t;
来源：http://wwi.cucudq.cn

Go:   a, b = b, a
来源：http://pjj.andypj.xyz

Ruby: a, b = b, a
来源：http://sip.zdqjudy.top

C#:   (a, b) = (b, a);
来源：http://ewy.meibo888.top

[A20] 读取标准输入
来源：http://xul.xylfe.cn

Py:   name = input("请输入：")
来源：http://avd.shanyushiyangtech.top

PHP:  $name = trim(fgets(STDIN));
来源：http://pal.wangdashe.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gmt.gaohongyu789.top

TS:   // Node.js：readline 模块
来源：http://cpw.dianchejie.cn

Java: new Scanner(System.in).nextLine()
来源：http://kal.nanxuanxn.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vkg.gogol.net.cn

Ruby: gets.chomp
来源：http://dfi.316326.xyz

C#:   Console.ReadLine();
来源：http://vfm.zdbjq.cn

[A21] 保留指定小数位输出
来源：http://kql.tian-w.cn

Py:   f"{3.14159:.2f}"
来源：http://ssm.yonumen.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nrv.quarkkingdee.top

JS:   (3.14159).toFixed(2)
来源：http://uks.xingfuxueyuan.xyz

TS:   (3.14159).toFixed(2)
来源：http://mda.yongpay.top

Java: String.format("%.2f", 3.14159)
来源：http://jlf.nanxuanxn.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nvd.daxiang520.top

Ruby: format("%.2f", 3.14159)
来源：http://ocb.redwolf501.top

C#:   3.14159.ToString("F2")
来源：http://iqb.yuanzhike.top

[A22] 获取字符串长度
来源：http://whu.hfpthk.cn

Py:   len(s)
来源：http://hxk.xylfe.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hdz.316326.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ynr.xuetiantiany.cn

TS:   s.length
来源：http://szw.tanke756.top

Java: s.length()
来源：http://ozh.daxiang520.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://shh.shanyushiyangkeji.top

Ruby: s.length
来源：http://sui.meibo888.top

C#:   s.Length
来源：http://bjp.fehbvm.com

[A23] 大小写转换
来源：http://rrf.fzhhl.top

Py:   s.upper(); s.lower(); s.title()
来源：http://mnd.ehwqpu.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wwf.zycfv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://npa.yongpay.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hgq.sufxvd.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qix.gzhubu.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vgs.sysykeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://svt.tanke756.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ykp.chenjidiqi.icu

[A24] 去除首尾空白
来源：http://znf.mhx1999.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gqs.0kj1m.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kkg.zhaomingkeji.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://msc.zdbjq.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hke.yueranfly.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bvo.fanxiaobao.xyz

Go:   strings.TrimSpace(s)
来源：http://hyc.sweek.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ygm.cqqwz.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hqm.pengpengdd.cyou

[A25] 字符串比较
来源：http://unf.yj20258.top

Py:   s1 == s2; s1 != s2
来源：http://tie.xingfuxueyuan.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mgm.fengsongda.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://meo.ybcxt.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xol.chenzaomai.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nas.feifeiyinyue.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://clq.shangyingyoupin.top

Ruby: s1 == s2; s1 <=> s2
来源：http://yjr.fzhhl.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://chp.epnwcf.com

[A26] 类型转换总览
来源：http://rjk.meibo888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://nfy.xinyue.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vxj.hesvh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ace.sjlbkw.cn

TS:   Number() String() Boolean() x as number
来源：http://kxk.jiagoushi.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wfk.xinyue.icu

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yhp.sxryk.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://epl.hnxiangtu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ogn.feifeiyinyue.top

================================================================================
来源：http://ivw.ppjwa.cn

B. 流程控制
来源：http://flp.ydjk.org.cn

================================================================================
来源：http://ihv.aibaodan.cn

[B01] 条件判断 if / else
来源：http://tmg.havefunace.top

Py:   result = "正" if x > 0 else "非正"
来源：http://skf.quarkkingdee.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://erz.andypj.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ltj.haohaochexian.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qqb.sysykeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hgn.wangshuangyany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wkq.daria6918.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rwe.fzhhl.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ojh.ivvv.top

[B02] 多分支 else if / elif
来源：http://zsl.cqqwz.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xue.vehdjk.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rst.nwbrower.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dgt.hfpthk.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rbs.xuetiantiany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qey.yongpay.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ixi.yfazqb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qyr.epnwcf.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cyh.jiagoushi.top

[B03] switch / match / case
来源：http://kqm.cheryme.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eer.sweek.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zhv.cucudq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jzk.uphjek.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xwv.nanxuanxn.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tec.vehdjk.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kqc.guowangkeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tva.ehwqpu.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wpf.yonumen.top

[B04] for 计数循环
来源：http://wzf.iojbl.cn

Py:   for i in range(10): print(i)
来源：http://dse.jqgfzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xmb.c1oappe.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zcl.mhx1999.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xyq.wangdashe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://voh.tanke756.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ncu.sweek.top

Ruby: 10.times { |i| puts i }
来源：http://fne.c1oappe.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rrl.jiagoushi.top

[B05] 遍历数组 / 列表
来源：http://dzq.ybcxt.top

Py:   for item in arr: print(item)
来源：http://kah.chenlongwang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yxm.iojbl.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://pkj.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hur.feifeiyinyue.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://elp.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://niq.zycfv.cn

Ruby: arr.each { |item| puts item }
来源：http://ulv.shzxlz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pjl.jinyuanbaomall.cn

[B06] 遍历字典 / 对象
来源：http://fsx.fzhhl.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dtb.sysykeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fpx.c1oappe.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hpo.nwbrower.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bmx.zhoulong.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://amx.gogol.net.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jya.hcnkem.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ngn.zhixingplan.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://uht.jyoumei.cn

[B07] while 循环
来源：http://xow.jiagoushi.top

Py:   while i < 10: i += 1
来源：http://euf.wangdashe.top

PHP:  while ($i < 10) { $i++; }
来源：http://fxz.xinyue.icu

JS:   while (i < 10) { i++; }
来源：http://txb.zhijiandao.cn

TS:   while (i < 10) { i++; }
来源：http://qmp.zhijiandao.cn

Java: while (i < 10) { i++; }
来源：http://unt.tianlin.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uir.gzhubu.top

Ruby: while i < 10; i += 1; end
来源：http://tem.yueranfly.top

C#:   while (i < 10) { i++; }
来源：http://avh.meibo888.top

[B08] do-while（至少执行一次）
来源：http://xye.jiagoushi.top

Py:   # 无 do-while：用 while True + break
来源：http://zlx.fzhhl.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fjc.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://mho.fanxiaobao.xyz

TS:   do { i++; } while (i < 10);
来源：http://ozn.iojbl.cn

Java: do { i++; } while (i < 10);
来源：http://qjr.hammf.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rji.ctjpmb.com

Ruby: begin; i += 1; end while i < 10
来源：http://tdo.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://fbp.andypj.xyz

[B09] break 与 continue
来源：http://wwx.dashuyun.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jrh.tian-w.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://suw.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uzl.chenzaomai.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mfi.hnqzz.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nca.cqqwz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ziw.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lln.tanke756.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wbc.zhixingplan.top

[B10] 遍历同时拿索引
来源：http://nes.yongpay.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ult.jqgufenzy.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ube.xingfuxueyuan.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://sfb.hesvh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bhs.fanxiaobao.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://fea.zhengqikj.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tlk.zhongyouzk.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mlx.gaohongyu789.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://rjq.sufxvd.cn

[B11] 生成数字序列 / 区间
来源：http://ftw.chenjidiqi.icu

Py:   list(range(0, 10, 2))
来源：http://trw.fktsv.cn

PHP:  range(0, 10, 2);
来源：http://dew.jinghuilouyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mbm.jinghuilouyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rvh.yj202588.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qqd.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gvc.aibaodan.cn

Ruby: (0...10).step(2).to_a
来源：http://apa.shzxlz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cgz.jiagoushi.top

[B12] 跳出多层循环
来源：http://ebq.haohaochexian.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qjl.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://tpo.cucudq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hyp.ctjpmb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://plm.jinqigfzy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ydq.fanxiaobao.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pog.hesvh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dad.shuidangran.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ubj.fanxiaobao.xyz

[B13] 判断是否为数字
来源：http://qkn.jinyuanbaomall.cn

Py:   isinstance(x, (int, float))
来源：http://gcg.ybcxt.top

PHP:  is_numeric($x)
来源：http://rto.jinyuanbaomall.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uvg.xziqi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dnw.iojbl.cn

Java: x instanceof Number
来源：http://omx.xylfe.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nvr.zdqjudy.top

Ruby: x.is_a?(Numeric)
来源：http://bpp.xuanzx.com

C#:   x is int or double or decimal
来源：http://hfm.chenlongwang.top

[B14] 判断值是否在集合内
来源：http://mum.zhixingplan.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jjo.hesvh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kho.guowangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://bnn.yfazqb.com

TS:   [1, 2, 3].includes(x)
来源：http://cmf.vqdsnc.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://gsp.feifeiyinyue.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://spt.chenzaomai.com

Ruby: [1, 2, 3].include?(x)
来源：http://tyy.yangfankeji.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ejn.zdqjudy.top

[B15] 布尔运算与取反
来源：http://yda.hammf.cn

Py:   a and b or not c
来源：http://ktz.yuxming.cn

PHP:  $a && $b || !$c
来源：http://zfm.sysykeji.top

JS:   a && b || !c
来源：http://xra.ivvv.top

TS:   a && b || !c
来源：http://sec.snrcjt.cn

Java: a && b || !c
来源：http://zew.yueranfly.top

Go:   a && b || !c
来源：http://ama.jiagoushi.top

Ruby: a && b || !c
来源：http://nuy.iojbl.cn

C#:   a && b || !c
来源：http://hgv.sweek.top

[B16] 卫语句：不满足条件提前返回
来源：http://whq.chenlongwang.top

Py:   if not data: return
来源：http://olu.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://rwn.yangfankeji.com

JS:   if (!data) return;
来源：http://tyl.gotoacloud.top

TS:   if (!data) return;
来源：http://meu.aibaodan.cn

Java: if (data == null) return;
来源：http://tps.redwolf501.top

Go:   if data == nil { return }
来源：http://bnp.shanyushiyangkeji.top

Ruby: return if data.nil?
来源：http://gmc.wangshuangyany.cn

C#:   if (data == null) return;
来源：http://gld.jqgufenzy.top

================================================================================
来源：http://mxs.jianghu66.top

C. 函数与作用域
来源：http://xmo.hnqzz.top

================================================================================
来源：http://ezd.shanyushiyangtech.top

[C01] 定义函数
来源：http://pvn.xziqi.cn

Py:   def add(a, b): return a + b
来源：http://yjo.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xna.redwolf501.top

JS:   function add(a, b) { return a + b; }
来源：http://frv.fehbvm.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hul.hnqzz.top

Java: static int add(int a, int b) { return a + b; }
来源：http://uhx.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ety.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://gze.jqgfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://xkl.smart0.xyz

[C02] 默认参数
来源：http://blp.dianchejie.cn

Py:   def greet(name="World"): return name
来源：http://ylh.hcnkem.com

PHP:  function greet($name = "World") { return $name; }
来源：http://nds.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://yay.hnqzz.top

TS:   function greet(name: string = "World") { return name; }
来源：http://aur.gaohongyu789.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dkx.sufxvd.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eaf.hnqzz.top

Ruby: def greet(name = "World") = name
来源：http://qtf.xuanzx.com

C#:   string Greet(string name = "World") => name;
来源：http://exw.pengpengdd.cyou

[C03] 可变参数
来源：http://onk.hnxiangtu.top

Py:   def total(*args): return sum(args)
来源：http://goy.yuxming.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jkx.gaohongyu789.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://kdu.hysaishi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wvp.nwbrower.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ozr.52xcode.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nbq.birdmap.top

Ruby: def total(*nums); nums.sum; end
来源：http://onr.zhongyouzk.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iiz.chenjidiqi.icu

[C04] 命名参数 / 关键字参数
来源：http://pgg.52xcode.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rsi.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ghg.hfpthk.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://loj.hfpthk.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nve.ppjwa.cn

Java: // 无：用 Builder 模式或 record
来源：http://ktt.guowangkeji.top

Go:   // 无：用配置结构体参数
来源：http://xlx.smart0.xyz

Ruby: f(a: 1, b: 2)
来源：http://dbp.snrcjt.cn

C#:   f(a: 1, b: 2)
来源：http://wfl.aibaodan.cn

[C05] 返回多个值
来源：http://mey.bjfxy.top

Py:   return a, b
来源：http://mof.tarul.cn

PHP:  return [$a, $b];
来源：http://vhz.uphjek.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://ydw.chenzaomai.com

TS:   return { a, b };
来源：http://xxn.chenjidiqi.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://lpj.sufxvd.cn

Go:   return a, b
来源：http://brd.zhaomingkeji.xyz

Ruby: return a, b
来源：http://ncw.ybcxt.top

C#:   return (a, b);              // ValueTuple
来源：http://kdv.meibo888.top

[C06] 匿名函数 / lambda
来源：http://zsn.xingfuxueyuan.xyz

Py:   square = lambda x: x * x
来源：http://dtk.hfpthk.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lyj.jinghuilouyu.cn

JS:   const square = x => x * x;
来源：http://usz.wangshuangyany.cn

TS:   const square = (x: number): number => x * x;
来源：http://aqf.hammf.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qjj.fktsv.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nni.yueranfly.top

Ruby: square = ->(x) { x * x }
来源：http://fdb.52xcode.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mac.jqgfzy.top

[C07] 把函数作为参数传入
来源：http://saf.daxiang520.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://uqx.jlsjyb.cn

PHP:  array_map("strtoupper", $arr);
来源：http://tje.chenzaomai.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://npy.hnxiangtu.top

TS:   arr.map(String)
来源：http://qjo.tarul.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cgs.gotoacloud.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mau.vehdjk.com

Ruby: arr.map(&:upcase)
来源：http://rqu.birdmap.top

C#:   arr.Select(s => s.ToUpper())
来源：http://gca.hywenlv.cn

[C08] 闭包
来源：http://vjn.shanyushiyangkeji.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ocs.yangfankeji.com

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uzz.bjfxy.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dqb.jiagoushi.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lbn.ivvv.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://aks.yonumen.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://vhm.jinghuilouyu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://med.shangyingyoupin.top

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://oxc.zhongyouzk.top

[C09] 递归
来源：http://rtd.tanke756.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://gln.jiagoushi.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ddj.tian-w.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://byz.quarkkingdee.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mfa.hesvh.cn


<!-- 参考信息 -->