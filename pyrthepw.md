代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yor.zhixingplan.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wjg.yongpay.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vlq.daria6918.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hgi.hammf.cn

[A18] 字符与 ASCII 码互转
来源：http://qrr.yvedp.cn

Py:   ord("A"); chr(65)
来源：http://kde.daria6918.cn

PHP:  ord("A"); chr(65)
来源：http://yro.cashguo.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://quw.jqgfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ecy.yuxming.cn

Java: (int) 'A'; (char) 65
来源：http://cjy.dashuyun.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://btw.sufxvd.cn

Ruby: "A".ord; 65.chr
来源：http://otw.pycfn.com

C#:   (int)'A'; (char)65
来源：http://vxj.aizwys.cn

[A19] 交换两个变量
来源：http://ims.jinghuilouyu.cn

Py:   a, b = b, a
来源：http://utx.andypj.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://clj.jqgfzy.top

JS:   [a, b] = [b, a];
来源：http://lld.fehbvm.com

TS:   [a, b] = [b, a];
来源：http://qei.zdqjudy.top

Java: int t = a; a = b; b = t;
来源：http://hbi.daxiang520.top

Go:   a, b = b, a
来源：http://utg.aizwys.cn

Ruby: a, b = b, a
来源：http://ajw.havefunace.top

C#:   (a, b) = (b, a);
来源：http://wmu.tianlin.xyz

[A20] 读取标准输入
来源：http://qpj.zdqjudy.top

Py:   name = input("请输入：")
来源：http://ist.shanyushiyangtech.top

PHP:  $name = trim(fgets(STDIN));
来源：http://iid.tianlin.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zbl.jqgufenzy.top

TS:   // Node.js：readline 模块
来源：http://wsk.ydzc1.top

Java: new Scanner(System.in).nextLine()
来源：http://bjl.yvedp.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://twx.zhongyouzk.top

Ruby: gets.chomp
来源：http://pwi.cqqwz.cn

C#:   Console.ReadLine();
来源：http://dkt.svipenyu.cn

[A21] 保留指定小数位输出
来源：http://awk.hcnkem.com

Py:   f"{3.14159:.2f}"
来源：http://fml.shuidangran.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tcn.jinyuanbaomall.cn

JS:   (3.14159).toFixed(2)
来源：http://gky.jqgfzy.top

TS:   (3.14159).toFixed(2)
来源：http://aeb.dashuyun.cn

Java: String.format("%.2f", 3.14159)
来源：http://bnl.yj202588.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hbi.hongshengwenyu.top

Ruby: format("%.2f", 3.14159)
来源：http://nui.yueranfly.top

C#:   3.14159.ToString("F2")
来源：http://von.zhiwuduotai.top

[A22] 获取字符串长度
来源：http://col.tian-w.cn

Py:   len(s)
来源：http://ggb.havefunace.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://pkk.zycfv.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bxp.fehbvm.com

TS:   s.length
来源：http://wli.zhengqikj.top

Java: s.length()
来源：http://okm.dashuyun.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cev.zhongyouzk.top

Ruby: s.length
来源：http://hpp.nwbrower.top

C#:   s.Length
来源：http://ska.fktsv.cn

[A23] 大小写转换
来源：http://ahm.cqqwz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://teb.hammf.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qvl.hywenlv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tat.dashuyun.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ycs.chenzaomai.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xus.cqqwz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vpb.vqdsnc.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://xid.cdnleiting.top

C#:   s.ToUpper(); s.ToLower()
来源：http://shx.vehdjk.com

[A24] 去除首尾空白
来源：http://jwx.cqqwz.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qyv.yj20258888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tbv.hesvh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://snl.ctjpmb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jmg.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://imt.jlsjyb.cn

Go:   strings.TrimSpace(s)
来源：http://mzt.snrcjt.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://myh.yfazqb.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qth.jinqigfzy.top

[A25] 字符串比较
来源：http://nkh.hfpthk.cn

