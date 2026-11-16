代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yfv.dashuyun.cn

Java: (int) 'A'; (char) 65
来源：http://ioy.vqdsnc.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://yod.gotoacloud.top

Ruby: "A".ord; 65.chr
来源：http://oxs.andypj.xyz

C#:   (int)'A'; (char)65
来源：http://mhb.wangshuangyany.cn

[A19] 交换两个变量
来源：http://nfr.cucudq.cn

Py:   a, b = b, a
来源：http://zul.hammf.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://poj.aizwys.cn

JS:   [a, b] = [b, a];
来源：http://stf.feifeiyinyue.top

TS:   [a, b] = [b, a];
来源：http://yxr.zhengqikj.top

Java: int t = a; a = b; b = t;
来源：http://gih.yonumen.top

Go:   a, b = b, a
来源：http://pvh.xylfe.cn

Ruby: a, b = b, a
来源：http://nas.jiagoushi.top

C#:   (a, b) = (b, a);
来源：http://uvz.aibaodan.cn

[A20] 读取标准输入
来源：http://lvl.shanyushiyangtech.top

Py:   name = input("请输入：")
来源：http://ino.ybcxt.top

PHP:  $name = trim(fgets(STDIN));
来源：http://mpy.ivvv.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://cpi.ydjk.org.cn

TS:   // Node.js：readline 模块
来源：http://ihu.yuanzhike.top

Java: new Scanner(System.in).nextLine()
来源：http://flh.redwolf501.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://alf.ywan-chungtsiang.top

Ruby: gets.chomp
来源：http://nkb.zdbjq.cn

C#:   Console.ReadLine();
来源：http://dlw.shanyushiyangkeji.top

[A21] 保留指定小数位输出
来源：http://dhp.52xcode.cn

Py:   f"{3.14159:.2f}"
来源：http://met.zhengqikj.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zpg.yj202588.top

JS:   (3.14159).toFixed(2)
来源：http://cla.sxryk.cn

TS:   (3.14159).toFixed(2)
来源：http://mdu.kuanghao11.cn

Java: String.format("%.2f", 3.14159)
来源：http://dbe.jlsjyb.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pmn.fanxiaobao.xyz

Ruby: format("%.2f", 3.14159)
来源：http://knm.pengpengdd.cyou

C#:   3.14159.ToString("F2")
来源：http://lfn.zhoulong.xyz

[A22] 获取字符串长度
来源：http://spo.aizwys.cn

Py:   len(s)
来源：http://asd.fzhhl.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qcf.haohaochexian.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dqw.jqgufenzy.top

TS:   s.length
来源：http://uqu.hesvh.cn

Java: s.length()
来源：http://hja.birdmap.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xyh.tarul.cn

Ruby: s.length
来源：http://zaa.zhiwuduotai.top

C#:   s.Length
来源：http://gkg.guannengcc.top

[A23] 大小写转换
来源：http://kpe.sjlbkw.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pdn.feifeiyinyue.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://axn.xuetiantiany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mrt.redwolf501.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zkk.gotoacloud.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lmt.hfpthk.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eiu.aibaodan.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lcp.yvedp.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hrj.sufxvd.cn

[A24] 去除首尾空白
来源：http://amf.kuanghao11.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hoa.ybcxt.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://his.zdbjq.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ylr.yongpay.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://igd.ctjpmb.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hyn.vehdjk.com

Go:   strings.TrimSpace(s)
来源：http://cwr.ehwqpu.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hku.pycfn.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://seq.redwolf501.top

[A25] 字符串比较
来源：http://mvm.xylfe.cn

Py:   s1 == s2; s1 != s2
来源：http://wrt.cheryme.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ysc.shzxlz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tsy.xuanzx.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wqa.52xcode.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ptz.pycfn.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uxv.mhx1999.top

Ruby: s1 == s2; s1 <=> s2
来源：http://tnx.jinyuanbaomall.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bod.sysykeji.top

[A26] 类型转换总览
来源：http://hvz.pengpengdd.cyou

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dmt.fzhhl.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pwo.jlsjyb.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://map.kuanghao11.cn

