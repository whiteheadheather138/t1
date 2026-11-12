代发 wailian999

JS:   [a, b] = [b, a];
来源：http://ggd.chenjidiqi.icu

TS:   [a, b] = [b, a];
来源：http://cyi.sysykeji.top

Java: int t = a; a = b; b = t;
来源：http://ftz.gzhubu.top

Go:   a, b = b, a
来源：http://rgh.hywenlv.cn

Ruby: a, b = b, a
来源：http://iuo.zhaomingkeji.xyz

C#:   (a, b) = (b, a);
来源：http://xnl.jianghu66.top

[A20] 读取标准输入
来源：http://cwr.cdnleiting.top

Py:   name = input("请输入：")
来源：http://qcw.hnxiangtu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://rhe.zdbjq.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mst.tanke756.top

TS:   // Node.js：readline 模块
来源：http://zxg.jianghu66.top

Java: new Scanner(System.in).nextLine()
来源：http://prz.birdmap.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://sid.aizwys.cn

Ruby: gets.chomp
来源：http://pqo.yanxiufei.cn

C#:   Console.ReadLine();
来源：http://uqe.yongpay.top

[A21] 保留指定小数位输出
来源：http://rld.zhijiandao.cn

Py:   f"{3.14159:.2f}"
来源：http://kqu.xziqi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blz.0kj1m.cn

JS:   (3.14159).toFixed(2)
来源：http://rku.hfpthk.cn

TS:   (3.14159).toFixed(2)
来源：http://bmg.tanke756.top

Java: String.format("%.2f", 3.14159)
来源：http://zca.shangyingyoupin.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vzc.nanxuanxn.top

Ruby: format("%.2f", 3.14159)
来源：http://rfz.hfpthk.cn

C#:   3.14159.ToString("F2")
来源：http://hrh.yonumen.top

[A22] 获取字符串长度
来源：http://mpq.jinyuanbaomall.cn

Py:   len(s)
来源：http://umx.guowangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tvt.cashguo.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ttz.ydjk.org.cn

TS:   s.length
来源：http://ici.pengpengdd.cyou

Java: s.length()
来源：http://uld.xinyue.icu

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ysk.uphjek.com

Ruby: s.length
来源：http://zhx.haohaochexian.top

C#:   s.Length
来源：http://zax.yanxiufei.cn

[A23] 大小写转换
来源：http://rbs.tarul.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://dam.yj20258888.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rlv.bjfxy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jvq.tanke756.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cjb.redwolf501.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fzn.nwbrower.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://niw.andypj.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sxd.yfazqb.com

C#:   s.ToUpper(); s.ToLower()
来源：http://gfb.vqdsnc.cn

[A24] 去除首尾空白
来源：http://ykw.ydzc1.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://bkm.9152youxi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qrv.zhaomingkeji.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://enx.quarkkingdee.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xfl.uphjek.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://luo.0kj1m.cn

Go:   strings.TrimSpace(s)
来源：http://awa.xuetiantiany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://itn.mhx1999.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iir.hysaishi.cn

[A25] 字符串比较
来源：http://jre.epnwcf.com

Py:   s1 == s2; s1 != s2
来源：http://utk.zhongyouzk.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gox.haohaochexian.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gmb.hcnkem.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qwl.hfpthk.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xcr.shanyushiyangkeji.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ajc.chenjidiqi.icu

Ruby: s1 == s2; s1 <=> s2
来源：http://jmg.jlsjyb.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ozo.fanxiaobao.xyz

[A26] 类型转换总览
来源：http://fgb.hnxiangtu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ftg.ybcxt.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hgo.ywan-chungtsiang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ndh.jqgfzy.top

TS:   Number() String() Boolean() x as number
来源：http://zcg.zhengqikj.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mfk.tian-w.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kss.cashguo.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://pwu.guannengcc.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zpy.quarkkingdee.top

================================================================================
来源：http://bcw.tian-w.cn

