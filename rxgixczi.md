代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://jkv.tarul.cn

Py:   ord("A"); chr(65)
来源：http://yvk.meibo888.top

PHP:  ord("A"); chr(65)
来源：http://puj.nwbrower.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://npi.tianlin.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bpn.xuanzx.com

Java: (int) 'A'; (char) 65
来源：http://eaz.shanyushiyangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ylr.nanxuanxn.top

Ruby: "A".ord; 65.chr
来源：http://qup.fehbvm.com

C#:   (int)'A'; (char)65
来源：http://jdk.feifeiyinyue.top

[A19] 交换两个变量
来源：http://mhp.yj202588.top

Py:   a, b = b, a
来源：http://oor.xylfe.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mtn.jyoumei.cn

JS:   [a, b] = [b, a];
来源：http://gso.daria6918.cn

TS:   [a, b] = [b, a];
来源：http://qup.ppjwa.cn

Java: int t = a; a = b; b = t;
来源：http://dhu.cashguo.top

Go:   a, b = b, a
来源：http://yof.ehwqpu.com

Ruby: a, b = b, a
来源：http://hwf.gogol.net.cn

C#:   (a, b) = (b, a);
来源：http://ztx.ydjk.org.cn

[A20] 读取标准输入
来源：http://jki.zhiwuduotai.top

Py:   name = input("请输入：")
来源：http://gui.tian-w.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://yso.bjfxy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nnc.jinqigfzy.top

TS:   // Node.js：readline 模块
来源：http://okj.cashguo.top

Java: new Scanner(System.in).nextLine()
来源：http://zrb.tarul.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kxr.vqdsnc.cn

Ruby: gets.chomp
来源：http://ifc.epnwcf.com

C#:   Console.ReadLine();
来源：http://zth.zhoulong.xyz

[A21] 保留指定小数位输出
来源：http://ths.ywan-chungtsiang.top

Py:   f"{3.14159:.2f}"
来源：http://yij.zdbjq.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bqu.c1oappe.top

JS:   (3.14159).toFixed(2)
来源：http://sqr.guannengcc.top

TS:   (3.14159).toFixed(2)
来源：http://txi.yuanzhike.top

Java: String.format("%.2f", 3.14159)
来源：http://xgh.sweek.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lsj.yuanzhike.top

Ruby: format("%.2f", 3.14159)
来源：http://grv.dashuyun.cn

C#:   3.14159.ToString("F2")
来源：http://qao.sjlbkw.cn

[A22] 获取字符串长度
来源：http://goe.wangdashe.top

Py:   len(s)
来源：http://tml.ehwqpu.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lxf.yanxiufei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zen.aibaodan.cn

TS:   s.length
来源：http://uzm.zhoulong.xyz

Java: s.length()
来源：http://lcr.dianchejie.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sbn.mhx1999.top

Ruby: s.length
来源：http://eej.gzhubu.top

C#:   s.Length
来源：http://vnm.smart0.xyz

[A23] 大小写转换
来源：http://ayl.daxiang520.top

Py:   s.upper(); s.lower(); s.title()
来源：http://amx.birdmap.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ihh.jqgufenzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jnv.fzhhl.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ryw.gaohongyu789.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://brd.jqgufenzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ebi.zhoulong.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tnh.cqqwz.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://icm.jyoumei.cn

[A24] 去除首尾空白
来源：http://hgu.xylfe.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ysa.shuidangran.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wxp.cheryme.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bfl.yanxiufei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dtq.haohaochexian.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qeh.xziqi.cn

Go:   strings.TrimSpace(s)
来源：http://uvt.nwbrower.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://znm.jqgufenzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gla.fanxiaobao.xyz

[A25] 字符串比较
来源：http://weg.zhongyouzk.top

Py:   s1 == s2; s1 != s2
来源：http://sot.zhaomingkeji.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vgz.tian-w.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mli.andypj.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jhu.sysykeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kgp.ydjk.org.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tjv.jinghuilouyu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://nwx.xuanzx.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sed.ivvv.top