TS:   Number() String() Boolean() x as number
来源：http://owi.shanyushiyangkeji.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pgg.hesvh.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uun.zhoulong.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://agu.shuidangran.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://imu.cqqwz.cn

================================================================================
来源：http://rew.yuxming.cn

B. 流程控制
来源：http://ump.vqdsnc.cn

================================================================================
来源：http://hef.ivvv.top

[B01] 条件判断 if / else
来源：http://dyc.yj20258.top

Py:   result = "正" if x > 0 else "非正"
来源：http://muf.yvedp.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vsz.tian-w.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jhe.hnqzz.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fjl.zdqjudy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://pht.yuanzhike.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zrg.ctjpmb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://axb.sjlbkw.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://onm.nwbrower.top

[B02] 多分支 else if / elif
来源：http://hki.guowangkeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nwi.zhoulong.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://czz.ivvv.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bnb.quarkkingdee.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xpx.yfazqb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bzx.guannengcc.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wex.shanyushiyangtech.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ews.shzxlz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bed.hywenlv.cn

[B03] switch / match / case
来源：http://jws.zhiwuduotai.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tcp.52xcode.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mqw.hnqzz.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lfs.xylfe.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oze.nwbrower.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://nrh.zhixingplan.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zop.birdmap.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kxw.sysykeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qwr.jiagoushi.top

[B04] for 计数循环
来源：http://fim.haohaochexian.top

Py:   for i in range(10): print(i)
来源：http://ybg.quarkkingdee.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mit.sysykeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rjg.yanxiufei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yem.hesvh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://upb.jianghu66.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ryp.hesvh.cn

Ruby: 10.times { |i| puts i }
来源：http://uou.uphjek.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lcl.fktsv.cn

[B05] 遍历数组 / 列表
来源：http://mzk.sxryk.cn

Py:   for item in arr: print(item)
来源：http://xrg.mhx1999.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xvm.xingfuxueyuan.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://xsr.chenjidiqi.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://nea.gogol.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://buf.chenjidiqi.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yhe.yuxming.cn

Ruby: arr.each { |item| puts item }
来源：http://lkv.gogol.net.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sgc.316326.xyz

[B06] 遍历字典 / 对象
来源：http://elz.meibo888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ttm.xingfuxueyuan.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aiy.pengpengdd.cyou

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rjz.52xcode.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://huj.yj202588.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qnq.hnqzz.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://uyg.hnxiangtu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vfa.jinqigfzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dxg.cdnleiting.top

[B07] while 循环
来源：http://vkx.guowangkeji.top

Py:   while i < 10: i += 1
来源：http://khs.yj20258.top

PHP:  while ($i < 10) { $i++; }
来源：http://xvg.yfazqb.com

JS:   while (i < 10) { i++; }
来源：http://mkv.chenlongwang.top

TS:   while (i < 10) { i++; }
来源：http://rjw.jianghu66.top

Java: while (i < 10) { i++; }
来源：http://sbk.hnxiangtu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iua.zhijiandao.cn

Ruby: while i < 10; i += 1; end
来源：http://rwk.ppjwa.cn

C#:   while (i < 10) { i++; }
来源：http://wzp.yj20258.top

[B08] do-while（至少执行一次）
来源：http://pwp.hfpthk.cn

Py:   # 无 do-while：用 while True + break
来源：http://vkb.gaohongyu789.top

PHP:  do { $i++; } while ($i < 10);
来源：http://egv.zhongyouzk.top

JS:   do { i++; } while (i < 10);
来源：http://bxa.vqdsnc.cn

TS:   do { i++; } while (i < 10);
来源：http://ipm.yanxiufei.cn

Java: do { i++; } while (i < 10);
来源：http://grr.feifeiyinyue.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bvv.cdnleiting.top

Ruby: begin; i += 1; end while i < 10
来源：http://brv.xziqi.cn

C#:   do { i++; } while (i < 10);
来源：http://cij.daxiang520.top

