代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://smm.ppjwa.cn

TS:   const value = data ?? "默认值";
来源：http://gzj.dianchejie.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ocl.wangshuangyany.cn

Go:   if data == "" { data = "默认值" }
来源：http://jva.nanxuanxn.top

Ruby: value = data || "默认值"
来源：http://gzl.chenjidiqi.icu

C#:   var value = data ?? "默认值";
来源：http://twp.xingfuxueyuan.xyz

[A16] 真假值判断规则
来源：http://szu.jiagoushi.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hzg.cqqwz.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ryy.wangshuangyany.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nts.chenzaomai.com

TS:   if (!x) {}
来源：http://lgi.ctjpmb.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dlj.zhixingplan.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zze.tian-w.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cuy.aizwys.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://egj.ywan-chungtsiang.top

[A17] 位运算
来源：http://vaq.iojbl.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xhv.yueranfly.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tkj.havefunace.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cpc.aizwys.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bvx.xylfe.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pem.xuetiantiany.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wlu.pengpengdd.cyou

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iii.tanke756.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lil.daxiang520.top

[A18] 字符与 ASCII 码互转
来源：http://caf.ywan-chungtsiang.top

Py:   ord("A"); chr(65)
来源：http://bbf.yanxiufei.cn

PHP:  ord("A"); chr(65)
来源：http://ljx.sufxvd.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yuj.chenjidiqi.icu

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wev.zycfv.cn

Java: (int) 'A'; (char) 65
来源：http://yxs.yuanzhike.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bhm.sxryk.cn

Ruby: "A".ord; 65.chr
来源：http://qhs.jianghu66.top

C#:   (int)'A'; (char)65
来源：http://hll.daria6918.cn

[A19] 交换两个变量
来源：http://ehi.hesvh.cn

Py:   a, b = b, a
来源：http://ipi.hongshengwenyu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://sqf.zdqjudy.top

JS:   [a, b] = [b, a];
来源：http://pmx.gogol.net.cn

TS:   [a, b] = [b, a];
来源：http://bkn.tianlin.xyz

Java: int t = a; a = b; b = t;
来源：http://ccf.hongshengwenyu.top

Go:   a, b = b, a
来源：http://oge.zhixingplan.top

Ruby: a, b = b, a
来源：http://tmi.yongpay.top

C#:   (a, b) = (b, a);
来源：http://tng.hywenlv.cn

[A20] 读取标准输入
来源：http://quh.hysaishi.cn

Py:   name = input("请输入：")
来源：http://osx.tian-w.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pub.jyoumei.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hjo.fzhhl.top

TS:   // Node.js：readline 模块
来源：http://irv.bbcook.cn

Java: new Scanner(System.in).nextLine()
来源：http://llv.vqdsnc.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://efv.jlsjyb.cn

Ruby: gets.chomp
来源：http://lup.jinghuilouyu.cn

C#:   Console.ReadLine();
来源：http://qpg.xylfe.cn

[A21] 保留指定小数位输出
来源：http://pip.fzhhl.top

Py:   f"{3.14159:.2f}"
来源：http://xtr.zhixingplan.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ivo.yueranfly.top

JS:   (3.14159).toFixed(2)
来源：http://kkj.yongpay.top

TS:   (3.14159).toFixed(2)
来源：http://jnj.ybcxt.top

Java: String.format("%.2f", 3.14159)
来源：http://ttu.yonumen.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ntv.chenjidiqi.icu

Ruby: format("%.2f", 3.14159)
来源：http://uhq.ybcxt.top

C#:   3.14159.ToString("F2")
来源：http://uoe.fzhhl.top

[A22] 获取字符串长度
来源：http://emp.hnxiangtu.top

Py:   len(s)
来源：http://pht.ydjk.org.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://phb.kuanghao11.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ram.chenzaomai.com

TS:   s.length
来源：http://kos.zhaomingkeji.xyz