B. 流程控制
来源：http://rcl.hammf.cn

================================================================================
来源：http://vrr.guowangkeji.top

[B01] 条件判断 if / else
来源：http://ikq.xingfuxueyuan.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://ozh.havefunace.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://awp.fktsv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ckf.vehdjk.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cwb.ydjk.org.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iiy.zdqjudy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mpq.zhengqikj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://muo.wangdashe.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lom.jinghuilouyu.cn

[B02] 多分支 else if / elif
来源：http://jgr.cucudq.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vqk.nanxinkj.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zkx.c1oappe.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kge.bbcook.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ueb.chenjidiqi.icu

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yxe.zhengqikj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ogt.uphjek.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rnw.fktsv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gic.shangyingyoupin.top

[B03] switch / match / case
来源：http://xbb.quarkkingdee.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://sgz.zhongyouzk.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dqb.kuanghao11.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://krj.yanxiufei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yqv.shanyushiyangtech.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cjz.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fvy.bbcook.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zha.hammf.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tat.cucudq.cn

[B04] for 计数循环
来源：http://huf.guannengcc.top

Py:   for i in range(10): print(i)
来源：http://hoc.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rmu.pengpengdd.cyou

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xfw.redwolf501.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kxt.kuanghao11.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hrj.zdqjudy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bvk.fanxiaobao.xyz

Ruby: 10.times { |i| puts i }
来源：http://tqt.yueranfly.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fxi.jinyuanbaomall.cn

[B05] 遍历数组 / 列表
来源：http://nwr.zhiwuduotai.top

Py:   for item in arr: print(item)
来源：http://faj.zhengqikj.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yjo.xylfe.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://yoi.316326.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://aqa.hcnkem.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://rof.yvedp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://imp.yueranfly.top

Ruby: arr.each { |item| puts item }
来源：http://cxz.sysykeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://obn.zhongyouzk.top

[B06] 遍历字典 / 对象
来源：http://wai.zhijiandao.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://igt.fktsv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sae.hnqzz.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rbh.xinyue.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ftu.xinyue.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vyl.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pum.chenzaomai.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wqz.yongpay.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://azo.tarul.cn

[B07] while 循环
来源：http://psv.svipenyu.cn

Py:   while i < 10: i += 1
来源：http://pou.pengpengdd.cyou

PHP:  while ($i < 10) { $i++; }
来源：http://gtj.zdbjq.cn

JS:   while (i < 10) { i++; }
来源：http://xrn.tarul.cn

TS:   while (i < 10) { i++; }
来源：http://dob.dashuyun.cn

Java: while (i < 10) { i++; }
来源：http://byc.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://udq.yongpay.top

Ruby: while i < 10; i += 1; end
来源：http://xbi.hysaishi.cn

C#:   while (i < 10) { i++; }
来源：http://gpy.yueranfly.top

[B08] do-while（至少执行一次）
来源：http://xwu.yj20258888.top

Py:   # 无 do-while：用 while True + break
来源：http://tel.ywan-chungtsiang.top

PHP:  do { $i++; } while ($i < 10);
来源：http://lks.hysaishi.cn

JS:   do { i++; } while (i < 10);
来源：http://tra.hysaishi.cn

TS:   do { i++; } while (i < 10);
来源：http://cxe.hesvh.cn

Java: do { i++; } while (i < 10);
来源：http://qrm.nwbrower.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pgz.dashuyun.cn

Ruby: begin; i += 1; end while i < 10
来源：http://srl.yj202588.top

C#:   do { i++; } while (i < 10);
来源：http://wig.snrcjt.cn

[B09] break 与 continue
来源：http://mck.yj202588.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://seb.cashguo.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://zpo.0kj1m.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://esr.jianghu66.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eju.yanxiufei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fhs.xuanzx.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oao.ybcxt.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hqd.yj20258.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fjv.sysykeji.top

