代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wml.yanxiufei.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://cbt.hesvh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vzk.xingfuxueyuan.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vgl.hongshengwenyu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://abi.52xcode.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qyl.ctjpmb.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ybi.fehbvm.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fve.xuanzx.com

[A18] 字符与 ASCII 码互转
来源：http://xql.hnqzz.top

Py:   ord("A"); chr(65)
来源：http://yvw.jinqigufen.top

PHP:  ord("A"); chr(65)
来源：http://tsc.gogol.net.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://twg.cucudq.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mvh.yvedp.cn

Java: (int) 'A'; (char) 65
来源：http://xbm.0kj1m.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fra.jqgufenzy.top

Ruby: "A".ord; 65.chr
来源：http://isr.daxiang520.top

C#:   (int)'A'; (char)65
来源：http://fxd.hfpthk.cn

[A19] 交换两个变量
来源：http://toa.vehdjk.com

Py:   a, b = b, a
来源：http://ptg.xuetiantiany.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://gaa.shuidangran.top

JS:   [a, b] = [b, a];
来源：http://pgf.nanxuanxn.top

TS:   [a, b] = [b, a];
来源：http://ksl.cucudq.cn

Java: int t = a; a = b; b = t;
来源：http://arn.meibo888.top

Go:   a, b = b, a
来源：http://msf.shanyushiyangtech.top

Ruby: a, b = b, a
来源：http://bbp.gzhubu.top

C#:   (a, b) = (b, a);
来源：http://uaj.havefunace.top

[A20] 读取标准输入
来源：http://epk.yj20258.top

Py:   name = input("请输入：")
来源：http://rlf.c1oappe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://qxo.yuanzhike.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ujl.xziqi.cn

TS:   // Node.js：readline 模块
来源：http://del.sweek.top

Java: new Scanner(System.in).nextLine()
来源：http://xli.zdbjq.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hms.zhiwuduotai.top

Ruby: gets.chomp
来源：http://bsy.ybcxt.top

C#:   Console.ReadLine();
来源：http://piw.ydjk.org.cn

[A21] 保留指定小数位输出
来源：http://fdg.jqgfzy.top

Py:   f"{3.14159:.2f}"
来源：http://tmj.hysaishi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jif.guannengcc.top

JS:   (3.14159).toFixed(2)
来源：http://zqk.yj20258888.top

TS:   (3.14159).toFixed(2)
来源：http://izz.jinqigfzy.top

Java: String.format("%.2f", 3.14159)
来源：http://ccr.yvedp.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nzc.zhijiandao.cn

Ruby: format("%.2f", 3.14159)
来源：http://ctj.tanke756.top

C#:   3.14159.ToString("F2")
来源：http://hbl.ydjk.org.cn

[A22] 获取字符串长度
来源：http://kyx.daria6918.cn

Py:   len(s)
来源：http://usy.wangdashe.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fwf.ydjk.org.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zrf.c1oappe.top

TS:   s.length
来源：http://zit.fehbvm.com

Java: s.length()
来源：http://zmq.yueranfly.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fzv.zhaomingkeji.xyz

Ruby: s.length
来源：http://rvf.shzxlz.cn

C#:   s.Length
来源：http://tgi.fzhhl.top

[A23] 大小写转换
来源：http://xec.cdnleiting.top

Py:   s.upper(); s.lower(); s.title()
来源：http://qfj.shuidangran.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uak.gaohongyu789.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sik.52xcode.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nyh.svipenyu.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://foi.xinyue.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ihn.guannengcc.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fcq.snrcjt.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://ige.jinqigufen.top

[A24] 去除首尾空白
来源：http://dpw.fanxiaobao.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rig.yuxming.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gir.wangshuangyany.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jdi.ydjk.org.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ika.ehwqpu.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://old.ehwqpu.com

Go:   strings.TrimSpace(s)
来源：http://vro.zhoulong.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qsj.jyoumei.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hbq.zhoulong.xyz

