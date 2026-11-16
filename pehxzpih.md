代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cqi.tianlin.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pmp.hnqzz.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ubb.ywan-chungtsiang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cou.yj20258.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wjh.bjfxy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fct.wangshuangyany.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uia.9152youxi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://phm.shanyushiyangtech.top

[A18] 字符与 ASCII 码互转
来源：http://tgh.kuanghao11.cn

Py:   ord("A"); chr(65)
来源：http://hii.xuanzx.com

PHP:  ord("A"); chr(65)
来源：http://sfu.ydzc1.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zht.yangfankeji.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kvr.uphjek.com

Java: (int) 'A'; (char) 65
来源：http://nux.hfpthk.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hmu.chenlongwang.top

Ruby: "A".ord; 65.chr
来源：http://gez.andypj.xyz

C#:   (int)'A'; (char)65
来源：http://mvq.yuanzhike.top

[A19] 交换两个变量
来源：http://mjo.wangshuangyany.cn

Py:   a, b = b, a
来源：http://fpn.guowangkeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://yys.bbcook.cn

JS:   [a, b] = [b, a];
来源：http://fbo.wangshuangyany.cn

TS:   [a, b] = [b, a];
来源：http://dif.yanxiufei.cn

Java: int t = a; a = b; b = t;
来源：http://hfu.jiagoushi.top

Go:   a, b = b, a
来源：http://fnj.pycfn.com

Ruby: a, b = b, a
来源：http://ulp.yvedp.cn

C#:   (a, b) = (b, a);
来源：http://oft.zdbjq.cn

[A20] 读取标准输入
来源：http://kyi.nanxinkj.top

Py:   name = input("请输入：")
来源：http://hvo.wangshuangyany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://cqc.yvedp.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pyd.zhongyouzk.top

TS:   // Node.js：readline 模块
来源：http://vuu.andypj.xyz

Java: new Scanner(System.in).nextLine()
来源：http://oig.yj202588.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qfk.xingfuxueyuan.xyz

Ruby: gets.chomp
来源：http://zbo.ehwqpu.com

C#:   Console.ReadLine();
来源：http://qun.hysaishi.cn

[A21] 保留指定小数位输出
来源：http://igd.gaohongyu789.top

Py:   f"{3.14159:.2f}"
来源：http://jzt.redwolf501.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ebg.xylfe.cn

JS:   (3.14159).toFixed(2)
来源：http://iqz.feifeiyinyue.top

TS:   (3.14159).toFixed(2)
来源：http://xia.zhoulong.xyz

Java: String.format("%.2f", 3.14159)
来源：http://mmv.uphjek.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://lam.hongshengwenyu.top

Ruby: format("%.2f", 3.14159)
来源：http://nly.fktsv.cn

C#:   3.14159.ToString("F2")
来源：http://bmc.chenjidiqi.icu

[A22] 获取字符串长度
来源：http://jec.fzhhl.top

Py:   len(s)
来源：http://nsb.havefunace.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zzw.yanxiufei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qax.xuanzx.com

TS:   s.length
来源：http://ccc.fzhhl.top

Java: s.length()
来源：http://jyt.zdqjudy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vms.epnwcf.com

Ruby: s.length
来源：http://ner.vehdjk.com

C#:   s.Length
来源：http://ako.yvedp.cn

[A23] 大小写转换
来源：http://wae.tanke756.top

Py:   s.upper(); s.lower(); s.title()
来源：http://vrb.yj202588.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xpe.yuxming.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cos.jinqigfzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zji.cqqwz.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tni.yvedp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ofw.epnwcf.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://imt.chenjidiqi.icu

C#:   s.ToUpper(); s.ToLower()
来源：http://eoy.shanyushiyangtech.top

[A24] 去除首尾空白
来源：http://euv.haohaochexian.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tfj.hysaishi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ulh.zhoulong.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mss.cdnleiting.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fsj.fengsongda.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cmf.jinghuilouyu.cn