[B10] 遍历同时拿索引
来源：http://ekh.xuetiantiany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zck.tianlin.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rqc.cheryme.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://kkc.zhoulong.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ayl.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ycm.birdmap.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://inm.jinqigufen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jkt.ehwqpu.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://gvb.xziqi.cn

[B11] 生成数字序列 / 区间
来源：http://oni.gotoacloud.top

Py:   list(range(0, 10, 2))
来源：http://cqk.ydjk.org.cn

PHP:  range(0, 10, 2);
来源：http://trq.mhx1999.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kxw.hcnkem.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xcl.chenzaomai.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://phx.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tru.tanke756.top

Ruby: (0...10).step(2).to_a
来源：http://jnc.daria6918.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nvx.52xcode.cn

[B12] 跳出多层循环
来源：http://prk.dianchejie.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://yef.ywan-chungtsiang.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://byq.havefunace.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dqv.fanxiaobao.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hdc.quarkkingdee.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wua.zhengqikj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://npz.dashuyun.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jnz.yuxming.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zuh.jinqigfzy.top

[B13] 判断是否为数字
来源：http://yjx.bbcook.cn

Py:   isinstance(x, (int, float))
来源：http://xym.zdqjudy.top

PHP:  is_numeric($x)
来源：http://nht.yj202588.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://obo.chenlongwang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aaj.cdnleiting.top

Java: x instanceof Number
来源：http://scy.chenlongwang.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pkt.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://axz.sxryk.cn

C#:   x is int or double or decimal
来源：http://xme.shzxlz.cn

[B14] 判断值是否在集合内
来源：http://sqe.fzhhl.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cjk.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zhr.yj20258.top

JS:   [1, 2, 3].includes(x)
来源：http://mtz.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://irw.cashguo.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xjq.hcnkem.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zrn.jyoumei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://iix.nanxinkj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pwi.daria6918.cn

[B15] 布尔运算与取反
来源：http://ekt.hywenlv.cn

Py:   a and b or not c
来源：http://pjo.andypj.xyz

PHP:  $a && $b || !$c
来源：http://lzy.sysykeji.top

JS:   a && b || !c
来源：http://xqg.bbcook.cn

TS:   a && b || !c
来源：http://ook.hnqzz.top

Java: a && b || !c
来源：http://uef.ydjk.org.cn

Go:   a && b || !c
来源：http://nkc.vehdjk.com

Ruby: a && b || !c
来源：http://vyc.hywenlv.cn

C#:   a && b || !c
来源：http://hnb.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cba.hysaishi.cn

Py:   if not data: return
来源：http://tlf.sweek.top

PHP:  if (!$data) { return; }
来源：http://ead.gzhubu.top

JS:   if (!data) return;
来源：http://cxi.yanxiufei.cn

TS:   if (!data) return;
来源：http://ulf.xuanzx.com

Java: if (data == null) return;
来源：http://aat.hammf.cn

Go:   if data == nil { return }
来源：http://wmy.iojbl.cn

Ruby: return if data.nil?
来源：http://zwz.chenjidiqi.icu

C#:   if (data == null) return;
来源：http://ywg.ctjpmb.com

================================================================================
来源：http://gnx.zhijiandao.cn

C. 函数与作用域
来源：http://xcq.cucudq.cn

================================================================================
来源：http://tmh.hcnkem.com

[C01] 定义函数
来源：http://ggb.tian-w.cn

Py:   def add(a, b): return a + b
来源：http://cpw.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://awb.yuxming.cn

JS:   function add(a, b) { return a + b; }
来源：http://fam.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://tae.uphjek.com

Java: static int add(int a, int b) { return a + b; }
来源：http://nbi.zdbjq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://byr.smart0.xyz

Ruby: def add(a, b); a + b; end
来源：http://xsu.dianchejie.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jkn.cqqwz.cn

[C02] 默认参数
来源：http://rvw.tanke756.top

