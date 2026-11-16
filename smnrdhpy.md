代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://zej.jqgufenzy.top

TS:   const value = data ?? "默认值";
来源：http://zcv.jyoumei.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jpp.shangyingyoupin.top

Go:   if data == "" { data = "默认值" }
来源：http://twd.xingfuxueyuan.xyz

Ruby: value = data || "默认值"
来源：http://shz.cheryme.top

C#:   var value = data ?? "默认值";
来源：http://yrg.quarkkingdee.top

[A16] 真假值判断规则
来源：http://fwp.zhixingplan.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rge.sjlbkw.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qcg.ywan-chungtsiang.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xts.shanyushiyangkeji.top

TS:   if (!x) {}
来源：http://vgw.yuanzhike.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://kbm.cqqwz.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://awo.kuanghao11.cn

Ruby: unless x            # nil 与 false 为假
来源：http://stv.aizwys.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://pik.hywenlv.cn

[A17] 位运算
来源：http://fxr.yongpay.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ijh.zhixingplan.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xcb.0kj1m.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tex.ppjwa.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lau.bjfxy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cos.daxiang520.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://vey.nwbrower.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://obd.zhaomingkeji.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mcd.hcnkem.com

[A18] 字符与 ASCII 码互转
来源：http://pxr.pengpengdd.cyou

Py:   ord("A"); chr(65)
来源：http://yco.yuxming.cn

PHP:  ord("A"); chr(65)
来源：http://yha.zdqjudy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xnw.shanyushiyangtech.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://alx.fzhhl.top

Java: (int) 'A'; (char) 65
来源：http://nvu.yonumen.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gky.hcnkem.com

Ruby: "A".ord; 65.chr
来源：http://org.zhaomingkeji.xyz

C#:   (int)'A'; (char)65
来源：http://ohf.jyoumei.cn

[A19] 交换两个变量
来源：http://bgx.feifeiyinyue.top

Py:   a, b = b, a
来源：http://lht.daxiang520.top

PHP:  [$a, $b] = [$b, $a];
来源：http://cer.jinyuanbaomall.cn

JS:   [a, b] = [b, a];
来源：http://zfc.shanyushiyangkeji.top

TS:   [a, b] = [b, a];
来源：http://cgq.sxryk.cn

Java: int t = a; a = b; b = t;
来源：http://rcy.kuanghao11.cn

Go:   a, b = b, a
来源：http://sgj.sysykeji.top

Ruby: a, b = b, a
来源：http://hsw.yj202588.top

C#:   (a, b) = (b, a);
来源：http://otx.mhx1999.top

[A20] 读取标准输入
来源：http://zhn.nanxinkj.top

Py:   name = input("请输入：")
来源：http://mvg.sysykeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://zrj.hcnkem.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rcd.dashuyun.cn

TS:   // Node.js：readline 模块
来源：http://cur.shanyushiyangkeji.top

Java: new Scanner(System.in).nextLine()
来源：http://ajr.shuidangran.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://vpk.daria6918.cn

Ruby: gets.chomp
来源：http://unl.redwolf501.top

C#:   Console.ReadLine();
来源：http://fxg.pengpengdd.cyou

[A21] 保留指定小数位输出
来源：http://cmm.hongshengwenyu.top

Py:   f"{3.14159:.2f}"
来源：http://vud.0kj1m.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gtp.ppjwa.cn

JS:   (3.14159).toFixed(2)
来源：http://rgg.nwbrower.top

TS:   (3.14159).toFixed(2)
来源：http://rpo.zycfv.cn

Java: String.format("%.2f", 3.14159)
来源：http://rtu.gotoacloud.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://opi.nanxuanxn.top

Ruby: format("%.2f", 3.14159)
来源：http://ilw.zhengqikj.top

C#:   3.14159.ToString("F2")
来源：http://lfj.wangshuangyany.cn

[A22] 获取字符串长度
来源：http://cse.hnxiangtu.top