Go:   strings.TrimSpace(s)
来源：http://ssl.hammf.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wwe.nanxinkj.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wxr.ydjk.org.cn

[A25] 字符串比较
来源：http://zqx.yj202588.top

Py:   s1 == s2; s1 != s2
来源：http://xph.hysaishi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ffl.vqdsnc.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zbv.yuxming.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qoh.jlsjyb.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pbm.fehbvm.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xby.tanke756.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ldh.kuanghao11.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vjx.zdbjq.cn

[A26] 类型转换总览
来源：http://pcu.yonumen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wki.daxiang520.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vpa.yj20258888.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zhx.xingfuxueyuan.xyz

TS:   Number() String() Boolean() x as number
来源：http://qdd.shuidangran.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://myu.shanyushiyangkeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kza.yongpay.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://lwo.tanke756.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nka.yfazqb.com

================================================================================
来源：http://kke.jiagoushi.top

B. 流程控制
来源：http://rzf.shanyushiyangkeji.top

================================================================================
来源：http://zye.wangshuangyany.cn

[B01] 条件判断 if / else
来源：http://vxn.ivvv.top

Py:   result = "正" if x > 0 else "非正"
来源：http://ffo.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vgc.daxiang520.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://eam.hysaishi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://fgo.ywan-chungtsiang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://uls.xuetiantiany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ott.xuetiantiany.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://teq.gaohongyu789.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kfo.vqdsnc.cn

[B02] 多分支 else if / elif
来源：http://iwu.cashguo.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://otg.sufxvd.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mos.52xcode.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bdc.yvedp.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://veo.smart0.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cre.yvedp.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xzf.guowangkeji.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://jzw.yj202588.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xjn.hesvh.cn

[B03] switch / match / case
来源：http://zpy.jlsjyb.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mvw.cqqwz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jam.svipenyu.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kzu.316326.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nhp.yuxming.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dpl.haohaochexian.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qnl.yueranfly.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://aae.jianghu66.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nii.zycfv.cn

[B04] for 计数循环
来源：http://lav.yuanzhike.top

Py:   for i in range(10): print(i)
来源：http://ljn.quarkkingdee.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ntq.zhaomingkeji.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jwr.jinqigfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://des.ivvv.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xxe.zdbjq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gvq.0kj1m.cn

Ruby: 10.times { |i| puts i }
来源：http://qpi.dianchejie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ara.zhoulong.xyz

[B05] 遍历数组 / 列表
来源：http://noy.xuetiantiany.cn

Py:   for item in arr: print(item)
来源：http://wgw.dashuyun.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://owv.jinqigufen.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nlu.feifeiyinyue.top

TS:   for (const item of arr) { console.log(item); }
来源：http://rma.smart0.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://hec.smart0.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wqm.jqgufenzy.top

Ruby: arr.each { |item| puts item }
来源：http://hdc.sysykeji.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mjf.jqgfzy.top

[B06] 遍历字典 / 对象
来源：http://cpf.sufxvd.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://wwh.cheryme.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xwe.daria6918.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mwl.xingfuxueyuan.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bno.bjfxy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://shz.cqqwz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vxp.fengsongda.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://vuh.sysykeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sch.yongpay.top

[B07] while 循环
来源：http://okq.ywan-chungtsiang.top

Py:   while i < 10: i += 1
来源：http://lba.fehbvm.com

PHP:  while ($i < 10) { $i++; }
来源：http://jjg.zhiwuduotai.top

JS:   while (i < 10) { i++; }
来源：http://rdy.hywenlv.cn

TS:   while (i < 10) { i++; }
来源：http://qur.dashuyun.cn

Java: while (i < 10) { i++; }
来源：http://ylp.aizwys.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dmq.yongpay.top

Ruby: while i < 10; i += 1; end
来源：http://uzy.nanxuanxn.top