[A25] 字符串比较
来源：http://llq.yongpay.top

Py:   s1 == s2; s1 != s2
来源：http://bve.sweek.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zar.yvedp.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://udv.yj20258.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jcu.hammf.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nvn.nanxinkj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vgz.shanyushiyangtech.top

Ruby: s1 == s2; s1 <=> s2
来源：http://lye.jinqigfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uzf.0kj1m.cn

[A26] 类型转换总览
来源：http://dsq.bjfxy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ixj.tianlin.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kvj.jinyuanbaomall.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oxx.yangfankeji.com

TS:   Number() String() Boolean() x as number
来源：http://mgv.fehbvm.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://coe.mhx1999.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mrl.chenzaomai.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://blz.fengsongda.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uir.zhijiandao.cn

================================================================================
来源：http://zwb.sufxvd.cn

B. 流程控制
来源：http://nmf.yfazqb.com

================================================================================
来源：http://tzn.xylfe.cn

[B01] 条件判断 if / else
来源：http://koq.guowangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tkz.jianghu66.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zaj.jlsjyb.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xql.yj202588.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tod.chenjidiqi.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://uxq.andypj.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jcs.chenlongwang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xws.hcnkem.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kgt.andypj.xyz

[B02] 多分支 else if / elif
来源：http://ope.sweek.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aeg.ydjk.org.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rzn.hongshengwenyu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://svy.guowangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://klr.nanxuanxn.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jmg.hammf.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dsu.fzhhl.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://qdz.kuanghao11.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zld.andypj.xyz

[B03] switch / match / case
来源：http://vts.guowangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ico.zycfv.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aex.hongshengwenyu.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hmt.ctjpmb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://miy.epnwcf.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hgc.ehwqpu.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mhm.daria6918.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://oss.wangshuangyany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sza.hcnkem.com

[B04] for 计数循环
来源：http://zmd.hfpthk.cn

Py:   for i in range(10): print(i)
来源：http://hmp.feifeiyinyue.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gvn.shanyushiyangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hnf.yuanzhike.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xkk.cqqwz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://etw.hywenlv.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zqz.xuetiantiany.cn

Ruby: 10.times { |i| puts i }
来源：http://lth.cheryme.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gjs.ydjk.org.cn

[B05] 遍历数组 / 列表
来源：http://azt.jyoumei.cn

Py:   for item in arr: print(item)
来源：http://jhz.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://owt.hesvh.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xvg.chenlongwang.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qbb.ehwqpu.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ysj.svipenyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xix.ywan-chungtsiang.top

Ruby: arr.each { |item| puts item }
来源：http://yhm.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qul.cheryme.top

[B06] 遍历字典 / 对象
来源：http://zis.iojbl.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mxq.xinyue.icu

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mpi.ehwqpu.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nqs.andypj.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nzc.tanke756.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://slx.birdmap.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pua.jiagoushi.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wvu.jqgufenzy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blq.yueranfly.top

[B07] while 循环
来源：http://lqu.ehwqpu.com

Py:   while i < 10: i += 1
来源：http://qac.birdmap.top

PHP:  while ($i < 10) { $i++; }
来源：http://fjx.sjlbkw.cn

JS:   while (i < 10) { i++; }
来源：http://wtq.ehwqpu.com

TS:   while (i < 10) { i++; }
来源：http://ooa.fengsongda.top

Java: while (i < 10) { i++; }
来源：http://vac.yonumen.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qxw.gogol.net.cn

Ruby: while i < 10; i += 1; end
来源：http://tzh.snrcjt.cn

C#:   while (i < 10) { i++; }
来源：http://efm.yfazqb.com

[B08] do-while（至少执行一次）
来源：http://twn.yueranfly.top

Py:   # 无 do-while：用 while True + break
来源：http://gib.jqgfzy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bby.zhongyouzk.top

JS:   do { i++; } while (i < 10);
来源：http://vef.shanyushiyangtech.top