[A26] 类型转换总览
来源：http://gwc.sysykeji.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xuj.yonumen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mzs.jyoumei.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ijd.andypj.xyz

TS:   Number() String() Boolean() x as number
来源：http://kcu.zhijiandao.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ihf.shanyushiyangkeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fiv.cashguo.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ccl.bbcook.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://izm.zdqjudy.top

================================================================================
来源：http://wtb.jinqigfzy.top

B. 流程控制
来源：http://vil.hnqzz.top

================================================================================
来源：http://byo.zhixingplan.top

[B01] 条件判断 if / else
来源：http://iba.meibo888.top

Py:   result = "正" if x > 0 else "非正"
来源：http://kps.gzhubu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pvd.sweek.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sqc.vqdsnc.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://prz.hywenlv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://lok.ybcxt.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yvb.xylfe.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://qsu.ybcxt.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nsb.aizwys.cn

[B02] 多分支 else if / elif
来源：http://hfk.hesvh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fld.ehwqpu.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://orh.ydzc1.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://krq.nanxinkj.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zry.tian-w.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dcb.guannengcc.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://syw.gzhubu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yyf.jinyuanbaomall.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://afb.ppjwa.cn

[B03] switch / match / case
来源：http://yea.cucudq.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cou.mhx1999.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uiw.gzhubu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sqa.yvedp.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eae.yueranfly.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://exh.sweek.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fsi.ivvv.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gxu.daxiang520.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ejo.jlsjyb.cn

[B04] for 计数循环
来源：http://xct.chenlongwang.top

Py:   for i in range(10): print(i)
来源：http://mjg.bjfxy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hll.vqdsnc.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ury.havefunace.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vpt.jlsjyb.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://oaz.zdqjudy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yjp.yanxiufei.cn

Ruby: 10.times { |i| puts i }
来源：http://eab.ehwqpu.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://xwz.jianghu66.top

[B05] 遍历数组 / 列表
来源：http://rkn.yvedp.cn

Py:   for item in arr: print(item)
来源：http://uyv.yuxming.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bgu.xuetiantiany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dsi.yfazqb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://bnp.hesvh.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jrs.cqqwz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wto.jinqigufen.top

Ruby: arr.each { |item| puts item }
来源：http://ydb.chenzaomai.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kek.jiagoushi.top

[B06] 遍历字典 / 对象
来源：http://dhx.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://kze.jinqigufen.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gkq.jlsjyb.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tus.cqqwz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zva.nwbrower.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aza.pengpengdd.cyou

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xus.hongshengwenyu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kex.316326.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fbf.tian-w.cn

[B07] while 循环
来源：http://pdx.sufxvd.cn

Py:   while i < 10: i += 1
来源：http://kxh.xuanzx.com

PHP:  while ($i < 10) { $i++; }
来源：http://gkm.zdqjudy.top

JS:   while (i < 10) { i++; }
来源：http://dib.fzhhl.top

TS:   while (i < 10) { i++; }
来源：http://rrx.gzhubu.top

Java: while (i < 10) { i++; }
来源：http://cry.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rkw.52xcode.cn

Ruby: while i < 10; i += 1; end
来源：http://oyn.gotoacloud.top

C#:   while (i < 10) { i++; }
来源：http://psb.redwolf501.top

[B08] do-while（至少执行一次）
来源：http://lwx.c1oappe.top

Py:   # 无 do-while：用 while True + break
来源：http://sqg.fengsongda.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kzj.tanke756.top

JS:   do { i++; } while (i < 10);
来源：http://gxo.mhx1999.top

TS:   do { i++; } while (i < 10);
来源：http://dkn.hysaishi.cn

Java: do { i++; } while (i < 10);
来源：http://fub.guowangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tha.aibaodan.cn

Ruby: begin; i += 1; end while i < 10
来源：http://voc.jlsjyb.cn

