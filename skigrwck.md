代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://ufc.vqdsnc.cn

[A15] 空值判断与默认值
来源：http://jwb.vehdjk.com

Py:   value = data or "默认值"
来源：http://wpo.yonumen.top

PHP:  $value = $data ?? "默认值";
来源：http://yaq.cdnleiting.top

JS:   const value = data ?? "默认值";
来源：http://dql.yuxming.cn

TS:   const value = data ?? "默认值";
来源：http://uii.yvedp.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://izh.gogol.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://dmr.iojbl.cn

Ruby: value = data || "默认值"
来源：http://cip.yj20258888.top

C#:   var value = data ?? "默认值";
来源：http://twz.shanyushiyangkeji.top

[A16] 真假值判断规则
来源：http://iax.gzhubu.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kcy.zhoulong.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bab.ehwqpu.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://nwd.vehdjk.com

TS:   if (!x) {}
来源：http://qrd.wangdashe.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://bed.jinyuanbaomall.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://olt.hnxiangtu.top

Ruby: unless x            # nil 与 false 为假
来源：http://ehz.smart0.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jmj.52xcode.cn

[A17] 位运算
来源：http://zfm.tarul.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://utl.ydjk.org.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://okm.iojbl.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aaf.sweek.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ogo.wangshuangyany.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eaf.316326.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ijh.guannengcc.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gyf.fengsongda.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ndg.hywenlv.cn

[A18] 字符与 ASCII 码互转
来源：http://osi.hnxiangtu.top

Py:   ord("A"); chr(65)
来源：http://lgp.fanxiaobao.xyz

PHP:  ord("A"); chr(65)
来源：http://yxz.yueranfly.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://liz.epnwcf.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uch.tanke756.top

Java: (int) 'A'; (char) 65
来源：http://sqc.yanxiufei.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hnq.xingfuxueyuan.xyz

Ruby: "A".ord; 65.chr
来源：http://osn.redwolf501.top

C#:   (int)'A'; (char)65
来源：http://ozc.fanxiaobao.xyz

[A19] 交换两个变量
来源：http://ptv.sjlbkw.cn

Py:   a, b = b, a
来源：http://dqx.jinghuilouyu.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jua.52xcode.cn

JS:   [a, b] = [b, a];
来源：http://eua.hfpthk.cn

TS:   [a, b] = [b, a];
来源：http://teh.ywan-chungtsiang.top

Java: int t = a; a = b; b = t;
来源：http://ztx.yj202588.top

Go:   a, b = b, a
来源：http://cbs.c1oappe.top

Ruby: a, b = b, a
来源：http://slz.chenjidiqi.icu

C#:   (a, b) = (b, a);
来源：http://ocf.cashguo.top

[A20] 读取标准输入
来源：http://ifv.0kj1m.cn

Py:   name = input("请输入：")
来源：http://yyg.yj20258888.top

PHP:  $name = trim(fgets(STDIN));
来源：http://edd.jlsjyb.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://utu.guannengcc.top

TS:   // Node.js：readline 模块
来源：http://hes.ehwqpu.com

Java: new Scanner(System.in).nextLine()
来源：http://rar.yj20258888.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://enf.fehbvm.com

Ruby: gets.chomp
来源：http://fxj.hnxiangtu.top

C#:   Console.ReadLine();
来源：http://qah.pengpengdd.cyou

[A21] 保留指定小数位输出
来源：http://cwq.tarul.cn

Py:   f"{3.14159:.2f}"
来源：http://qia.snrcjt.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://eio.shzxlz.cn

JS:   (3.14159).toFixed(2)
来源：http://yum.nanxinkj.top

TS:   (3.14159).toFixed(2)
来源：http://fna.bbcook.cn

Java: String.format("%.2f", 3.14159)
来源：http://skz.wangdashe.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://pbg.dashuyun.cn