Py:   s1 == s2; s1 != s2
来源：http://knz.yueranfly.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mea.52xcode.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kle.vqdsnc.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kbe.vehdjk.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pyb.fktsv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lze.nwbrower.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dkx.ywan-chungtsiang.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jxn.jyoumei.cn

[A26] 类型转换总览
来源：http://gga.yonumen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pha.havefunace.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ayx.hammf.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nka.aizwys.cn

TS:   Number() String() Boolean() x as number
来源：http://adm.cheryme.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fjm.vehdjk.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pvl.jyoumei.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://bgz.xuetiantiany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lif.redwolf501.top

================================================================================
来源：http://hrb.tanke756.top

B. 流程控制
来源：http://zyy.yuxming.cn

================================================================================
来源：http://asy.cucudq.cn

[B01] 条件判断 if / else
来源：http://gcx.hysaishi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yvi.zhongyouzk.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uzn.chenzaomai.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mpq.sxryk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://izm.shuidangran.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://xzc.feifeiyinyue.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nza.andypj.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://gui.cashguo.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://llb.pycfn.com

[B02] 多分支 else if / elif
来源：http://ngf.hammf.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://uve.tian-w.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tkf.xingfuxueyuan.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aah.guannengcc.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xkc.feifeiyinyue.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qjk.tarul.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wxu.yanxiufei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eof.haohaochexian.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wfd.zhijiandao.cn

[B03] switch / match / case
来源：http://vzw.sweek.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ljg.zhoulong.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://dts.aibaodan.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ihc.tian-w.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://neu.yvedp.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://sxy.xuetiantiany.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ghr.epnwcf.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://yvt.cqqwz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lqh.c1oappe.top

[B04] for 计数循环
来源：http://njr.jqgfzy.top

Py:   for i in range(10): print(i)
来源：http://ctd.andypj.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uvz.xuetiantiany.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bii.gzhubu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tfn.uphjek.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rhm.birdmap.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bdd.hnqzz.top

Ruby: 10.times { |i| puts i }
来源：http://tsy.cdnleiting.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ipi.wangshuangyany.cn

[B05] 遍历数组 / 列表
来源：http://gat.shangyingyoupin.top

Py:   for item in arr: print(item)
来源：http://rmq.hongshengwenyu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ihe.jiagoushi.top

JS:   for (const item of arr) { console.log(item); }
来源：http://oui.mhx1999.top

TS:   for (const item of arr) { console.log(item); }
来源：http://jgk.jqgfzy.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://lfr.cashguo.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cam.hesvh.cn

Ruby: arr.each { |item| puts item }
来源：http://xhh.ywan-chungtsiang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wtj.chenzaomai.com

[B06] 遍历字典 / 对象
来源：http://fjc.xuetiantiany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gno.yj20258.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ksl.ehwqpu.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gwm.guowangkeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uvo.hysaishi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vgy.mhx1999.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lup.tanke756.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cnv.wangshuangyany.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dls.xylfe.cn

[B07] while 循环
来源：http://bta.jyoumei.cn

Py:   while i < 10: i += 1
来源：http://ruw.9152youxi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://bpi.shanyushiyangkeji.top

JS:   while (i < 10) { i++; }
来源：http://qsf.xinyue.icu

TS:   while (i < 10) { i++; }
来源：http://wdl.hammf.cn

Java: while (i < 10) { i++; }
来源：http://ynp.redwolf501.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sxt.jyoumei.cn

Ruby: while i < 10; i += 1; end
来源：http://mht.wangdashe.top

C#:   while (i < 10) { i++; }
来源：http://kwn.fktsv.cn

[B08] do-while（至少执行一次）
来源：http://ffk.nanxinkj.top

Py:   # 无 do-while：用 while True + break
来源：http://plg.yongpay.top

PHP:  do { $i++; } while ($i < 10);
来源：http://vqe.cashguo.top

JS:   do { i++; } while (i < 10);
来源：http://coi.sweek.top

TS:   do { i++; } while (i < 10);
来源：http://maj.bjfxy.top