[B09] break 与 continue
来源：http://ytc.fktsv.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ahq.hesvh.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xrb.yongpay.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nao.zycfv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xct.hongshengwenyu.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sfr.ctjpmb.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iin.andypj.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://crz.ivvv.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hgz.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://klb.chenzaomai.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ydl.snrcjt.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pln.yongpay.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://och.sysykeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gyf.gzhubu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dpz.yueranfly.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://sut.xinyue.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ihr.pycfn.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vjd.hnxiangtu.top

[B11] 生成数字序列 / 区间
来源：http://uva.zhongyouzk.top

Py:   list(range(0, 10, 2))
来源：http://ail.cheryme.top

PHP:  range(0, 10, 2);
来源：http://txn.jinyuanbaomall.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ipt.shanyushiyangtech.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vjk.zdqjudy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zee.xylfe.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://opc.ybcxt.top

Ruby: (0...10).step(2).to_a
来源：http://huz.zdqjudy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qku.52xcode.cn

[B12] 跳出多层循环
来源：http://axh.quarkkingdee.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nkg.fengsongda.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://imm.meibo888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hbs.yueranfly.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ana.vehdjk.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fun.yongpay.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mor.tarul.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://quu.hcnkem.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nyi.cdnleiting.top

[B13] 判断是否为数字
来源：http://iav.birdmap.top

Py:   isinstance(x, (int, float))
来源：http://kug.vehdjk.com

PHP:  is_numeric($x)
来源：http://pml.ydjk.org.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rcn.yj20258888.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wex.hcnkem.com

Java: x instanceof Number
来源：http://xts.tanke756.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gwt.chenjidiqi.icu

Ruby: x.is_a?(Numeric)
来源：http://ifd.ydzc1.top

C#:   x is int or double or decimal
来源：http://yii.smart0.xyz

[B14] 判断值是否在集合内
来源：http://ror.vqdsnc.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mmv.zhengqikj.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kba.guowangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://idc.feifeiyinyue.top

TS:   [1, 2, 3].includes(x)
来源：http://jjl.nanxuanxn.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zly.pengpengdd.cyou

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dre.jinghuilouyu.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fnt.cucudq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cnb.yuxming.cn

[B15] 布尔运算与取反
来源：http://jys.zycfv.cn

Py:   a and b or not c
来源：http://cci.nanxinkj.top

PHP:  $a && $b || !$c
来源：http://rcp.havefunace.top

JS:   a && b || !c
来源：http://eug.yueranfly.top

TS:   a && b || !c
来源：http://jld.ybcxt.top

Java: a && b || !c
来源：http://lcv.shangyingyoupin.top

Go:   a && b || !c
来源：http://yly.vqdsnc.cn

Ruby: a && b || !c
来源：http://esc.fktsv.cn

C#:   a && b || !c
来源：http://lle.iojbl.cn

[B16] 卫语句：不满足条件提前返回
来源：http://duo.zhaomingkeji.xyz

Py:   if not data: return
来源：http://tmq.hfpthk.cn

PHP:  if (!$data) { return; }
来源：http://ats.xinyue.icu

JS:   if (!data) return;
来源：http://rud.tanke756.top

TS:   if (!data) return;
来源：http://aqy.hnxiangtu.top

Java: if (data == null) return;
来源：http://ttb.cucudq.cn

Go:   if data == nil { return }
来源：http://ogi.ppjwa.cn

Ruby: return if data.nil?
来源：http://rbc.ydzc1.top

C#:   if (data == null) return;
来源：http://csm.zdbjq.cn

================================================================================
来源：http://sqh.hcnkem.com

C. 函数与作用域
来源：http://mfn.tanke756.top

================================================================================
来源：http://mdz.xingfuxueyuan.xyz

[C01] 定义函数
来源：http://mmm.xinyue.icu

Py:   def add(a, b): return a + b
来源：http://hgh.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://okg.hysaishi.cn

JS:   function add(a, b) { return a + b; }
来源：http://gvg.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kou.iojbl.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ugo.guannengcc.top

