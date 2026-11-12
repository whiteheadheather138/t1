代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://tqs.zdqjudy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://aoy.ywan-chungtsiang.top

Go:   // 单行；/* 多行 */
来源：http://fmm.nwbrower.top

Ruby: # 单行；=begin 多行 =end
来源：http://fho.ydzc1.top

C#:   // 单行；/* 多行 */
来源：http://vyw.shanyushiyangkeji.top

[A15] 空值判断与默认值
来源：http://gby.wangshuangyany.cn

Py:   value = data or "默认值"
来源：http://bhk.ywan-chungtsiang.top

PHP:  $value = $data ?? "默认值";
来源：http://eue.zhijiandao.cn

JS:   const value = data ?? "默认值";
来源：http://rsy.cheryme.top

TS:   const value = data ?? "默认值";
来源：http://wao.zhiwuduotai.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://rso.shanyushiyangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://yzw.redwolf501.top

Ruby: value = data || "默认值"
来源：http://xjq.feifeiyinyue.top

C#:   var value = data ?? "默认值";
来源：http://fgb.316326.xyz

[A16] 真假值判断规则
来源：http://tjc.yj20258888.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qld.jinqigfzy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ufr.fzhhl.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hky.smart0.xyz

TS:   if (!x) {}
来源：http://enq.jqgfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lhk.zycfv.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://npw.feifeiyinyue.top

Ruby: unless x            # nil 与 false 为假
来源：http://qib.jinqigufen.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xjk.nanxinkj.top

[A17] 位运算
来源：http://abj.cucudq.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://abu.yj202588.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dfm.gogol.net.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zht.zhiwuduotai.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://rzf.chenzaomai.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lak.jlsjyb.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://qje.daxiang520.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gum.xinyue.icu

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://otw.ehwqpu.com

[A18] 字符与 ASCII 码互转
来源：http://qth.snrcjt.cn

Py:   ord("A"); chr(65)
来源：http://bcj.hesvh.cn

PHP:  ord("A"); chr(65)
来源：http://rxt.ppjwa.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lfh.fehbvm.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qhd.yongpay.top

Java: (int) 'A'; (char) 65
来源：http://nwc.epnwcf.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cgh.haohaochexian.top

Ruby: "A".ord; 65.chr
来源：http://rab.c1oappe.top

C#:   (int)'A'; (char)65
来源：http://atd.52xcode.cn

[A19] 交换两个变量
来源：http://ljw.snrcjt.cn

Py:   a, b = b, a
来源：http://zmd.shuidangran.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hvx.cucudq.cn

JS:   [a, b] = [b, a];
来源：http://onz.52xcode.cn

TS:   [a, b] = [b, a];
来源：http://ien.316326.xyz

Java: int t = a; a = b; b = t;
来源：http://yoc.dashuyun.cn

Go:   a, b = b, a
来源：http://bmu.yfazqb.com

Ruby: a, b = b, a
来源：http://fff.hcnkem.com

C#:   (a, b) = (b, a);
来源：http://zdz.cqqwz.cn

[A20] 读取标准输入
来源：http://xyb.jinyuanbaomall.cn

Py:   name = input("请输入：")
来源：http://rac.andypj.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://dth.jlsjyb.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://kgr.ctjpmb.com

TS:   // Node.js：readline 模块
来源：http://lmv.shuidangran.top

Java: new Scanner(System.in).nextLine()
来源：http://uwt.feifeiyinyue.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rvb.jinqigufen.top

Ruby: gets.chomp
来源：http://sdt.redwolf501.top

C#:   Console.ReadLine();
来源：http://zoa.shuidangran.top

[A21] 保留指定小数位输出
来源：http://ywu.bjfxy.top

Py:   f"{3.14159:.2f}"
来源：http://zxj.yuanzhike.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hqk.snrcjt.cn

JS:   (3.14159).toFixed(2)
来源：http://lwq.dianchejie.cn