Java: s.length()
来源：http://svs.c1oappe.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://khr.haohaochexian.top

Ruby: s.length
来源：http://wqt.vehdjk.com

C#:   s.Length
来源：http://wbz.feifeiyinyue.top

[A23] 大小写转换
来源：http://qii.316326.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://klk.zhoulong.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rmz.fehbvm.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://saj.guannengcc.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qlh.mhx1999.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zcr.chenjidiqi.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rjf.xingfuxueyuan.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://pxj.shuidangran.top

C#:   s.ToUpper(); s.ToLower()
来源：http://bmc.52xcode.cn

[A24] 去除首尾空白
来源：http://pfn.jianghu66.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ihn.feifeiyinyue.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://emt.yueranfly.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vbs.jinyuanbaomall.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hzo.xuanzx.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fhz.hcnkem.com

Go:   strings.TrimSpace(s)
来源：http://tde.yvedp.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://djj.pengpengdd.cyou

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ktm.yvedp.cn

[A25] 字符串比较
来源：http://djv.fktsv.cn

Py:   s1 == s2; s1 != s2
来源：http://jug.0kj1m.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pzy.zdqjudy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dil.guowangkeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://auq.zhiwuduotai.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jjy.cdnleiting.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vqs.yongpay.top

Ruby: s1 == s2; s1 <=> s2
来源：http://myt.ydjk.org.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://riv.cucudq.cn

[A26] 类型转换总览
来源：http://euc.xziqi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bke.jinyuanbaomall.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://njk.sjlbkw.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yhl.wangdashe.top

TS:   Number() String() Boolean() x as number
来源：http://dgy.tian-w.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://top.cqqwz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wsv.aibaodan.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://skq.yuanzhike.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mev.svipenyu.cn

================================================================================
来源：http://pad.tarul.cn

B. 流程控制
来源：http://qxf.havefunace.top

================================================================================
来源：http://cpf.guannengcc.top

[B01] 条件判断 if / else
来源：http://til.ehwqpu.com

Py:   result = "正" if x > 0 else "非正"
来源：http://mex.xinyue.icu

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://olh.meibo888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vpm.hongshengwenyu.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cby.yuxming.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tji.guannengcc.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://heh.hcnkem.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cum.tarul.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dex.316326.xyz

[B02] 多分支 else if / elif
来源：http://mbl.tianlin.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://omw.hongshengwenyu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zfo.ydjk.org.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iyt.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dgw.cdnleiting.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vex.havefunace.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xcm.hongshengwenyu.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ivz.chenzaomai.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qwd.ivvv.top

[B03] switch / match / case
来源：http://tyh.sysykeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tlk.gogol.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kiv.quarkkingdee.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lwt.jlsjyb.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fsr.shanyushiyangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qoz.hesvh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hie.chenzaomai.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xwp.yuxming.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qew.pycfn.com

[B04] for 计数循环
来源：http://dhv.ehwqpu.com

Py:   for i in range(10): print(i)
来源：http://hfu.yuxming.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://abz.tanke756.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jnw.xylfe.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qge.c1oappe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dgt.pycfn.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://osh.wangdashe.top

Ruby: 10.times { |i| puts i }
来源：http://lig.zhixingplan.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kqe.xuanzx.com

[B05] 遍历数组 / 列表
来源：http://wgv.iojbl.cn

Py:   for item in arr: print(item)
来源：http://eiq.hesvh.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mrt.sufxvd.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://dtz.xinyue.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://dik.fehbvm.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://zsz.xziqi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yjv.chenzaomai.com

Ruby: arr.each { |item| puts item }
来源：http://kuu.jinqigfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tdw.hywenlv.cn

[B06] 遍历字典 / 对象
来源：http://tnd.ybcxt.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ixb.sxryk.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ita.zhixingplan.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pkh.nwbrower.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tiq.iojbl.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://iqn.zhixingplan.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qag.shzxlz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ssy.hammf.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dvw.sysykeji.top