Ruby: format("%.2f", 3.14159)
来源：http://ihm.ctjpmb.com

C#:   3.14159.ToString("F2")
来源：http://ksz.yfazqb.com

[A22] 获取字符串长度
来源：http://udn.andypj.xyz

Py:   len(s)
来源：http://jiy.yonumen.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fco.cqqwz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bdu.jqgufenzy.top

TS:   s.length
来源：http://oqg.316326.xyz

Java: s.length()
来源：http://bjr.jinghuilouyu.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oup.jyoumei.cn

Ruby: s.length
来源：http://hqi.ctjpmb.com

C#:   s.Length
来源：http://aqt.fehbvm.com

[A23] 大小写转换
来源：http://eqn.tarul.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wrr.nwbrower.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xak.pycfn.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yuv.52xcode.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qwm.bbcook.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wht.mhx1999.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ysx.ivvv.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mqt.tarul.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pxd.jinqigufen.top

[A24] 去除首尾空白
来源：http://vmu.yuanzhike.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nen.shanyushiyangtech.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yjz.hysaishi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blz.zhijiandao.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yft.ivvv.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vdn.shanyushiyangkeji.top

Go:   strings.TrimSpace(s)
来源：http://jrb.hysaishi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://usn.dianchejie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fjg.yongpay.top

[A25] 字符串比较
来源：http://wlc.hywenlv.cn

Py:   s1 == s2; s1 != s2
来源：http://hxw.nanxuanxn.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wzw.smart0.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://iky.uphjek.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://twn.zhijiandao.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hsw.aibaodan.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mjh.hysaishi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vcy.guowangkeji.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jih.redwolf501.top

[A26] 类型转换总览
来源：http://tfp.fehbvm.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vdv.shangyingyoupin.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mvm.jinqigufen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://utr.daxiang520.top

TS:   Number() String() Boolean() x as number
来源：http://xxd.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ixz.zhijiandao.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jcz.ydzc1.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://fvn.zhiwuduotai.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://wgx.cheryme.top

================================================================================
来源：http://ulg.zycfv.cn

B. 流程控制
来源：http://qcu.hnqzz.top

================================================================================
来源：http://bql.jinyuanbaomall.cn

[B01] 条件判断 if / else
来源：http://yll.bjfxy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://zxw.hcnkem.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://khd.hfpthk.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wtr.kuanghao11.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pmn.daria6918.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xov.hywenlv.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ycj.gaohongyu789.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ykk.0kj1m.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zzn.cqqwz.cn

[B02] 多分支 else if / elif
来源：http://gly.shuidangran.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kym.zhiwuduotai.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ekk.birdmap.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lol.c1oappe.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rcp.dianchejie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fzk.wangshuangyany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://cpv.vehdjk.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mjo.yueranfly.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xxy.ydjk.org.cn

[B03] switch / match / case
来源：http://fef.xingfuxueyuan.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tnh.zhijiandao.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gtk.sufxvd.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tbp.mhx1999.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pfq.shanyushiyangkeji.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dwz.wangdashe.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rzo.cucudq.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lag.ivvv.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ekp.pycfn.com

[B04] for 计数循环
来源：http://ycl.cashguo.top

Py:   for i in range(10): print(i)
来源：http://ehu.wangshuangyany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wvz.ivvv.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://epb.birdmap.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mvm.shanyushiyangkeji.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vvd.ydzc1.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://obx.nwbrower.top

Ruby: 10.times { |i| puts i }
来源：http://yye.uphjek.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://oua.fengsongda.top

[B05] 遍历数组 / 列表
来源：http://uhb.jqgufenzy.top

Py:   for item in arr: print(item)
来源：http://xck.sysykeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://kko.zhixingplan.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wcn.yj20258888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nhf.yangfankeji.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://erq.dianchejie.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://axi.wangdashe.top

Ruby: arr.each { |item| puts item }
来源：http://vmi.yonumen.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lkh.hesvh.cn