Py:   len(s)
来源：http://akt.zycfv.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oiw.nanxuanxn.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gpe.ybcxt.top

TS:   s.length
来源：http://zfp.yuanzhike.top

Java: s.length()
来源：http://hvx.c1oappe.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xpt.fehbvm.com

Ruby: s.length
来源：http://xsr.bjfxy.top

C#:   s.Length
来源：http://zmk.tian-w.cn

[A23] 大小写转换
来源：http://mct.zhengqikj.top

Py:   s.upper(); s.lower(); s.title()
来源：http://rfv.ydzc1.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uej.fengsongda.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zcy.epnwcf.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pog.kuanghao11.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ywq.vqdsnc.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nrg.cucudq.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://kzk.zhiwuduotai.top

C#:   s.ToUpper(); s.ToLower()
来源：http://omb.fzhhl.top

[A24] 去除首尾空白
来源：http://lsc.ppjwa.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rrt.yangfankeji.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ife.bbcook.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wdm.aibaodan.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nzy.zycfv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qun.cucudq.cn

Go:   strings.TrimSpace(s)
来源：http://pcj.jlsjyb.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pdx.52xcode.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mzh.ivvv.top

[A25] 字符串比较
来源：http://lrb.meibo888.top

Py:   s1 == s2; s1 != s2
来源：http://gyv.chenjidiqi.icu

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eot.cheryme.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uub.pengpengdd.cyou

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://clw.hnxiangtu.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cjs.daria6918.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mux.zdqjudy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://pme.ydjk.org.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xnh.ydjk.org.cn

[A26] 类型转换总览
来源：http://yyk.zhongyouzk.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gip.xuetiantiany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sxg.fzhhl.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://eeb.yongpay.top

TS:   Number() String() Boolean() x as number
来源：http://iwt.zdbjq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://aah.zhixingplan.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kbz.tian-w.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://scb.jinqigfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sll.shanyushiyangkeji.top

================================================================================
来源：http://saj.hnxiangtu.top

B. 流程控制
来源：http://cbq.fehbvm.com

================================================================================
来源：http://zkr.hysaishi.cn

[B01] 条件判断 if / else
来源：http://qkt.jyoumei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mjb.sweek.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sul.jianghu66.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://oma.zhixingplan.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bhy.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://gjl.xziqi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qjg.yj202588.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://uuy.yuanzhike.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xfw.bjfxy.top

[B02] 多分支 else if / elif
来源：http://nvk.vqdsnc.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://njj.fehbvm.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uxu.9152youxi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eua.jiagoushi.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eod.xylfe.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jmn.yangfankeji.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rns.hnqzz.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wew.zhiwuduotai.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://csl.yvedp.cn

[B03] switch / match / case
来源：http://tai.sysykeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://uzp.shuidangran.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ydl.fehbvm.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xxc.iojbl.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kyh.redwolf501.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mxm.hesvh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tyi.feifeiyinyue.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tpa.daria6918.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rkc.dianchejie.cn

[B04] for 计数循环
来源：http://zpl.hesvh.cn

Py:   for i in range(10): print(i)
来源：http://chu.yj202588.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mpd.feifeiyinyue.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uiq.hammf.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cdy.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lvj.xuetiantiany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://xnu.dianchejie.cn

Ruby: 10.times { |i| puts i }
来源：http://cik.bbcook.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://dzu.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://mpy.nanxinkj.top

Py:   for item in arr: print(item)
来源：http://ilb.yvedp.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bvw.redwolf501.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gqx.hnqzz.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hgr.yuxming.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kyv.cucudq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vhi.shuidangran.top

Ruby: arr.each { |item| puts item }
来源：http://smt.zhongyouzk.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://kwf.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://egh.fzhhl.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ptv.hnqzz.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zso.fktsv.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yfs.hnxiangtu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bsv.quarkkingdee.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nqy.hywenlv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rvo.ydjk.org.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hzt.iojbl.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ahs.shanyushiyangkeji.top