[B07] while 循环
来源：http://qmn.yuxming.cn

Py:   while i < 10: i += 1
来源：http://erb.jlsjyb.cn

PHP:  while ($i < 10) { $i++; }
来源：http://hdp.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://rkm.snrcjt.cn

TS:   while (i < 10) { i++; }
来源：http://mtw.xuetiantiany.cn

Java: while (i < 10) { i++; }
来源：http://rox.xinyue.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pjt.zdbjq.cn

Ruby: while i < 10; i += 1; end
来源：http://byw.gaohongyu789.top

C#:   while (i < 10) { i++; }
来源：http://auj.bbcook.cn

[B08] do-while（至少执行一次）
来源：http://tcp.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://saf.xuetiantiany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lhk.wangdashe.top

JS:   do { i++; } while (i < 10);
来源：http://nfw.iojbl.cn

TS:   do { i++; } while (i < 10);
来源：http://zxp.yangfankeji.com

Java: do { i++; } while (i < 10);
来源：http://yds.chenlongwang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://kjp.hysaishi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wsy.fktsv.cn

C#:   do { i++; } while (i < 10);
来源：http://kpv.cashguo.top

[B09] break 与 continue
来源：http://iyu.316326.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lyp.shanyushiyangtech.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kpi.nanxuanxn.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dxi.svipenyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xuv.xuanzx.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://shw.zhaomingkeji.xyz

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ydp.ehwqpu.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://bjm.zhaomingkeji.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lox.daria6918.cn

[B10] 遍历同时拿索引
来源：http://vob.fktsv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wdp.pengpengdd.cyou

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vsw.gogol.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vte.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hxh.hammf.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kni.daria6918.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qih.52xcode.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vxu.nanxuanxn.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tyf.cqqwz.cn

[B11] 生成数字序列 / 区间
来源：http://srh.shanyushiyangtech.top

Py:   list(range(0, 10, 2))
来源：http://tzc.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://snd.chenlongwang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yfj.jiagoushi.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://abl.nanxuanxn.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://svr.cqqwz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zxk.316326.xyz

Ruby: (0...10).step(2).to_a
来源：http://sue.xingfuxueyuan.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://rce.cucudq.cn

[B12] 跳出多层循环
来源：http://gjl.shuidangran.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ipg.bjfxy.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://aow.jlsjyb.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mln.snrcjt.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hza.fzhhl.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://htr.zhiwuduotai.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://sge.zhiwuduotai.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xcy.cqqwz.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tfa.nanxinkj.top

[B13] 判断是否为数字
来源：http://gyt.wangdashe.top

Py:   isinstance(x, (int, float))
来源：http://ufn.ywan-chungtsiang.top

PHP:  is_numeric($x)
来源：http://eig.52xcode.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iga.wangshuangyany.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nex.sufxvd.cn

Java: x instanceof Number
来源：http://gaj.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tvv.cucudq.cn

Ruby: x.is_a?(Numeric)
来源：http://imn.guowangkeji.top

C#:   x is int or double or decimal
来源：http://qtm.jinqigfzy.top

[B14] 判断值是否在集合内
来源：http://qox.sufxvd.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jgy.ydjk.org.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://thd.vehdjk.com

JS:   [1, 2, 3].includes(x)
来源：http://uhi.havefunace.top

TS:   [1, 2, 3].includes(x)
来源：http://fbz.xuetiantiany.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fyn.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://miq.hywenlv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://hgs.sufxvd.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nes.zdbjq.cn

[B15] 布尔运算与取反
来源：http://mer.c1oappe.top

Py:   a and b or not c
来源：http://lyp.yj20258888.top

PHP:  $a && $b || !$c
来源：http://atv.ehwqpu.com

JS:   a && b || !c
来源：http://oio.jinyuanbaomall.cn