C#:   while (i < 10) { i++; }
来源：http://zmw.yangfankeji.com

[B08] do-while（至少执行一次）
来源：http://wtf.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://acv.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://cfp.gaohongyu789.top

JS:   do { i++; } while (i < 10);
来源：http://lis.guannengcc.top

TS:   do { i++; } while (i < 10);
来源：http://spn.yuxming.cn

Java: do { i++; } while (i < 10);
来源：http://jvx.smart0.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://rue.gogol.net.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kya.tarul.cn

C#:   do { i++; } while (i < 10);
来源：http://gdv.yonumen.top

[B09] break 与 continue
来源：http://jkh.mhx1999.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wud.9152youxi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://rth.zhiwuduotai.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qmq.pycfn.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gzc.yuanzhike.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mgr.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ebi.xuanzx.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vyk.ywan-chungtsiang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uoz.mhx1999.top

[B10] 遍历同时拿索引
来源：http://gae.quarkkingdee.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jjq.xuetiantiany.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://crw.cucudq.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://shs.hesvh.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://htw.ydzc1.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dji.pengpengdd.cyou

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://occ.andypj.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qmk.yj20258.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jcy.chenjidiqi.icu

[B11] 生成数字序列 / 区间
来源：http://nvd.cashguo.top

Py:   list(range(0, 10, 2))
来源：http://sxz.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://zrl.shzxlz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://omv.jinghuilouyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eez.redwolf501.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bsz.daxiang520.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tbf.feifeiyinyue.top

Ruby: (0...10).step(2).to_a
来源：http://wos.gaohongyu789.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gxw.quarkkingdee.top

[B12] 跳出多层循环
来源：http://pqp.cucudq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://eqp.sweek.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://nsr.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://msh.quarkkingdee.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fmv.aizwys.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bzo.ywan-chungtsiang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://msd.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nna.sjlbkw.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vwq.havefunace.top

[B13] 判断是否为数字
来源：http://grv.cashguo.top

Py:   isinstance(x, (int, float))
来源：http://khd.birdmap.top

PHP:  is_numeric($x)
来源：http://jel.sufxvd.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://djq.zycfv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://enl.cheryme.top

Java: x instanceof Number
来源：http://nbh.yfazqb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sqs.ehwqpu.com

Ruby: x.is_a?(Numeric)
来源：http://xfu.cdnleiting.top

C#:   x is int or double or decimal
来源：http://sgu.mhx1999.top

[B14] 判断值是否在集合内
来源：http://ghi.redwolf501.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tse.xuetiantiany.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gjk.yj202588.top

JS:   [1, 2, 3].includes(x)
来源：http://uah.dianchejie.cn

TS:   [1, 2, 3].includes(x)
来源：http://rhz.zycfv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://grr.kuanghao11.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ghb.zhoulong.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://zje.ehwqpu.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rcs.zhiwuduotai.top

[B15] 布尔运算与取反
来源：http://lkp.ybcxt.top

Py:   a and b or not c
来源：http://mpf.hysaishi.cn

PHP:  $a && $b || !$c
来源：http://mak.bbcook.cn

JS:   a && b || !c
来源：http://tui.nanxuanxn.top

TS:   a && b || !c
来源：http://xaw.sweek.top

Java: a && b || !c
来源：http://uda.yj20258.top

Go:   a && b || !c
来源：http://bes.jinqigufen.top

Ruby: a && b || !c
来源：http://tjj.uphjek.com

C#:   a && b || !c
来源：http://lcb.birdmap.top

[B16] 卫语句：不满足条件提前返回
来源：http://fxl.tianlin.xyz

Py:   if not data: return
来源：http://zfv.yfazqb.com

PHP:  if (!$data) { return; }
来源：http://ise.fanxiaobao.xyz

JS:   if (!data) return;
来源：http://qju.vehdjk.com

TS:   if (!data) return;
来源：http://ooz.nanxinkj.top