[B06] 遍历字典 / 对象
来源：http://boo.chenjidiqi.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://pas.vqdsnc.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://sma.sjlbkw.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ifr.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fsg.fzhhl.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uwy.yj20258.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://yht.chenlongwang.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bxo.xingfuxueyuan.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cnr.fengsongda.top

[B07] while 循环
来源：http://zdb.andypj.xyz

Py:   while i < 10: i += 1
来源：http://dkf.zdbjq.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ths.tanke756.top

JS:   while (i < 10) { i++; }
来源：http://sqc.ydzc1.top

TS:   while (i < 10) { i++; }
来源：http://aqn.xingfuxueyuan.xyz

Java: while (i < 10) { i++; }
来源：http://xpf.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://mru.hysaishi.cn

Ruby: while i < 10; i += 1; end
来源：http://jst.316326.xyz

C#:   while (i < 10) { i++; }
来源：http://bmo.meibo888.top

[B08] do-while（至少执行一次）
来源：http://yfc.jinghuilouyu.cn

Py:   # 无 do-while：用 while True + break
来源：http://pph.xuanzx.com

PHP:  do { $i++; } while ($i < 10);
来源：http://eqr.xingfuxueyuan.xyz

JS:   do { i++; } while (i < 10);
来源：http://gbs.xziqi.cn

TS:   do { i++; } while (i < 10);
来源：http://vfc.dashuyun.cn

Java: do { i++; } while (i < 10);
来源：http://pkb.cheryme.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bnl.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://inj.mhx1999.top

C#:   do { i++; } while (i < 10);
来源：http://pbq.sxryk.cn

[B09] break 与 continue
来源：http://zzn.ivvv.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://cbr.dashuyun.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jys.wangdashe.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kyh.316326.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oea.bjfxy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lbg.jinghuilouyu.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eje.iojbl.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lri.zhixingplan.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ijp.gaohongyu789.top

[B10] 遍历同时拿索引
来源：http://mqa.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xmp.yuxming.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ncz.ywan-chungtsiang.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wkt.c1oappe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://and.xingfuxueyuan.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://khs.sysykeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://crg.cucudq.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xtp.wangshuangyany.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kyl.quarkkingdee.top

[B11] 生成数字序列 / 区间
来源：http://bgx.zhixingplan.top

Py:   list(range(0, 10, 2))
来源：http://lkm.epnwcf.com

PHP:  range(0, 10, 2);
来源：http://xmf.yvedp.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lic.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://paw.hnqzz.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wan.tanke756.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hgg.meibo888.top

Ruby: (0...10).step(2).to_a
来源：http://cwu.tarul.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vtp.yj202588.top

[B12] 跳出多层循环
来源：http://xah.fanxiaobao.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://rol.zhoulong.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://hpn.tianlin.xyz

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://set.shangyingyoupin.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zkw.cdnleiting.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nyd.xylfe.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ccr.sysykeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vrr.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vfj.316326.xyz

[B13] 判断是否为数字
来源：http://qti.yj20258888.top

Py:   isinstance(x, (int, float))
来源：http://vrr.cashguo.top

PHP:  is_numeric($x)
来源：http://kwq.ctjpmb.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ulk.ehwqpu.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tpe.fktsv.cn

Java: x instanceof Number
来源：http://quv.ybcxt.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pgu.yueranfly.top

Ruby: x.is_a?(Numeric)
来源：http://skt.sjlbkw.cn

C#:   x is int or double or decimal
来源：http://qtf.cashguo.top

[B14] 判断值是否在集合内
来源：http://aff.ctjpmb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fei.xylfe.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lyb.chenjidiqi.icu

JS:   [1, 2, 3].includes(x)
来源：http://sgf.sxryk.cn

TS:   [1, 2, 3].includes(x)
来源：http://mxp.birdmap.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mhp.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://aei.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://htx.vqdsnc.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://exr.jianghu66.top