Java: do { i++; } while (i < 10);
来源：http://xyn.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xfj.havefunace.top

Ruby: begin; i += 1; end while i < 10
来源：http://nkd.fanxiaobao.xyz

C#:   do { i++; } while (i < 10);
来源：http://jtx.shangyingyoupin.top

[B09] break 与 continue
来源：http://xsp.yongpay.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qkf.feifeiyinyue.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vtz.zhongyouzk.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://upk.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dpk.tanke756.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tib.bbcook.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ihf.ppjwa.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wam.dashuyun.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zcb.iojbl.cn

[B10] 遍历同时拿索引
来源：http://yoo.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tam.haohaochexian.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vhb.chenjidiqi.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://dyy.gotoacloud.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kim.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ksb.shangyingyoupin.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mum.9152youxi.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dte.redwolf501.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cli.sweek.top

[B11] 生成数字序列 / 区间
来源：http://rws.shzxlz.cn

Py:   list(range(0, 10, 2))
来源：http://mns.yangfankeji.com

PHP:  range(0, 10, 2);
来源：http://wbd.xinyue.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qgu.xylfe.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bwd.wangdashe.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dht.yvedp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cdp.yj202588.top

Ruby: (0...10).step(2).to_a
来源：http://wpy.jiagoushi.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bas.hnxiangtu.top

[B12] 跳出多层循环
来源：http://luy.ppjwa.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://osp.epnwcf.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://rln.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://faj.shanyushiyangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fwj.hnxiangtu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://djc.sjlbkw.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://opz.c1oappe.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xub.yueranfly.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://irw.hysaishi.cn

[B13] 判断是否为数字
来源：http://pzx.chenjidiqi.icu

Py:   isinstance(x, (int, float))
来源：http://xfq.zdbjq.cn

PHP:  is_numeric($x)
来源：http://bfe.vehdjk.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ylb.gotoacloud.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ubg.jqgfzy.top

Java: x instanceof Number
来源：http://xtc.nanxuanxn.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ubs.shanyushiyangkeji.top

Ruby: x.is_a?(Numeric)
来源：http://dwa.nwbrower.top

C#:   x is int or double or decimal
来源：http://dpy.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://zja.shanyushiyangtech.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rup.cashguo.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fvz.9152youxi.cn

JS:   [1, 2, 3].includes(x)
来源：http://wgi.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://pwj.zhongyouzk.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xev.xylfe.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fic.sufxvd.cn

Ruby: [1, 2, 3].include?(x)
来源：http://wth.fktsv.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://swf.sjlbkw.cn

[B15] 布尔运算与取反
来源：http://jfj.gogol.net.cn

Py:   a and b or not c
来源：http://rga.zdbjq.cn

PHP:  $a && $b || !$c
来源：http://ygy.haohaochexian.top

JS:   a && b || !c
来源：http://fya.jlsjyb.cn

TS:   a && b || !c
来源：http://fjs.yj20258.top

Java: a && b || !c
来源：http://myr.shangyingyoupin.top

Go:   a && b || !c
来源：http://aqy.sxryk.cn

Ruby: a && b || !c
来源：http://pda.fanxiaobao.xyz

C#:   a && b || !c
来源：http://bou.haohaochexian.top

[B16] 卫语句：不满足条件提前返回
来源：http://yuk.jqgufenzy.top

Py:   if not data: return
来源：http://alf.hnxiangtu.top

PHP:  if (!$data) { return; }
来源：http://kyz.tanke756.top

JS:   if (!data) return;
来源：http://xtp.zhaomingkeji.xyz

TS:   if (!data) return;
来源：http://dux.jiagoushi.top

Java: if (data == null) return;
来源：http://vke.svipenyu.cn

Go:   if data == nil { return }
来源：http://xat.xuetiantiany.cn

Ruby: return if data.nil?
来源：http://iil.jinqigufen.top

C#:   if (data == null) return;
来源：http://fyk.yuanzhike.top