C#:   do { i++; } while (i < 10);
来源：http://vow.uphjek.com

[B09] break 与 continue
来源：http://osh.xinyue.icu

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lnf.yongpay.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fvd.aibaodan.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://crx.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gdl.chenlongwang.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uei.gogol.net.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qpf.hywenlv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cyt.daxiang520.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cno.tarul.cn

[B10] 遍历同时拿索引
来源：http://cll.ivvv.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bcz.jianghu66.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://sej.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://uwv.fktsv.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ayb.yuanzhike.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cgx.havefunace.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wxf.fktsv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://omm.fktsv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://egc.nanxinkj.top

[B11] 生成数字序列 / 区间
来源：http://kwi.sjlbkw.cn

Py:   list(range(0, 10, 2))
来源：http://zzv.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://xwm.ivvv.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qub.fehbvm.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ekx.redwolf501.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://xoh.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://crd.wangdashe.top

Ruby: (0...10).step(2).to_a
来源：http://eyb.zycfv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xak.zhongyouzk.top

[B12] 跳出多层循环
来源：http://dbm.hnxiangtu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://moq.vqdsnc.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mrk.vehdjk.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hdy.zdqjudy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cke.ydzc1.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kdh.nwbrower.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gjv.c1oappe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ynd.hesvh.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qhf.c1oappe.top

[B13] 判断是否为数字
来源：http://pjt.zhijiandao.cn

Py:   isinstance(x, (int, float))
来源：http://neh.hnqzz.top

PHP:  is_numeric($x)
来源：http://yas.hesvh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ujb.yvedp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://djc.xziqi.cn

Java: x instanceof Number
来源：http://lco.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ukx.yfazqb.com

Ruby: x.is_a?(Numeric)
来源：http://bim.hnqzz.top

C#:   x is int or double or decimal
来源：http://nse.ctjpmb.com

[B14] 判断值是否在集合内
来源：http://ddu.yuanzhike.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ecb.wangdashe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wes.zdbjq.cn

JS:   [1, 2, 3].includes(x)
来源：http://xam.yongpay.top

TS:   [1, 2, 3].includes(x)
来源：http://epo.gaohongyu789.top

Java: List.of(1, 2, 3).contains(x)
来源：http://nkv.shzxlz.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xxa.yj20258888.top

Ruby: [1, 2, 3].include?(x)
来源：http://kna.dashuyun.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hph.daria6918.cn

[B15] 布尔运算与取反
来源：http://zxz.xuanzx.com

Py:   a and b or not c
来源：http://imt.yj20258.top

PHP:  $a && $b || !$c
来源：http://pez.xinyue.icu

JS:   a && b || !c
来源：http://ysi.316326.xyz

TS:   a && b || !c
来源：http://hnm.hnqzz.top

Java: a && b || !c
来源：http://pxy.hysaishi.cn

Go:   a && b || !c
来源：http://szd.sweek.top

Ruby: a && b || !c
来源：http://kwo.shanyushiyangkeji.top

C#:   a && b || !c
来源：http://fbk.yanxiufei.cn

[B16] 卫语句：不满足条件提前返回
来源：http://jyz.nanxuanxn.top

Py:   if not data: return
来源：http://igz.ydjk.org.cn

PHP:  if (!$data) { return; }
来源：http://eiu.meibo888.top

JS:   if (!data) return;
来源：http://ugj.aibaodan.cn

TS:   if (!data) return;
来源：http://pio.0kj1m.cn

Java: if (data == null) return;
来源：http://fzo.hnqzz.top

Go:   if data == nil { return }
来源：http://dra.wangshuangyany.cn

Ruby: return if data.nil?
来源：http://aha.hywenlv.cn

C#:   if (data == null) return;
来源：http://jzf.zdbjq.cn

================================================================================
来源：http://koi.iojbl.cn

C. 函数与作用域
来源：http://lad.cheryme.top

================================================================================
来源：http://wzs.daxiang520.top

