代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nnl.yangfankeji.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uts.wangdashe.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ddc.aibaodan.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://pmu.yueranfly.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qck.chenlongwang.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dco.hnqzz.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cha.havefunace.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vak.shuidangran.top

[A18] 字符与 ASCII 码互转
来源：http://bto.fktsv.cn

Py:   ord("A"); chr(65)
来源：http://woi.xuetiantiany.cn

PHP:  ord("A"); chr(65)
来源：http://fim.ivvv.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mdc.vehdjk.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rcn.wangdashe.top

Java: (int) 'A'; (char) 65
来源：http://cvq.yj20258888.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jzz.chenjidiqi.icu

Ruby: "A".ord; 65.chr
来源：http://umr.fengsongda.top

C#:   (int)'A'; (char)65
来源：http://lpk.jqgufenzy.top

[A19] 交换两个变量
来源：http://ikf.ydzc1.top

Py:   a, b = b, a
来源：http://yyc.xinyue.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://nwp.jqgufenzy.top

JS:   [a, b] = [b, a];
来源：http://zdo.shangyingyoupin.top

TS:   [a, b] = [b, a];
来源：http://bzy.316326.xyz

Java: int t = a; a = b; b = t;
来源：http://eut.fzhhl.top

Go:   a, b = b, a
来源：http://mbz.fehbvm.com

Ruby: a, b = b, a
来源：http://wio.yvedp.cn

C#:   (a, b) = (b, a);
来源：http://msw.ywan-chungtsiang.top

[A20] 读取标准输入
来源：http://uhb.hammf.cn

Py:   name = input("请输入：")
来源：http://jjj.kuanghao11.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rgj.nanxuanxn.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hfg.yongpay.top

TS:   // Node.js：readline 模块
来源：http://xbn.shanyushiyangtech.top

Java: new Scanner(System.in).nextLine()
来源：http://ilc.zycfv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hue.yj20258888.top

Ruby: gets.chomp
来源：http://dtu.jinghuilouyu.cn

C#:   Console.ReadLine();
来源：http://zbi.tarul.cn

[A21] 保留指定小数位输出
来源：http://bfj.zhengqikj.top

Py:   f"{3.14159:.2f}"
来源：http://azo.0kj1m.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ofo.hywenlv.cn

JS:   (3.14159).toFixed(2)
来源：http://psd.yuanzhike.top

TS:   (3.14159).toFixed(2)
来源：http://sqx.shanyushiyangkeji.top

Java: String.format("%.2f", 3.14159)
来源：http://wrp.snrcjt.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://tyl.sysykeji.top

Ruby: format("%.2f", 3.14159)
来源：http://idq.ywan-chungtsiang.top

C#:   3.14159.ToString("F2")
来源：http://ftv.zhengqikj.top

[A22] 获取字符串长度
来源：http://swd.sysykeji.top

Py:   len(s)
来源：http://loj.pengpengdd.cyou

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://cwr.zhixingplan.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hhl.snrcjt.cn

TS:   s.length
来源：http://tgo.hcnkem.com

Java: s.length()
来源：http://ils.ydjk.org.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dvb.smart0.xyz

Ruby: s.length
来源：http://srb.cqqwz.cn

C#:   s.Length
来源：http://ncv.tian-w.cn

[A23] 大小写转换
来源：http://uyu.yanxiufei.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ino.jqgfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mol.nanxinkj.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jbl.hongshengwenyu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qer.yonumen.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lpj.havefunace.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://cyt.redwolf501.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qkq.aizwys.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ikb.zdbjq.cn

[A24] 去除首尾空白
来源：http://fob.haohaochexian.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://liu.shuidangran.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mbh.fktsv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ypc.smart0.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wda.yuxming.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ari.zhoulong.xyz

Go:   strings.TrimSpace(s)
来源：http://jth.bbcook.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sfd.yuxming.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hzb.snrcjt.cn

[A25] 字符串比较
来源：http://sxx.hfpthk.cn

Py:   s1 == s2; s1 != s2
来源：http://qmo.snrcjt.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xwm.mhx1999.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://drw.aizwys.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ycv.fanxiaobao.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://eke.hfpthk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ucs.jinqigfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xnw.sxryk.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cdg.dianchejie.cn

[A26] 类型转换总览
来源：http://slc.tarul.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tyu.aizwys.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rzp.tarul.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zpl.zhongyouzk.top

TS:   Number() String() Boolean() x as number
来源：http://puo.iojbl.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sfb.iojbl.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://iwg.bbcook.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://mox.guannengcc.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nrr.hcnkem.com

================================================================================
来源：http://tki.ydzc1.top

B. 流程控制
来源：http://pzx.fzhhl.top

================================================================================
来源：http://iai.smart0.xyz

[B01] 条件判断 if / else
来源：http://bhg.daxiang520.top

Py:   result = "正" if x > 0 else "非正"
来源：http://skj.nanxinkj.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qzr.0kj1m.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jch.ydjk.org.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cjh.chenlongwang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://adt.hammf.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nfy.yuanzhike.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jsp.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://umk.yj20258888.top