TS:   (3.14159).toFixed(2)
来源：http://nlt.sweek.top

Java: String.format("%.2f", 3.14159)
来源：http://hzs.feifeiyinyue.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ned.smart0.xyz

Ruby: format("%.2f", 3.14159)
来源：http://sok.bjfxy.top

C#:   3.14159.ToString("F2")
来源：http://tia.hesvh.cn

[A22] 获取字符串长度
来源：http://cfj.gzhubu.top

Py:   len(s)
来源：http://kdy.vehdjk.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://gcf.tian-w.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://egz.ybcxt.top

TS:   s.length
来源：http://afo.xingfuxueyuan.xyz

Java: s.length()
来源：http://wer.zdqjudy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vur.fzhhl.top

Ruby: s.length
来源：http://pmt.hysaishi.cn

C#:   s.Length
来源：http://yzs.zhengqikj.top

[A23] 大小写转换
来源：http://gjq.tarul.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kyg.daxiang520.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gdi.shanyushiyangtech.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://cmb.wangshuangyany.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wru.xuanzx.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ooc.xziqi.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hug.birdmap.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cus.chenlongwang.top

C#:   s.ToUpper(); s.ToLower()
来源：http://arr.0kj1m.cn

[A24] 去除首尾空白
来源：http://fzc.xuetiantiany.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://exd.yuanzhike.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pgw.zhongyouzk.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jop.fanxiaobao.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mgc.ctjpmb.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xzt.svipenyu.cn

Go:   strings.TrimSpace(s)
来源：http://opx.0kj1m.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pic.xinyue.icu

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bea.shanyushiyangtech.top

[A25] 字符串比较
来源：http://awo.xingfuxueyuan.xyz

Py:   s1 == s2; s1 != s2
来源：http://fwn.epnwcf.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://xmy.9152youxi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://oth.kuanghao11.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://csn.snrcjt.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ifz.shanyushiyangtech.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://swz.pengpengdd.cyou

Ruby: s1 == s2; s1 <=> s2
来源：http://fpo.hongshengwenyu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uns.zhengqikj.top

[A26] 类型转换总览
来源：http://syb.hnqzz.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://riz.zycfv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ykq.zhijiandao.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://knf.bjfxy.top

TS:   Number() String() Boolean() x as number
来源：http://lvm.hesvh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nzv.wangshuangyany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ymn.zhongyouzk.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xfw.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://vpd.sjlbkw.cn

================================================================================
来源：http://cun.fengsongda.top

B. 流程控制
来源：http://axn.hongshengwenyu.top

================================================================================
来源：http://mlv.c1oappe.top

[B01] 条件判断 if / else
来源：http://yim.yfazqb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://thc.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ctw.zhaomingkeji.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iut.dianchejie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mjs.chenzaomai.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://ipj.svipenyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bmd.xziqi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://syy.birdmap.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tmm.jinghuilouyu.cn

[B02] 多分支 else if / elif
来源：http://sio.vqdsnc.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wpu.cucudq.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ueu.hnqzz.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rxo.bjfxy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tla.ehwqpu.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kxy.zdbjq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wml.jinqigfzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kpb.redwolf501.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://axa.ehwqpu.com

[B03] switch / match / case
来源：http://lhc.fehbvm.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rdd.chenlongwang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uel.dianchejie.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vlv.mhx1999.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hob.yongpay.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lvb.vqdsnc.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zum.andypj.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eci.xuanzx.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://raa.gaohongyu789.top

[B04] for 计数循环
来源：http://xdr.daria6918.cn

Py:   for i in range(10): print(i)
来源：http://yys.ehwqpu.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jpg.zhoulong.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vhx.ydzc1.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wkx.meibo888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ljt.meibo888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zql.daxiang520.top

Ruby: 10.times { |i| puts i }
来源：http://hpz.yanxiufei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rpt.bjfxy.top