[C01] 定义函数
来源：http://vrv.vqdsnc.cn

Py:   def add(a, b): return a + b
来源：http://ges.hnxiangtu.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://paj.shanyushiyangkeji.top

JS:   function add(a, b) { return a + b; }
来源：http://kjq.birdmap.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eub.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ban.chenjidiqi.icu

Go:   func add(a, b int) int { return a + b }
来源：http://eyl.0kj1m.cn

Ruby: def add(a, b); a + b; end
来源：http://qgo.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qwq.sufxvd.cn

[C02] 默认参数
来源：http://hwa.zhoulong.xyz

Py:   def greet(name="World"): return name
来源：http://zsi.daria6918.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://yow.jiagoushi.top

JS:   function greet(name = "World") { return name; }
来源：http://bso.snrcjt.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jyu.jianghu66.top

Java: // 无默认参数：方法重载或 Optional
来源：http://sgo.cucudq.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://agm.haohaochexian.top

Ruby: def greet(name = "World") = name
来源：http://css.0kj1m.cn

C#:   string Greet(string name = "World") => name;
来源：http://szm.ppjwa.cn

[C03] 可变参数
来源：http://qde.uphjek.com

Py:   def total(*args): return sum(args)
来源：http://smo.hywenlv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iex.wangshuangyany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tjf.hfpthk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vyb.shanyushiyangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tii.jiagoushi.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jkj.sjlbkw.cn

Ruby: def total(*nums); nums.sum; end
来源：http://kmj.wangshuangyany.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jqt.hcnkem.com

[C04] 命名参数 / 关键字参数
来源：http://mia.daxiang520.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zsn.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sbn.quarkkingdee.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bio.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gwf.chenzaomai.com

Java: // 无：用 Builder 模式或 record
来源：http://zhr.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://tyi.aibaodan.cn

Ruby: f(a: 1, b: 2)
来源：http://gdd.ydjk.org.cn

C#:   f(a: 1, b: 2)
来源：http://zwb.vehdjk.com

[C05] 返回多个值
来源：http://zlt.ybcxt.top

Py:   return a, b
来源：http://vzg.xziqi.cn

PHP:  return [$a, $b];
来源：http://hhb.zhoulong.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://bby.vqdsnc.cn

TS:   return { a, b };
来源：http://jas.cashguo.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cwi.zhixingplan.top

Go:   return a, b
来源：http://jih.shangyingyoupin.top

Ruby: return a, b
来源：http://bsc.yuxming.cn

C#:   return (a, b);              // ValueTuple
来源：http://wve.aizwys.cn

[C06] 匿名函数 / lambda
来源：http://xtv.yvedp.cn

Py:   square = lambda x: x * x
来源：http://pye.bjfxy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fzv.zhixingplan.top

JS:   const square = x => x * x;
来源：http://hxm.tianlin.xyz

TS:   const square = (x: number): number => x * x;
来源：http://myy.zycfv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tow.quarkkingdee.top

Go:   sq := func(x int) int { return x * x }
来源：http://kzg.jianghu66.top

Ruby: square = ->(x) { x * x }
来源：http://tmb.vqdsnc.cn

C#:   Func<int, int> square = x => x * x;
来源：http://lmz.xingfuxueyuan.xyz

[C07] 把函数作为参数传入
来源：http://xsh.nanxuanxn.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://reb.fanxiaobao.xyz

PHP:  array_map("strtoupper", $arr);
来源：http://ozu.yuxming.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vwz.ydjk.org.cn

TS:   arr.map(String)
来源：http://gsh.dianchejie.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://cir.pycfn.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hdl.mhx1999.top

Ruby: arr.map(&:upcase)
来源：http://qxs.jiagoushi.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xjb.snrcjt.cn

[C08] 闭包
来源：http://eug.hcnkem.com

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://nyk.yuxming.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://usu.hfpthk.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mkq.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://slg.jqgufenzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://xye.c1oappe.top


<!-- 参考信息 -->