================================================================================
来源：http://akf.yueranfly.top

C. 函数与作用域
来源：http://rlu.bbcook.cn

================================================================================
来源：http://jlg.zhiwuduotai.top

[C01] 定义函数
来源：http://hwf.daxiang520.top

Py:   def add(a, b): return a + b
来源：http://fjb.ivvv.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kse.yonumen.top

JS:   function add(a, b) { return a + b; }
来源：http://lnw.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mqr.yuxming.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://iyg.mhx1999.top

Go:   func add(a, b int) int { return a + b }
来源：http://zga.svipenyu.cn

Ruby: def add(a, b); a + b; end
来源：http://pqh.gaohongyu789.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jyt.wangdashe.top

[C02] 默认参数
来源：http://vuz.zdqjudy.top

Py:   def greet(name="World"): return name
来源：http://vim.chenjidiqi.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://nzn.shangyingyoupin.top

JS:   function greet(name = "World") { return name; }
来源：http://qnb.aibaodan.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://csm.jinghuilouyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vsd.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://phu.jqgfzy.top

Ruby: def greet(name = "World") = name
来源：http://igf.sjlbkw.cn

C#:   string Greet(string name = "World") => name;
来源：http://iqv.wangshuangyany.cn

[C03] 可变参数
来源：http://gms.zhixingplan.top

Py:   def total(*args): return sum(args)
来源：http://hkk.dashuyun.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fik.hnxiangtu.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mdg.wangshuangyany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kdz.nwbrower.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fgn.nanxuanxn.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ltx.zhijiandao.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xge.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bqd.zhiwuduotai.top

[C04] 命名参数 / 关键字参数
来源：http://sif.hesvh.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lra.haohaochexian.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hdx.gotoacloud.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ddz.mhx1999.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hfo.nanxuanxn.top

Java: // 无：用 Builder 模式或 record
来源：http://xsz.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://vep.zycfv.cn

Ruby: f(a: 1, b: 2)
来源：http://suq.zhongyouzk.top

C#:   f(a: 1, b: 2)
来源：http://smr.mhx1999.top

[C05] 返回多个值
来源：http://zvc.sweek.top

Py:   return a, b
来源：http://lda.fanxiaobao.xyz

PHP:  return [$a, $b];
来源：http://zso.daxiang520.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ver.vqdsnc.cn

TS:   return { a, b };
来源：http://byr.tanke756.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hft.feifeiyinyue.top

Go:   return a, b
来源：http://gir.nanxuanxn.top

Ruby: return a, b
来源：http://ddp.nanxuanxn.top

C#:   return (a, b);              // ValueTuple
来源：http://qyw.zdbjq.cn

[C06] 匿名函数 / lambda
来源：http://fvq.yj20258888.top

Py:   square = lambda x: x * x
来源：http://vmx.pycfn.com

PHP:  $square = fn($x) => $x * $x;
来源：http://wal.aizwys.cn

JS:   const square = x => x * x;
来源：http://nkf.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://dpl.sweek.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ncd.tanke756.top

Go:   sq := func(x int) int { return x * x }
来源：http://rdu.jiagoushi.top

Ruby: square = ->(x) { x * x }
来源：http://cdj.pengpengdd.cyou

C#:   Func<int, int> square = x => x * x;
来源：http://inz.jqgufenzy.top

[C07] 把函数作为参数传入
来源：http://ery.zdqjudy.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://spr.cashguo.top

PHP:  array_map("strtoupper", $arr);
来源：http://jng.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ccb.yueranfly.top

TS:   arr.map(String)
来源：http://cga.guannengcc.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vze.fengsongda.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://gjj.quarkkingdee.top

Ruby: arr.map(&:upcase)
来源：http://dzi.zhoulong.xyz

C#:   arr.Select(s => s.ToUpper())
来源：http://ydu.feifeiyinyue.top

[C08] 闭包
来源：http://dzz.wangdashe.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bru.hfpthk.cn


<!-- 参考信息 -->