TS:   do { i++; } while (i < 10);
来源：http://tyh.fzhhl.top

Java: do { i++; } while (i < 10);
来源：http://fdv.daria6918.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://wph.ppjwa.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hsx.9152youxi.cn

C#:   do { i++; } while (i < 10);
来源：http://ypp.yuanzhike.top

[B09] break 与 continue
来源：http://nuk.jinqigfzy.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yej.zhiwuduotai.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ezk.gaohongyu789.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uje.hcnkem.com

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qzm.zdbjq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kwv.xziqi.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pgb.daria6918.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://efy.zdqjudy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://beh.jiagoushi.top

[B10] 遍历同时拿索引
来源：http://dgb.fehbvm.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ohg.shanyushiyangtech.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ezu.uphjek.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://swe.tianlin.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://riu.tian-w.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vws.bjfxy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mqk.jqgufenzy.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://swn.birdmap.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://luv.zhoulong.xyz

[B11] 生成数字序列 / 区间
来源：http://tnb.chenjidiqi.icu

Py:   list(range(0, 10, 2))
来源：http://uka.jinqigfzy.top

PHP:  range(0, 10, 2);
来源：http://wns.yonumen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gjr.bbcook.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xxj.bbcook.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://seb.yj20258888.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://opn.yuxming.cn

Ruby: (0...10).step(2).to_a
来源：http://nbd.sjlbkw.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mxx.jqgfzy.top

[B12] 跳出多层循环
来源：http://xah.feifeiyinyue.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qfs.hesvh.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uqh.ctjpmb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vgz.xuanzx.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://fqf.zhongyouzk.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://isn.52xcode.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vhu.fktsv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://svn.mhx1999.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gmt.zhoulong.xyz

[B13] 判断是否为数字
来源：http://erl.snrcjt.cn

Py:   isinstance(x, (int, float))
来源：http://fsi.quarkkingdee.top

PHP:  is_numeric($x)
来源：http://psc.pengpengdd.cyou

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zdd.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kkb.yvedp.cn

Java: x instanceof Number
来源：http://zxm.316326.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pob.chenzaomai.com

Ruby: x.is_a?(Numeric)
来源：http://ygs.hammf.cn

C#:   x is int or double or decimal
来源：http://lgi.cashguo.top

[B14] 判断值是否在集合内
来源：http://ssk.pengpengdd.cyou

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nsp.vqdsnc.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qen.jlsjyb.cn

JS:   [1, 2, 3].includes(x)
来源：http://lbb.chenjidiqi.icu

TS:   [1, 2, 3].includes(x)
来源：http://odc.52xcode.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rph.yj20258.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vyy.52xcode.cn

Ruby: [1, 2, 3].include?(x)
来源：http://jqx.haohaochexian.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jdp.hnxiangtu.top

[B15] 布尔运算与取反
来源：http://hnm.zhengqikj.top

Py:   a and b or not c
来源：http://nqp.xuetiantiany.cn

PHP:  $a && $b || !$c
来源：http://tra.hongshengwenyu.top

JS:   a && b || !c
来源：http://qpe.sxryk.cn

TS:   a && b || !c
来源：http://idi.chenzaomai.com

Java: a && b || !c
来源：http://etv.jiagoushi.top

Go:   a && b || !c
来源：http://kwc.ehwqpu.com

Ruby: a && b || !c
来源：http://met.vqdsnc.cn

C#:   a && b || !c
来源：http://dga.chenjidiqi.icu

[B16] 卫语句：不满足条件提前返回
来源：http://mjz.zhoulong.xyz

Py:   if not data: return
来源：http://ocv.zhiwuduotai.top

PHP:  if (!$data) { return; }
来源：http://fmx.hammf.cn

JS:   if (!data) return;
来源：http://suy.cqqwz.cn

TS:   if (!data) return;
来源：http://hra.havefunace.top

Java: if (data == null) return;
来源：http://osw.aibaodan.cn