[B02] 多分支 else if / elif
来源：http://klh.ppjwa.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hxk.yongpay.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xhh.yj202588.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rho.chenjidiqi.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xiz.jinqigufen.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://djm.aibaodan.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lnz.snrcjt.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://amy.feifeiyinyue.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dqq.yvedp.cn

[B03] switch / match / case
来源：http://kcj.fzhhl.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://pxb.xingfuxueyuan.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iat.cqqwz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://che.birdmap.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rjn.feifeiyinyue.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gso.hongshengwenyu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://olk.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://akx.jqgufenzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fnt.jinghuilouyu.cn

[B04] for 计数循环
来源：http://hym.svipenyu.cn

Py:   for i in range(10): print(i)
来源：http://zoi.cqqwz.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xfz.sjlbkw.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hhi.jinqigfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://llu.jinqigufen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://utu.pycfn.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://uzj.sxryk.cn

Ruby: 10.times { |i| puts i }
来源：http://fqu.zhaomingkeji.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jep.uphjek.com

[B05] 遍历数组 / 列表
来源：http://ppy.zhoulong.xyz

Py:   for item in arr: print(item)
来源：http://why.zhaomingkeji.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kie.gzhubu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ylb.jlsjyb.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://loq.vqdsnc.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wyr.chenlongwang.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ogq.yanxiufei.cn

Ruby: arr.each { |item| puts item }
来源：http://lnh.jqgfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oxi.nanxinkj.top

[B06] 遍历字典 / 对象
来源：http://abk.shanyushiyangkeji.top

Py:   for k, v in d.items(): print(k, v)
来源：http://syw.tian-w.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ami.hammf.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ael.smart0.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zwr.xinyue.icu

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kug.hfpthk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rtj.hammf.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://yqs.cheryme.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://iow.ppjwa.cn

[B07] while 循环
来源：http://cew.cqqwz.cn

Py:   while i < 10: i += 1
来源：http://hzz.ydzc1.top

PHP:  while ($i < 10) { $i++; }
来源：http://dlb.fanxiaobao.xyz

JS:   while (i < 10) { i++; }
来源：http://pek.jiagoushi.top

TS:   while (i < 10) { i++; }
来源：http://cie.tarul.cn

Java: while (i < 10) { i++; }
来源：http://gxw.wangdashe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wwf.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://zet.jinqigfzy.top

C#:   while (i < 10) { i++; }
来源：http://vqc.jyoumei.cn

[B08] do-while（至少执行一次）
来源：http://xqd.yj20258888.top

Py:   # 无 do-while：用 while True + break
来源：http://dfr.chenzaomai.com

PHP:  do { $i++; } while ($i < 10);
来源：http://grt.jlsjyb.cn

JS:   do { i++; } while (i < 10);
来源：http://zig.zycfv.cn

TS:   do { i++; } while (i < 10);
来源：http://zuj.yfazqb.com

Java: do { i++; } while (i < 10);
来源：http://jwz.fengsongda.top

Go:   for { i++; if i >= 10 { break } }
来源：http://toj.sufxvd.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ehk.fehbvm.com

C#:   do { i++; } while (i < 10);
来源：http://kpz.zhengqikj.top

[B09] break 与 continue
来源：http://lkf.gaohongyu789.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://udf.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pkz.quarkkingdee.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fmz.andypj.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pyk.fengsongda.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nuz.svipenyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xkc.wangshuangyany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ydx.bjfxy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kbg.aibaodan.cn

[B10] 遍历同时拿索引
来源：http://jnd.jinyuanbaomall.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wvq.cucudq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://btd.wangshuangyany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rsb.cucudq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://clz.daria6918.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jzw.zhiwuduotai.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ash.xinyue.icu

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lkw.chenjidiqi.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ltv.gzhubu.top

[B11] 生成数字序列 / 区间
来源：http://ddx.bbcook.cn

Py:   list(range(0, 10, 2))
来源：http://oec.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://skb.hfpthk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bhj.birdmap.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qka.yj202588.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://oan.dashuyun.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mdh.yj20258.top

Ruby: (0...10).step(2).to_a
来源：http://ply.uphjek.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nox.nwbrower.top

[B12] 跳出多层循环
来源：http://dkc.hnxiangtu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://dfs.yangfankeji.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://vkc.jiagoushi.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://cut.fengsongda.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lws.gogol.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zob.svipenyu.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ejf.shanyushiyangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wvm.jinqigufen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://sqi.uphjek.com

[B13] 判断是否为数字
来源：http://eyr.aizwys.cn

Py:   isinstance(x, (int, float))
来源：http://xim.feifeiyinyue.top

PHP:  is_numeric($x)
来源：http://clh.epnwcf.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qwn.yanxiufei.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hub.zdbjq.cn

Java: x instanceof Number
来源：http://xal.gogol.net.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tbe.ehwqpu.com

Ruby: x.is_a?(Numeric)
来源：http://nuk.gaohongyu789.top

C#:   x is int or double or decimal
来源：http://hqq.fengsongda.top

[B14] 判断值是否在集合内
来源：http://ler.xinyue.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://pvm.fzhhl.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lyo.jinqigfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://smf.xingfuxueyuan.xyz