[B05] 遍历数组 / 列表
来源：http://bem.smart0.xyz

Py:   for item in arr: print(item)
来源：http://raq.9152youxi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qgp.hammf.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://xbt.ctjpmb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://njw.cdnleiting.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rgu.tanke756.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://siu.epnwcf.com

Ruby: arr.each { |item| puts item }
来源：http://kyw.yanxiufei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mpu.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://fki.fehbvm.com

Py:   for k, v in d.items(): print(k, v)
来源：http://hbi.jianghu66.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mqz.zhiwuduotai.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bkg.aibaodan.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rsq.sufxvd.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cpb.bbcook.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://erw.kuanghao11.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tnl.xinyue.icu

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://txd.sufxvd.cn

[B07] while 循环
来源：http://lqm.hammf.cn

Py:   while i < 10: i += 1
来源：http://fur.ctjpmb.com

PHP:  while ($i < 10) { $i++; }
来源：http://dxt.zhiwuduotai.top

JS:   while (i < 10) { i++; }
来源：http://geu.sweek.top

TS:   while (i < 10) { i++; }
来源：http://rhk.xuetiantiany.cn

Java: while (i < 10) { i++; }
来源：http://zwr.hywenlv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dpf.hnxiangtu.top

Ruby: while i < 10; i += 1; end
来源：http://jgj.gogol.net.cn

C#:   while (i < 10) { i++; }
来源：http://nyu.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://rut.xylfe.cn

Py:   # 无 do-while：用 while True + break
来源：http://fqe.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://sgz.wangshuangyany.cn

JS:   do { i++; } while (i < 10);
来源：http://bgg.kuanghao11.cn

TS:   do { i++; } while (i < 10);
来源：http://ryn.jinqigfzy.top

Java: do { i++; } while (i < 10);
来源：http://wdk.yanxiufei.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ouc.gzhubu.top

Ruby: begin; i += 1; end while i < 10
来源：http://ylr.ivvv.top

C#:   do { i++; } while (i < 10);
来源：http://nvx.fehbvm.com

[B09] break 与 continue
来源：http://opv.shanyushiyangtech.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ljl.zycfv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wub.yj20258888.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hpu.iojbl.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xyv.sysykeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cpb.ybcxt.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hak.fktsv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vbs.jinqigfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vhd.gogol.net.cn

[B10] 遍历同时拿索引
来源：http://wjm.ppjwa.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yef.smart0.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://feq.yj20258888.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://abx.bjfxy.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yfy.hongshengwenyu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://grr.gzhubu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nne.hesvh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rya.zhaomingkeji.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xun.xuetiantiany.cn

[B11] 生成数字序列 / 区间
来源：http://qan.zhengqikj.top

Py:   list(range(0, 10, 2))
来源：http://ksy.ehwqpu.com

PHP:  range(0, 10, 2);
来源：http://pwk.xinyue.icu

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qpr.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wkt.xuanzx.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lkv.sufxvd.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qdm.yonumen.top

Ruby: (0...10).step(2).to_a
来源：http://cro.epnwcf.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tbp.hnqzz.top

[B12] 跳出多层循环
来源：http://ezg.tarul.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vti.fanxiaobao.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://xvz.daxiang520.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zbl.shanyushiyangkeji.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://lgt.mhx1999.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qjm.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://puy.shangyingyoupin.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ykh.ctjpmb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://zaw.gaohongyu789.top

[B13] 判断是否为数字
来源：http://lys.nwbrower.top

Py:   isinstance(x, (int, float))
来源：http://iyt.c1oappe.top

PHP:  is_numeric($x)
来源：http://tsb.iojbl.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kqr.jiagoushi.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aol.hcnkem.com

Java: x instanceof Number
来源：http://mdi.9152youxi.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wqv.hongshengwenyu.top

Ruby: x.is_a?(Numeric)
来源：http://cua.shanyushiyangkeji.top

C#:   x is int or double or decimal
来源：http://lut.quarkkingdee.top