[B15] 布尔运算与取反
来源：http://ume.yfazqb.com

Py:   a and b or not c
来源：http://teg.chenzaomai.com

PHP:  $a && $b || !$c
来源：http://ocd.redwolf501.top

JS:   a && b || !c
来源：http://dqy.zhiwuduotai.top

TS:   a && b || !c
来源：http://lns.ydjk.org.cn

Java: a && b || !c
来源：http://qbg.tian-w.cn

Go:   a && b || !c
来源：http://gcy.yueranfly.top

Ruby: a && b || !c
来源：http://vrz.jianghu66.top

C#:   a && b || !c
来源：http://ebq.redwolf501.top

[B16] 卫语句：不满足条件提前返回
来源：http://vah.fehbvm.com

Py:   if not data: return
来源：http://tqz.feifeiyinyue.top

PHP:  if (!$data) { return; }
来源：http://drf.yanxiufei.cn

JS:   if (!data) return;
来源：http://wqt.feifeiyinyue.top

TS:   if (!data) return;
来源：http://elr.tanke756.top

Java: if (data == null) return;
来源：http://wap.cucudq.cn

Go:   if data == nil { return }
来源：http://six.vqdsnc.cn

Ruby: return if data.nil?
来源：http://dnt.gotoacloud.top

C#:   if (data == null) return;
来源：http://qit.c1oappe.top

================================================================================
来源：http://idm.sufxvd.cn

C. 函数与作用域
来源：http://ppm.tianlin.xyz

================================================================================
来源：http://dqt.yuanzhike.top

[C01] 定义函数
来源：http://wvp.tianlin.xyz

Py:   def add(a, b): return a + b
来源：http://ogz.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aae.shzxlz.cn

JS:   function add(a, b) { return a + b; }
来源：http://ooy.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://oay.yvedp.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://skm.c1oappe.top

Go:   func add(a, b int) int { return a + b }
来源：http://cem.jyoumei.cn

Ruby: def add(a, b); a + b; end
来源：http://ehb.kuanghao11.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pub.cqqwz.cn

[C02] 默认参数
来源：http://lds.pycfn.com

Py:   def greet(name="World"): return name
来源：http://uox.hcnkem.com

PHP:  function greet($name = "World") { return $name; }
来源：http://yav.redwolf501.top

JS:   function greet(name = "World") { return name; }
来源：http://mqd.nanxinkj.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rss.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://txl.fktsv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xgn.cdnleiting.top

Ruby: def greet(name = "World") = name
来源：http://aev.ivvv.top

C#:   string Greet(string name = "World") => name;
来源：http://woe.sjlbkw.cn

[C03] 可变参数
来源：http://wnn.hongshengwenyu.top

Py:   def total(*args): return sum(args)
来源：http://hqw.zhoulong.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vtt.cdnleiting.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ygd.cashguo.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mdp.hfpthk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rtw.havefunace.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xvp.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://mnn.yonumen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zxi.pycfn.com

[C04] 命名参数 / 关键字参数
来源：http://npj.shuidangran.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lpc.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://svm.epnwcf.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vww.ydjk.org.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://igy.vqdsnc.cn

Java: // 无：用 Builder 模式或 record
来源：http://xrq.snrcjt.cn

Go:   // 无：用配置结构体参数
来源：http://fwe.guowangkeji.top

Ruby: f(a: 1, b: 2)
来源：http://avb.wangshuangyany.cn

C#:   f(a: 1, b: 2)
来源：http://zdj.daxiang520.top

[C05] 返回多个值
来源：http://its.zhongyouzk.top

Py:   return a, b
来源：http://bec.yuanzhike.top

PHP:  return [$a, $b];
来源：http://hog.smart0.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://tpw.jqgufenzy.top

TS:   return { a, b };
来源：http://yng.aibaodan.cn


<!-- 参考信息 -->