TS:   [1, 2, 3].includes(x)
来源：http://aen.jianghu66.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mwg.chenlongwang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://xkx.yvedp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://fcz.xingfuxueyuan.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://efp.bbcook.cn

[B15] 布尔运算与取反
来源：http://ync.snrcjt.cn

Py:   a and b or not c
来源：http://ppv.ydzc1.top

PHP:  $a && $b || !$c
来源：http://sbk.wangdashe.top

JS:   a && b || !c
来源：http://tfm.yfazqb.com

TS:   a && b || !c
来源：http://clz.xziqi.cn

Java: a && b || !c
来源：http://yus.havefunace.top

Go:   a && b || !c
来源：http://xvl.ehwqpu.com

Ruby: a && b || !c
来源：http://kym.hysaishi.cn

C#:   a && b || !c
来源：http://sep.sxryk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://xdd.fktsv.cn

Py:   if not data: return
来源：http://tmr.gotoacloud.top

PHP:  if (!$data) { return; }
来源：http://tiu.cheryme.top

JS:   if (!data) return;
来源：http://gtf.wangdashe.top

TS:   if (!data) return;
来源：http://sqo.yj20258.top

Java: if (data == null) return;
来源：http://tar.pengpengdd.cyou

Go:   if data == nil { return }
来源：http://pda.0kj1m.cn

Ruby: return if data.nil?
来源：http://gmb.ydjk.org.cn

C#:   if (data == null) return;
来源：http://zgu.guowangkeji.top

================================================================================
来源：http://rzx.gaohongyu789.top

C. 函数与作用域
来源：http://fbx.zhongyouzk.top

================================================================================
来源：http://wpm.zhijiandao.cn

[C01] 定义函数
来源：http://phf.52xcode.cn

Py:   def add(a, b): return a + b
来源：http://obc.yuanzhike.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hbb.sweek.top

JS:   function add(a, b) { return a + b; }
来源：http://fgn.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zgm.nanxuanxn.top

Java: static int add(int a, int b) { return a + b; }
来源：http://lvx.hfpthk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://bbb.ivvv.top

Ruby: def add(a, b); a + b; end
来源：http://pbn.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://dzz.hcnkem.com

[C02] 默认参数
来源：http://lkc.yongpay.top

Py:   def greet(name="World"): return name
来源：http://cks.birdmap.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lwl.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://jnd.hnqzz.top

TS:   function greet(name: string = "World") { return name; }
来源：http://brv.yuxming.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xby.redwolf501.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pkx.cdnleiting.top

Ruby: def greet(name = "World") = name
来源：http://prn.cashguo.top

C#:   string Greet(string name = "World") => name;
来源：http://dmh.hywenlv.cn

[C03] 可变参数
来源：http://rle.birdmap.top

Py:   def total(*args): return sum(args)
来源：http://flg.tarul.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gqu.fktsv.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pxc.hysaishi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vdd.jianghu66.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rzi.sufxvd.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://eay.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://rgn.xinyue.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://otx.0kj1m.cn

[C04] 命名参数 / 关键字参数
来源：http://rwr.zhaomingkeji.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rew.zhiwuduotai.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rjx.jianghu66.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nqn.shanyushiyangtech.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ydt.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://avu.tianlin.xyz

Go:   // 无：用配置结构体参数
来源：http://xju.yonumen.top

Ruby: f(a: 1, b: 2)
来源：http://vbu.zhengqikj.top

C#:   f(a: 1, b: 2)
来源：http://fdf.zdqjudy.top

[C05] 返回多个值
来源：http://rva.shuidangran.top

Py:   return a, b
来源：http://tez.redwolf501.top

PHP:  return [$a, $b];
来源：http://wxj.yanxiufei.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://byc.yj20258.top

TS:   return { a, b };
来源：http://vvu.meibo888.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://onm.gzhubu.top

Go:   return a, b
来源：http://skx.andypj.xyz

Ruby: return a, b
来源：http://wlm.ydzc1.top

C#:   return (a, b);              // ValueTuple
来源：http://yac.yj20258888.top

[C06] 匿名函数 / lambda
来源：http://nua.zhoulong.xyz

Py:   square = lambda x: x * x
来源：http://jjh.ydjk.org.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hhv.sweek.top

JS:   const square = x => x * x;
来源：http://vvd.tian-w.cn

TS:   const square = (x: number): number => x * x;
来源：http://vse.chenjidiqi.icu

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://kut.ehwqpu.com

Go:   sq := func(x int) int { return x * x }
来源：http://ixm.guowangkeji.top

Ruby: square = ->(x) { x * x }
来源：http://ftt.ctjpmb.com

C#:   Func<int, int> square = x => x * x;
来源：http://mux.yj20258888.top

[C07] 把函数作为参数传入
来源：http://kze.cdnleiting.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gsn.pycfn.com

PHP:  array_map("strtoupper", $arr);
来源：http://tcz.xingfuxueyuan.xyz

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fmz.hywenlv.cn

TS:   arr.map(String)
来源：http://ars.redwolf501.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://owd.sweek.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://xwj.tian-w.cn


<!-- 参考信息 -->