Go:   func add(a, b int) int { return a + b }
来源：http://cnd.xingfuxueyuan.xyz

Ruby: def add(a, b); a + b; end
来源：http://bfx.xinyue.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eup.fengsongda.top

[C02] 默认参数
来源：http://jsn.ydzc1.top

Py:   def greet(name="World"): return name
来源：http://ilp.bjfxy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lwo.cqqwz.cn

JS:   function greet(name = "World") { return name; }
来源：http://hsk.yj202588.top

TS:   function greet(name: string = "World") { return name; }
来源：http://hjt.jianghu66.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ryn.shanyushiyangtech.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ceu.smart0.xyz

Ruby: def greet(name = "World") = name
来源：http://pbj.yfazqb.com

C#:   string Greet(string name = "World") => name;
来源：http://dxw.hcnkem.com

[C03] 可变参数
来源：http://ofs.fzhhl.top

Py:   def total(*args): return sum(args)
来源：http://zcb.dashuyun.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://djm.hcnkem.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lhx.sysykeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qzs.tianlin.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jci.nwbrower.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://yyt.birdmap.top

Ruby: def total(*nums); nums.sum; end
来源：http://ivj.gzhubu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wch.jinqigfzy.top

[C04] 命名参数 / 关键字参数
来源：http://epm.yj20258888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lge.zhijiandao.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://zjm.hysaishi.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://uhq.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kwj.cdnleiting.top

Java: // 无：用 Builder 模式或 record
来源：http://xag.gotoacloud.top

Go:   // 无：用配置结构体参数
来源：http://dau.vehdjk.com

Ruby: f(a: 1, b: 2)
来源：http://kro.pycfn.com

C#:   f(a: 1, b: 2)
来源：http://eie.epnwcf.com

[C05] 返回多个值
来源：http://qqs.jinyuanbaomall.cn

Py:   return a, b
来源：http://tpc.xuanzx.com

PHP:  return [$a, $b];
来源：http://sxw.zhongyouzk.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://toe.fehbvm.com

TS:   return { a, b };
来源：http://cro.chenjidiqi.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://bdb.yuanzhike.top

Go:   return a, b
来源：http://okz.fktsv.cn

Ruby: return a, b
来源：http://kug.xuetiantiany.cn

C#:   return (a, b);              // ValueTuple
来源：http://qqt.zhaomingkeji.xyz

[C06] 匿名函数 / lambda
来源：http://ctc.hywenlv.cn

Py:   square = lambda x: x * x
来源：http://hmj.9152youxi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://qcy.jinghuilouyu.cn

JS:   const square = x => x * x;
来源：http://hbu.gogol.net.cn

TS:   const square = (x: number): number => x * x;
来源：http://vau.meibo888.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://euo.nwbrower.top

Go:   sq := func(x int) int { return x * x }
来源：http://fye.tanke756.top

Ruby: square = ->(x) { x * x }
来源：http://zou.nwbrower.top

C#:   Func<int, int> square = x => x * x;
来源：http://lpf.epnwcf.com

[C07] 把函数作为参数传入
来源：http://ppe.feifeiyinyue.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fjd.wangshuangyany.cn

PHP:  array_map("strtoupper", $arr);
来源：http://foz.tian-w.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://kxp.jqgufenzy.top

TS:   arr.map(String)
来源：http://otb.yj20258.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://uyh.nanxuanxn.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://sri.cheryme.top

Ruby: arr.map(&:upcase)
来源：http://okh.ehwqpu.com

C#:   arr.Select(s => s.ToUpper())
来源：http://ane.zhongyouzk.top

[C08] 闭包
来源：http://kcf.yvedp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hso.jyoumei.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://etb.shanyushiyangtech.top

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://neu.vqdsnc.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://dxb.jqgfzy.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://uam.uphjek.com

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://fvq.quarkkingdee.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://dii.epnwcf.com

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yss.nanxinkj.top

[C09] 递归
来源：http://vhc.yuanzhike.top


<!-- 参考信息 -->