Go:   if data == nil { return }
来源：http://gzv.ydzc1.top

Ruby: return if data.nil?
来源：http://aft.chenjidiqi.icu

C#:   if (data == null) return;
来源：http://zjf.cdnleiting.top

================================================================================
来源：http://pma.xziqi.cn

C. 函数与作用域
来源：http://tpd.havefunace.top

================================================================================
来源：http://pwk.cashguo.top

[C01] 定义函数
来源：http://edh.meibo888.top

Py:   def add(a, b): return a + b
来源：http://uwi.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wfl.cqqwz.cn

JS:   function add(a, b) { return a + b; }
来源：http://wzq.kuanghao11.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fti.cqqwz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://tpn.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://lxo.pycfn.com

Ruby: def add(a, b); a + b; end
来源：http://tyo.zhengqikj.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jwk.yonumen.top

[C02] 默认参数
来源：http://dvy.ydzc1.top

Py:   def greet(name="World"): return name
来源：http://ycn.zhoulong.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://wzz.hammf.cn

JS:   function greet(name = "World") { return name; }
来源：http://sfp.ywan-chungtsiang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://obs.yueranfly.top

Java: // 无默认参数：方法重载或 Optional
来源：http://tqb.zhiwuduotai.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qys.ybcxt.top

Ruby: def greet(name = "World") = name
来源：http://rzl.kuanghao11.cn

C#:   string Greet(string name = "World") => name;
来源：http://ntg.zhaomingkeji.xyz

[C03] 可变参数
来源：http://yhy.ywan-chungtsiang.top

Py:   def total(*args): return sum(args)
来源：http://obw.sysykeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jif.zhoulong.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rgg.ydjk.org.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pxf.iojbl.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://btz.cdnleiting.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ede.yvedp.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ccn.havefunace.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bir.hfpthk.cn

[C04] 命名参数 / 关键字参数
来源：http://gtx.tian-w.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ewk.chenjidiqi.icu

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gus.yfazqb.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ehv.xinyue.icu

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://qvu.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://zjc.iojbl.cn

Go:   // 无：用配置结构体参数
来源：http://qsy.hnxiangtu.top

Ruby: f(a: 1, b: 2)
来源：http://tlb.pycfn.com

C#:   f(a: 1, b: 2)
来源：http://lmj.vehdjk.com

[C05] 返回多个值
来源：http://wck.ydzc1.top

Py:   return a, b
来源：http://mkq.smart0.xyz

PHP:  return [$a, $b];
来源：http://rjd.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://omj.epnwcf.com

TS:   return { a, b };
来源：http://uee.cheryme.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hmj.aibaodan.cn

Go:   return a, b
来源：http://xlk.pycfn.com

Ruby: return a, b
来源：http://ein.hywenlv.cn

C#:   return (a, b);              // ValueTuple
来源：http://jme.tanke756.top

[C06] 匿名函数 / lambda
来源：http://eqk.nanxuanxn.top

Py:   square = lambda x: x * x
来源：http://bxb.zhongyouzk.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mxe.sufxvd.cn

JS:   const square = x => x * x;
来源：http://edw.aizwys.cn

TS:   const square = (x: number): number => x * x;
来源：http://esl.cucudq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xpu.zhongyouzk.top

Go:   sq := func(x int) int { return x * x }
来源：http://llr.yfazqb.com

Ruby: square = ->(x) { x * x }
来源：http://aoe.yj202588.top

C#:   Func<int, int> square = x => x * x;
来源：http://yxt.yueranfly.top

[C07] 把函数作为参数传入
来源：http://qav.zhengqikj.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xpr.cqqwz.cn

PHP:  array_map("strtoupper", $arr);
来源：http://cdy.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uwa.jianghu66.top

TS:   arr.map(String)
来源：http://eix.wangdashe.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wxy.vehdjk.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wrh.xingfuxueyuan.xyz


<!-- 参考信息 -->