TS:   a && b || !c
来源：http://ovk.jinqigufen.top

Java: a && b || !c
来源：http://xot.ehwqpu.com

Go:   a && b || !c
来源：http://rqn.jinqigfzy.top

Ruby: a && b || !c
来源：http://jtp.guannengcc.top

C#:   a && b || !c
来源：http://xmd.chenlongwang.top

[B16] 卫语句：不满足条件提前返回
来源：http://mwc.hongshengwenyu.top

Py:   if not data: return
来源：http://uxj.ywan-chungtsiang.top

PHP:  if (!$data) { return; }
来源：http://tjj.ywan-chungtsiang.top

JS:   if (!data) return;
来源：http://hvn.gaohongyu789.top

TS:   if (!data) return;
来源：http://wxn.chenjidiqi.icu

Java: if (data == null) return;
来源：http://suk.ehwqpu.com

Go:   if data == nil { return }
来源：http://gex.nanxinkj.top

Ruby: return if data.nil?
来源：http://oda.tian-w.cn

C#:   if (data == null) return;
来源：http://mgs.9152youxi.cn

================================================================================
来源：http://hos.mhx1999.top

C. 函数与作用域
来源：http://oub.fengsongda.top

================================================================================
来源：http://yeo.hfpthk.cn

[C01] 定义函数
来源：http://uwt.cucudq.cn

Py:   def add(a, b): return a + b
来源：http://wck.bjfxy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fiz.jinqigfzy.top

JS:   function add(a, b) { return a + b; }
来源：http://lgw.xylfe.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://zzg.cqqwz.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://bxt.fehbvm.com

Go:   func add(a, b int) int { return a + b }
来源：http://atl.jinyuanbaomall.cn

Ruby: def add(a, b); a + b; end
来源：http://ygm.yuxming.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://skm.chenlongwang.top

[C02] 默认参数
来源：http://vpd.jqgufenzy.top

Py:   def greet(name="World"): return name
来源：http://cpo.jlsjyb.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ydi.yuxming.cn

JS:   function greet(name = "World") { return name; }
来源：http://uhg.xuanzx.com

TS:   function greet(name: string = "World") { return name; }
来源：http://sjx.wangshuangyany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://lag.guannengcc.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aeo.wangdashe.top

Ruby: def greet(name = "World") = name
来源：http://qzq.jianghu66.top

C#:   string Greet(string name = "World") => name;
来源：http://iis.andypj.xyz

[C03] 可变参数
来源：http://gur.wangdashe.top

Py:   def total(*args): return sum(args)
来源：http://sgs.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kcl.yongpay.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://fws.epnwcf.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ses.hcnkem.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kgu.zhixingplan.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gdf.pycfn.com

Ruby: def total(*nums); nums.sum; end
来源：http://gye.cucudq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zhb.c1oappe.top

[C04] 命名参数 / 关键字参数
来源：http://gdf.hammf.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tfb.yanxiufei.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://brt.sysykeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ins.c1oappe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jrx.gotoacloud.top

Java: // 无：用 Builder 模式或 record
来源：http://vjp.pengpengdd.cyou

Go:   // 无：用配置结构体参数
来源：http://bia.guannengcc.top

Ruby: f(a: 1, b: 2)
来源：http://tpj.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://fum.dianchejie.cn

[C05] 返回多个值
来源：http://ceq.guowangkeji.top

Py:   return a, b
来源：http://alg.fktsv.cn

PHP:  return [$a, $b];
来源：http://giy.ehwqpu.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://bww.mhx1999.top

TS:   return { a, b };
来源：http://omu.snrcjt.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://pvp.ydzc1.top

Go:   return a, b
来源：http://aca.jqgufenzy.top

Ruby: return a, b
来源：http://nag.fanxiaobao.xyz

C#:   return (a, b);              // ValueTuple
来源：http://mdl.jinqigfzy.top


<!-- 参考信息 -->