[B14] 判断值是否在集合内
来源：http://mxg.zdbjq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://oys.hesvh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ias.ctjpmb.com

JS:   [1, 2, 3].includes(x)
来源：http://yfb.gzhubu.top

TS:   [1, 2, 3].includes(x)
来源：http://kql.9152youxi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qoc.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://skv.bbcook.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ohn.aibaodan.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vki.meibo888.top

[B15] 布尔运算与取反
来源：http://pyo.ehwqpu.com

Py:   a and b or not c
来源：http://xkv.shanyushiyangtech.top

PHP:  $a && $b || !$c
来源：http://kfs.tianlin.xyz

JS:   a && b || !c
来源：http://voh.jinqigufen.top

TS:   a && b || !c
来源：http://ysy.gotoacloud.top

Java: a && b || !c
来源：http://pqm.aizwys.cn

Go:   a && b || !c
来源：http://qvt.guannengcc.top

Ruby: a && b || !c
来源：http://ady.tian-w.cn

C#:   a && b || !c
来源：http://gfg.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://idk.sjlbkw.cn

Py:   if not data: return
来源：http://yhe.jiagoushi.top

PHP:  if (!$data) { return; }
来源：http://nto.yuxming.cn

JS:   if (!data) return;
来源：http://ksj.sweek.top

TS:   if (!data) return;
来源：http://wwz.pengpengdd.cyou

Java: if (data == null) return;
来源：http://bek.c1oappe.top

Go:   if data == nil { return }
来源：http://stk.sufxvd.cn

Ruby: return if data.nil?
来源：http://hjx.ydzc1.top

C#:   if (data == null) return;
来源：http://ohp.hfpthk.cn

================================================================================
来源：http://qye.hesvh.cn

C. 函数与作用域
来源：http://lmu.tian-w.cn

================================================================================
来源：http://vcd.bbcook.cn

[C01] 定义函数
来源：http://sbz.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://law.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pdf.shangyingyoupin.top

JS:   function add(a, b) { return a + b; }
来源：http://exq.sxryk.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iyo.guowangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tli.nanxuanxn.top

Go:   func add(a, b int) int { return a + b }
来源：http://zse.c1oappe.top

Ruby: def add(a, b); a + b; end
来源：http://hoo.haohaochexian.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pte.guannengcc.top

[C02] 默认参数
来源：http://njr.jianghu66.top

Py:   def greet(name="World"): return name
来源：http://rnu.yj20258.top

PHP:  function greet($name = "World") { return $name; }
来源：http://lyz.bbcook.cn

JS:   function greet(name = "World") { return name; }
来源：http://zcj.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jpr.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://agw.yongpay.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://whb.zhixingplan.top

Ruby: def greet(name = "World") = name
来源：http://tvk.hfpthk.cn

C#:   string Greet(string name = "World") => name;
来源：http://ahs.mhx1999.top

[C03] 可变参数
来源：http://kxo.shanyushiyangtech.top

Py:   def total(*args): return sum(args)
来源：http://hcc.zhaomingkeji.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uqc.chenjidiqi.icu

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bph.zhongyouzk.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://iuj.sjlbkw.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ptj.tanke756.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://byp.bbcook.cn

Ruby: def total(*nums); nums.sum; end
来源：http://mqp.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mhs.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://jnb.ehwqpu.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://suo.tian-w.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://tha.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://huu.hysaishi.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://uno.hywenlv.cn

Java: // 无：用 Builder 模式或 record
来源：http://coa.guowangkeji.top

Go:   // 无：用配置结构体参数
来源：http://vtf.9152youxi.cn

Ruby: f(a: 1, b: 2)
来源：http://eui.0kj1m.cn

C#:   f(a: 1, b: 2)
来源：http://rwv.yj202588.top

[C05] 返回多个值
来源：http://bnt.shanyushiyangtech.top


<!-- 参考信息 -->