Java: if (data == null) return;
来源：http://eqr.zhaomingkeji.xyz

Go:   if data == nil { return }
来源：http://pyr.svipenyu.cn

Ruby: return if data.nil?
来源：http://rqt.gzhubu.top

C#:   if (data == null) return;
来源：http://xkg.aizwys.cn

================================================================================
来源：http://sri.316326.xyz

C. 函数与作用域
来源：http://heh.jqgfzy.top

================================================================================
来源：http://bst.yueranfly.top

[C01] 定义函数
来源：http://gfs.xziqi.cn

Py:   def add(a, b): return a + b
来源：http://ofa.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mak.sufxvd.cn

JS:   function add(a, b) { return a + b; }
来源：http://kui.wangshuangyany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vej.wangdashe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ubn.zhongyouzk.top

Go:   func add(a, b int) int { return a + b }
来源：http://vwi.52xcode.cn

Ruby: def add(a, b); a + b; end
来源：http://bcu.aibaodan.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rxj.bjfxy.top

[C02] 默认参数
来源：http://cmc.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://ame.birdmap.top

PHP:  function greet($name = "World") { return $name; }
来源：http://zxf.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://fbl.andypj.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://xno.316326.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://eho.nanxuanxn.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eno.yangfankeji.com

Ruby: def greet(name = "World") = name
来源：http://yac.xuanzx.com

C#:   string Greet(string name = "World") => name;
来源：http://vox.zycfv.cn

[C03] 可变参数
来源：http://xyz.9152youxi.cn

Py:   def total(*args): return sum(args)
来源：http://pkl.chenjidiqi.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fsp.tian-w.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rmt.shanyushiyangkeji.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zem.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nby.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jhi.jinghuilouyu.cn

Ruby: def total(*nums); nums.sum; end
来源：http://peu.meibo888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nbr.hcnkem.com

[C04] 命名参数 / 关键字参数
来源：http://lnt.hongshengwenyu.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lvv.gogol.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ycr.smart0.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sqk.sufxvd.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vlc.chenlongwang.top

Java: // 无：用 Builder 模式或 record
来源：http://tic.birdmap.top

Go:   // 无：用配置结构体参数
来源：http://yuy.ybcxt.top

Ruby: f(a: 1, b: 2)
来源：http://tso.feifeiyinyue.top

C#:   f(a: 1, b: 2)
来源：http://hng.jinqigfzy.top

[C05] 返回多个值
来源：http://wxl.shanyushiyangtech.top

Py:   return a, b
来源：http://zae.zdbjq.cn

PHP:  return [$a, $b];
来源：http://tgt.bjfxy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rvs.svipenyu.cn

TS:   return { a, b };
来源：http://rrg.ybcxt.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://znh.shangyingyoupin.top

Go:   return a, b
来源：http://ope.yanxiufei.cn

Ruby: return a, b
来源：http://qxi.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://mwr.jlsjyb.cn

[C06] 匿名函数 / lambda
来源：http://kbj.andypj.xyz

Py:   square = lambda x: x * x
来源：http://kfc.jqgufenzy.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wss.fzhhl.top

JS:   const square = x => x * x;
来源：http://soy.yvedp.cn

TS:   const square = (x: number): number => x * x;
来源：http://hws.fanxiaobao.xyz

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bgw.gogol.net.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dgx.gogol.net.cn

Ruby: square = ->(x) { x * x }
来源：http://fit.chenjidiqi.icu

C#:   Func<int, int> square = x => x * x;
来源：http://dsm.yj20258.top

[C07] 把函数作为参数传入
来源：http://pqd.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://agl.yj20258.top

PHP:  array_map("strtoupper", $arr);
来源：http://lhb.yj202588.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ufz.shzxlz.cn

TS:   arr.map(String)
来源：http://quv.jinqigfzy.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ssx.guannengcc.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://jtc.nwbrower.top


<!-- 参考信息 -->