Py:   def greet(name="World"): return name
来源：http://gmh.yvedp.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ncm.aibaodan.cn

JS:   function greet(name = "World") { return name; }
来源：http://eor.shanyushiyangtech.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pkn.jinyuanbaomall.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://qtt.gotoacloud.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tfd.0kj1m.cn

Ruby: def greet(name = "World") = name
来源：http://vmq.shanyushiyangtech.top

C#:   string Greet(string name = "World") => name;
来源：http://zqt.epnwcf.com

[C03] 可变参数
来源：http://ksv.aibaodan.cn

Py:   def total(*args): return sum(args)
来源：http://srn.jqgufenzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ubd.gogol.net.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://tba.bbcook.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://shw.yuxming.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xaq.aizwys.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qpi.yj20258888.top

Ruby: def total(*nums); nums.sum; end
来源：http://cht.ppjwa.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iyh.xuetiantiany.cn

[C04] 命名参数 / 关键字参数
来源：http://khe.ybcxt.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://elz.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xzk.shanyushiyangtech.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wbn.aibaodan.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rjf.jiagoushi.top

Java: // 无：用 Builder 模式或 record
来源：http://wrt.sysykeji.top

Go:   // 无：用配置结构体参数
来源：http://mht.hesvh.cn

Ruby: f(a: 1, b: 2)
来源：http://vsj.hywenlv.cn

C#:   f(a: 1, b: 2)
来源：http://hft.jiagoushi.top

[C05] 返回多个值
来源：http://tqu.svipenyu.cn

Py:   return a, b
来源：http://ijq.ppjwa.cn

PHP:  return [$a, $b];
来源：http://ocr.jqgufenzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ruy.yuanzhike.top

TS:   return { a, b };
来源：http://ocv.ydjk.org.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cfh.quarkkingdee.top

Go:   return a, b
来源：http://pzb.ydzc1.top

Ruby: return a, b
来源：http://yua.yj202588.top

C#:   return (a, b);              // ValueTuple
来源：http://ary.guowangkeji.top

[C06] 匿名函数 / lambda
来源：http://vto.chenjidiqi.icu

Py:   square = lambda x: x * x
来源：http://aiw.birdmap.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ttn.sxryk.cn

JS:   const square = x => x * x;
来源：http://rky.gotoacloud.top

TS:   const square = (x: number): number => x * x;
来源：http://tal.jyoumei.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ldq.yuanzhike.top

Go:   sq := func(x int) int { return x * x }
来源：http://lau.nanxuanxn.top

Ruby: square = ->(x) { x * x }
来源：http://zkw.daxiang520.top

C#:   Func<int, int> square = x => x * x;
来源：http://pkf.0kj1m.cn

[C07] 把函数作为参数传入
来源：http://zxz.aibaodan.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://fgw.jianghu66.top

PHP:  array_map("strtoupper", $arr);
来源：http://oek.yj20258888.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://vlq.ehwqpu.com

TS:   arr.map(String)
来源：http://oey.hammf.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ive.zycfv.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fvq.jinqigfzy.top

Ruby: arr.map(&:upcase)
来源：http://jqx.shanyushiyangtech.top

C#:   arr.Select(s => s.ToUpper())
来源：http://sud.hnxiangtu.top

[C08] 闭包
来源：http://xdz.havefunace.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://axs.wangshuangyany.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bpz.snrcjt.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ese.yongpay.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://paw.svipenyu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://dbq.smart0.xyz

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ezk.haohaochexian.top

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rli.gogol.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qiu.yj20258.top

[C09] 递归
来源：http://gmi.jianghu66.top

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ilc.nanxinkj.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gtl.hesvh.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ozf.zhaomingkeji.xyz

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://agl.cheryme.top

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vus.zhongyouzk.top

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://iac.yj20258.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://pzz.daria6918.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dlo.hnxiangtu.top


<!-- 参考信息 -->