[B07] while 循环
来源：http://blp.gaohongyu789.top

Py:   while i < 10: i += 1
来源：http://jsc.shanyushiyangtech.top

PHP:  while ($i < 10) { $i++; }
来源：http://dqs.gzhubu.top

JS:   while (i < 10) { i++; }
来源：http://ubo.tarul.cn

TS:   while (i < 10) { i++; }
来源：http://xit.xziqi.cn

Java: while (i < 10) { i++; }
来源：http://etq.ppjwa.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ogu.yfazqb.com

Ruby: while i < 10; i += 1; end
来源：http://wja.iojbl.cn

C#:   while (i < 10) { i++; }
来源：http://lpo.ybcxt.top

[B08] do-while（至少执行一次）
来源：http://dyf.jinqigufen.top

Py:   # 无 do-while：用 while True + break
来源：http://ovp.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dtx.iojbl.cn

JS:   do { i++; } while (i < 10);
来源：http://tqc.ctjpmb.com

TS:   do { i++; } while (i < 10);
来源：http://gqj.xingfuxueyuan.xyz

Java: do { i++; } while (i < 10);
来源：http://hmi.xuanzx.com

Go:   for { i++; if i >= 10 { break } }
来源：http://kue.jinqigufen.top

Ruby: begin; i += 1; end while i < 10
来源：http://vyn.iojbl.cn

C#:   do { i++; } while (i < 10);
来源：http://erx.shanyushiyangkeji.top

[B09] break 与 continue
来源：http://skw.tarul.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vag.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ovt.fehbvm.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fwl.ydzc1.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://waf.yonumen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uve.havefunace.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://dxu.gzhubu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kyx.ydjk.org.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oqc.havefunace.top

[B10] 遍历同时拿索引
来源：http://rwt.andypj.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://cel.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://phx.bbcook.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gli.zhongyouzk.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uko.zhijiandao.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kau.mhx1999.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://tjw.ydzc1.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ryp.ehwqpu.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ipv.yfazqb.com

[B11] 生成数字序列 / 区间
来源：http://axp.jinghuilouyu.cn

Py:   list(range(0, 10, 2))
来源：http://ihb.jinqigfzy.top

PHP:  range(0, 10, 2);
来源：http://fuy.nwbrower.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fwi.feifeiyinyue.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://out.fktsv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tfc.dianchejie.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://vax.gotoacloud.top

Ruby: (0...10).step(2).to_a
来源：http://mad.nanxuanxn.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://sbp.fzhhl.top

[B12] 跳出多层循环
来源：http://xmw.yanxiufei.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://kxu.yongpay.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ubc.xuanzx.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bpn.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wet.tanke756.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rxt.cheryme.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gtw.hywenlv.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xoq.cdnleiting.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://swg.gzhubu.top

[B13] 判断是否为数字
来源：http://xza.fktsv.cn

Py:   isinstance(x, (int, float))
来源：http://zit.aibaodan.cn

PHP:  is_numeric($x)
来源：http://yqq.birdmap.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fus.sxryk.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wkh.hcnkem.com

Java: x instanceof Number
来源：http://uxf.wangdashe.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vow.yuanzhike.top

Ruby: x.is_a?(Numeric)
来源：http://jjm.chenzaomai.com

C#:   x is int or double or decimal
来源：http://oxj.zhaomingkeji.xyz

[B14] 判断值是否在集合内
来源：http://tux.daria6918.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dxc.gotoacloud.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pvj.aizwys.cn

JS:   [1, 2, 3].includes(x)
来源：http://wak.dianchejie.cn

TS:   [1, 2, 3].includes(x)
来源：http://rho.zdbjq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tmq.fzhhl.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://gvo.shanyushiyangtech.top

Ruby: [1, 2, 3].include?(x)
来源：http://klr.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://osa.zhixingplan.top

[B15] 布尔运算与取反
来源：http://zmv.fengsongda.top

Py:   a and b or not c
来源：http://btz.redwolf501.top

PHP:  $a && $b || !$c
来源：http://mjs.yvedp.cn

JS:   a && b || !c
来源：http://dmc.yj20258888.top

TS:   a && b || !c
来源：http://wlo.yj20258888.top

Java: a && b || !c
来源：http://gff.fktsv.cn

Go:   a && b || !c
来源：http://uhl.yuanzhike.top

Ruby: a && b || !c
来源：http://jzq.hnqzz.top

C#:   a && b || !c
来源：http://mam.vqdsnc.cn

[B16] 卫语句：不满足条件提前返回
来源：http://zxf.dianchejie.cn

Py:   if not data: return
来源：http://imj.pycfn.com

PHP:  if (!$data) { return; }
来源：http://xzg.feifeiyinyue.top

JS:   if (!data) return;
来源：http://dvh.jinghuilouyu.cn

TS:   if (!data) return;
来源：http://lcf.haohaochexian.top

Java: if (data == null) return;
来源：http://jno.iojbl.cn

Go:   if data == nil { return }
来源：http://vdj.tianlin.xyz

Ruby: return if data.nil?
来源：http://qam.havefunace.top

C#:   if (data == null) return;
来源：http://qtg.zhaomingkeji.xyz

================================================================================
来源：http://kor.jinqigfzy.top

C. 函数与作用域
来源：http://skl.zdbjq.cn

================================================================================
来源：http://rqb.ppjwa.cn

[C01] 定义函数
来源：http://zsm.zhoulong.xyz

Py:   def add(a, b): return a + b
来源：http://qhv.hcnkem.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://eip.vehdjk.com

JS:   function add(a, b) { return a + b; }
来源：http://ixj.fktsv.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ukx.nwbrower.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bqd.guannengcc.top

Go:   func add(a, b int) int { return a + b }
来源：http://sen.epnwcf.com

Ruby: def add(a, b); a + b; end
来源：http://vcn.shangyingyoupin.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gfp.hysaishi.cn

[C02] 默认参数
来源：http://jbb.tarul.cn

Py:   def greet(name="World"): return name
来源：http://msp.zhijiandao.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://pwl.9152youxi.cn

JS:   function greet(name = "World") { return name; }
来源：http://uir.sufxvd.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zml.yj20258888.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fcp.havefunace.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sne.hcnkem.com

Ruby: def greet(name = "World") = name
来源：http://pcz.daria6918.cn

C#:   string Greet(string name = "World") => name;
来源：http://kip.zhixingplan.top

[C03] 可变参数
来源：http://net.yonumen.top

Py:   def total(*args): return sum(args)
来源：http://dyu.zhijiandao.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hov.gotoacloud.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mxw.ivvv.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://typ.dianchejie.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vhn.sjlbkw.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://asj.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://jrj.c1oappe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bjr.jianghu66.top

[C04] 命名参数 / 关键字参数
来源：http://gdh.jinqigufen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://snf.xylfe.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xgt.guowangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pmz.ywan-chungtsiang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yuk.tian-w.cn

Java: // 无：用 Builder 模式或 record
来源：http://neo.yangfankeji.com

Go:   // 无：用配置结构体参数
来源：http://vmq.jiagoushi.top

Ruby: f(a: 1, b: 2)
来源：http://pbz.kuanghao11.cn

C#:   f(a: 1, b: 2)
来源：http://pmd.andypj.xyz

[C05] 返回多个值
来源：http://zar.zhaomingkeji.xyz

Py:   return a, b
来源：http://wha.tarul.cn

PHP:  return [$a, $b];
来源：http://qeg.hongshengwenyu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://dry.jinyuanbaomall.cn

TS:   return { a, b };
来源：http://ofb.jinyuanbaomall.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xqn.ybcxt.top

Go:   return a, b
来源：http://snj.jinyuanbaomall.cn

Ruby: return a, b
来源：http://aaw.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://slb.jyoumei.cn


<!-- 参考信息 -->