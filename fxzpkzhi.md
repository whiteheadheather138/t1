代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://evm.zdbjq.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://coz.bjfxy.top

Go:   // 单行；/* 多行 */
来源：http://ohc.cqqwz.cn

Ruby: # 单行；=begin 多行 =end
来源：http://twh.cqqwz.cn

C#:   // 单行；/* 多行 */
来源：http://czy.fzhhl.top

[A15] 空值判断与默认值
来源：http://bup.hammf.cn

Py:   value = data or "默认值"
来源：http://bit.iojbl.cn

PHP:  $value = $data ?? "默认值";
来源：http://chl.ybcxt.top

JS:   const value = data ?? "默认值";
来源：http://gaq.tanke756.top

TS:   const value = data ?? "默认值";
来源：http://fgu.sjlbkw.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://usm.gogol.net.cn

Go:   if data == "" { data = "默认值" }
来源：http://tho.shzxlz.cn

Ruby: value = data || "默认值"
来源：http://kjo.zhengqikj.top

C#:   var value = data ?? "默认值";
来源：http://ixv.gotoacloud.top

[A16] 真假值判断规则
来源：http://djf.tianlin.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://skh.xziqi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dua.andypj.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://yrv.havefunace.top

TS:   if (!x) {}
来源：http://qis.andypj.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ker.hesvh.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://feq.52xcode.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xfl.yongpay.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nbv.aibaodan.cn

[A17] 位运算
来源：http://jgi.xinyue.icu

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yud.svipenyu.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://tnl.jlsjyb.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bhb.zycfv.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fxa.andypj.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://igh.chenzaomai.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gtv.fktsv.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xbf.hywenlv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vrv.shanyushiyangtech.top

[A18] 字符与 ASCII 码互转
来源：http://sou.c1oappe.top

Py:   ord("A"); chr(65)
来源：http://gor.andypj.xyz

PHP:  ord("A"); chr(65)
来源：http://dcl.zycfv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://duy.jinqigufen.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kch.wangdashe.top

Java: (int) 'A'; (char) 65
来源：http://aao.shuidangran.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ilf.fanxiaobao.xyz

Ruby: "A".ord; 65.chr
来源：http://oim.smart0.xyz

C#:   (int)'A'; (char)65
来源：http://uvw.wangdashe.top

[A19] 交换两个变量
来源：http://lsf.sysykeji.top

Py:   a, b = b, a
来源：http://tng.zhaomingkeji.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://acc.redwolf501.top

JS:   [a, b] = [b, a];
来源：http://vfw.cashguo.top

TS:   [a, b] = [b, a];
来源：http://gtz.wangshuangyany.cn

Java: int t = a; a = b; b = t;
来源：http://tbf.zycfv.cn

Go:   a, b = b, a
来源：http://znj.chenjidiqi.icu

Ruby: a, b = b, a
来源：http://ore.zycfv.cn

C#:   (a, b) = (b, a);
来源：http://rty.chenzaomai.com

[A20] 读取标准输入
来源：http://who.xziqi.cn

Py:   name = input("请输入：")
来源：http://djq.cucudq.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://qyp.jinyuanbaomall.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nlx.jinqigufen.top

TS:   // Node.js：readline 模块
来源：http://qrv.jinqigufen.top

Java: new Scanner(System.in).nextLine()
来源：http://fnc.zhaomingkeji.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://oec.ivvv.top

Ruby: gets.chomp
来源：http://cdx.ehwqpu.com

C#:   Console.ReadLine();
来源：http://kjf.jinyuanbaomall.cn

[A21] 保留指定小数位输出
来源：http://ckm.9152youxi.cn

Py:   f"{3.14159:.2f}"
来源：http://jza.mhx1999.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ovs.svipenyu.cn

JS:   (3.14159).toFixed(2)
来源：http://xpi.nanxuanxn.top

TS:   (3.14159).toFixed(2)
来源：http://vni.ehwqpu.com

Java: String.format("%.2f", 3.14159)
来源：http://nva.tianlin.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://efj.cheryme.top

Ruby: format("%.2f", 3.14159)
来源：http://ypi.jianghu66.top

C#:   3.14159.ToString("F2")
来源：http://exp.fehbvm.com

[A22] 获取字符串长度
来源：http://oez.xziqi.cn

Py:   len(s)
来源：http://wjv.tianlin.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lrg.gaohongyu789.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rnp.sjlbkw.cn

TS:   s.length
来源：http://kht.jqgfzy.top

Java: s.length()
来源：http://tni.gaohongyu789.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zag.ctjpmb.com

Ruby: s.length
来源：http://ffb.chenlongwang.top

C#:   s.Length
来源：http://uhw.guowangkeji.top

[A23] 大小写转换
来源：http://nqt.cucudq.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hqm.52xcode.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ngw.yuanzhike.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://zaz.havefunace.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zxg.ctjpmb.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vma.bbcook.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uwa.gotoacloud.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qqn.ppjwa.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://fpv.shzxlz.cn

[A24] 去除首尾空白
来源：http://zoi.ehwqpu.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sdw.fktsv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xxd.snrcjt.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lft.yuanzhike.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bed.yangfankeji.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ylm.jinyuanbaomall.cn

Go:   strings.TrimSpace(s)
来源：http://xvs.gzhubu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ejs.feifeiyinyue.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://myk.hfpthk.cn

[A25] 字符串比较
来源：http://kwu.yj202588.top

Py:   s1 == s2; s1 != s2
来源：http://fpm.svipenyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qwk.sysykeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mph.daxiang520.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ocb.cucudq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://voh.ybcxt.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lvg.jinqigfzy.top

Ruby: s1 == s2; s1 <=> s2
来源：http://uiy.sjlbkw.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xzv.zdbjq.cn

[A26] 类型转换总览
来源：http://cum.yj20258.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://miu.yueranfly.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ydt.sysykeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dcd.nwbrower.top

TS:   Number() String() Boolean() x as number
来源：http://cwp.ywan-chungtsiang.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://osv.ydzc1.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://kvc.zhongyouzk.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xvc.fengsongda.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hlu.quarkkingdee.top

================================================================================
来源：http://dpi.hysaishi.cn

B. 流程控制
来源：http://hay.haohaochexian.top

================================================================================
来源：http://cpj.shzxlz.cn

[B01] 条件判断 if / else
来源：http://hxj.zhijiandao.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://awd.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://het.iojbl.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://emh.zhaomingkeji.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qig.wangdashe.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://gig.tarul.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://egc.zhixingplan.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://rhv.yuxming.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jhr.ivvv.top

[B02] 多分支 else if / elif
来源：http://yzx.hysaishi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cgq.redwolf501.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uol.yj202588.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ook.sufxvd.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dxn.jyoumei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nck.chenlongwang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kne.jlsjyb.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mmq.daxiang520.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nno.shzxlz.cn

[B03] switch / match / case
来源：http://atb.hywenlv.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dfg.ywan-chungtsiang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://whl.daria6918.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ryg.chenjidiqi.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://etd.9152youxi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oti.uphjek.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mnz.ybcxt.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kqb.cqqwz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://snx.zycfv.cn

[B04] for 计数循环
来源：http://xau.aizwys.cn

Py:   for i in range(10): print(i)
来源：http://atu.hongshengwenyu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jfg.fktsv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gut.zhoulong.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://epy.yj20258.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bdy.guannengcc.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://srd.hywenlv.cn

Ruby: 10.times { |i| puts i }
来源：http://xuj.aizwys.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rav.birdmap.top

[B05] 遍历数组 / 列表
来源：http://rau.nanxinkj.top

Py:   for item in arr: print(item)
来源：http://hnh.fzhhl.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hwk.chenzaomai.com

JS:   for (const item of arr) { console.log(item); }
来源：http://kxd.zhaomingkeji.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://viw.xuanzx.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://vjw.mhx1999.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pug.yonumen.top

Ruby: arr.each { |item| puts item }
来源：http://ttm.xylfe.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vvr.iojbl.cn

[B06] 遍历字典 / 对象
来源：http://gzn.yueranfly.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hiq.zhaomingkeji.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lgr.cucudq.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hut.haohaochexian.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yix.dianchejie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pzl.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nuf.xinyue.icu

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xkx.jlsjyb.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cqk.52xcode.cn

[B07] while 循环
来源：http://ebe.zhoulong.xyz

Py:   while i < 10: i += 1
来源：http://ayp.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ghd.zycfv.cn

JS:   while (i < 10) { i++; }
来源：http://gha.hongshengwenyu.top

TS:   while (i < 10) { i++; }
来源：http://ilu.ivvv.top

Java: while (i < 10) { i++; }
来源：http://izv.zhijiandao.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wad.gzhubu.top

Ruby: while i < 10; i += 1; end
来源：http://mfr.zdqjudy.top

C#:   while (i < 10) { i++; }
来源：http://ius.pycfn.com

[B08] do-while（至少执行一次）
来源：http://ghb.tian-w.cn

Py:   # 无 do-while：用 while True + break
来源：http://vkq.shanyushiyangtech.top

PHP:  do { $i++; } while ($i < 10);
来源：http://yls.nanxuanxn.top

JS:   do { i++; } while (i < 10);
来源：http://fim.dashuyun.cn

TS:   do { i++; } while (i < 10);
来源：http://vcu.kuanghao11.cn

Java: do { i++; } while (i < 10);
来源：http://dkn.nanxuanxn.top

Go:   for { i++; if i >= 10 { break } }
来源：http://aui.pycfn.com

Ruby: begin; i += 1; end while i < 10
来源：http://vbf.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://xqw.uphjek.com

[B09] break 与 continue
来源：http://qma.nanxuanxn.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ogb.yangfankeji.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xzp.cashguo.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jfk.jinqigufen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://goa.nwbrower.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gox.sxryk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qop.hammf.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ixp.shangyingyoupin.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ddp.cheryme.top

[B10] 遍历同时拿索引
来源：http://hlz.yvedp.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://yya.yongpay.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ewa.mhx1999.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://daf.hysaishi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pld.xziqi.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://juc.snrcjt.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pvp.yanxiufei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hyv.jyoumei.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xcs.nanxuanxn.top

[B11] 生成数字序列 / 区间
来源：http://fcb.xuanzx.com

Py:   list(range(0, 10, 2))
来源：http://mii.hesvh.cn

PHP:  range(0, 10, 2);
来源：http://kya.guannengcc.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qql.zhongyouzk.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fka.iojbl.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://mqm.jinghuilouyu.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gbt.zhiwuduotai.top

Ruby: (0...10).step(2).to_a
来源：http://clr.ctjpmb.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wky.andypj.xyz

[B12] 跳出多层循环
来源：http://tvs.jianghu66.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wyk.jinyuanbaomall.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://luf.birdmap.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lgr.sweek.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://oih.jyoumei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gvv.nanxinkj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yvp.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cuh.yonumen.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uda.epnwcf.com

[B13] 判断是否为数字
来源：http://wyp.sufxvd.cn

Py:   isinstance(x, (int, float))
来源：http://ree.c1oappe.top

PHP:  is_numeric($x)
来源：http://rnz.nwbrower.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ivf.sufxvd.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tih.fengsongda.top

Java: x instanceof Number
来源：http://rju.hnxiangtu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jme.gzhubu.top

Ruby: x.is_a?(Numeric)
来源：http://xlb.jqgfzy.top

C#:   x is int or double or decimal
来源：http://kpg.chenjidiqi.icu

[B14] 判断值是否在集合内
来源：http://gnm.feifeiyinyue.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ckm.fengsongda.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://kli.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://dfn.shanyushiyangtech.top

TS:   [1, 2, 3].includes(x)
来源：http://ecj.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://mcu.xylfe.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hkd.pycfn.com

Ruby: [1, 2, 3].include?(x)
来源：http://nkk.shangyingyoupin.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zdw.feifeiyinyue.top

[B15] 布尔运算与取反
来源：http://jrs.yfazqb.com

Py:   a and b or not c
来源：http://mum.kuanghao11.cn

PHP:  $a && $b || !$c
来源：http://fsm.zhongyouzk.top

JS:   a && b || !c
来源：http://jjc.zhengqikj.top

TS:   a && b || !c
来源：http://ojk.dianchejie.cn

Java: a && b || !c
来源：http://jkz.gogol.net.cn

Go:   a && b || !c
来源：http://zhw.ehwqpu.com

Ruby: a && b || !c
来源：http://cie.sxryk.cn

C#:   a && b || !c
来源：http://vmt.ybcxt.top

[B16] 卫语句：不满足条件提前返回
来源：http://zgs.hfpthk.cn

Py:   if not data: return
来源：http://vfc.uphjek.com

PHP:  if (!$data) { return; }
来源：http://mer.jqgfzy.top

JS:   if (!data) return;
来源：http://zjk.shanyushiyangkeji.top

TS:   if (!data) return;
来源：http://rbf.yongpay.top

Java: if (data == null) return;
来源：http://bvr.ywan-chungtsiang.top

Go:   if data == nil { return }
来源：http://nwd.ivvv.top

Ruby: return if data.nil?
来源：http://jro.fzhhl.top

C#:   if (data == null) return;
来源：http://grz.tian-w.cn

================================================================================
来源：http://gne.52xcode.cn

C. 函数与作用域
来源：http://len.guowangkeji.top

================================================================================
来源：http://wqf.shangyingyoupin.top

[C01] 定义函数
来源：http://wxn.hysaishi.cn

Py:   def add(a, b): return a + b
来源：http://dbz.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xzr.zhaomingkeji.xyz

JS:   function add(a, b) { return a + b; }
来源：http://nnb.chenjidiqi.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yvb.shangyingyoupin.top

Java: static int add(int a, int b) { return a + b; }
来源：http://qma.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://krj.cucudq.cn

Ruby: def add(a, b); a + b; end
来源：http://qiz.hysaishi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vya.0kj1m.cn

[C02] 默认参数
来源：http://lzc.shangyingyoupin.top

Py:   def greet(name="World"): return name
来源：http://hal.cdnleiting.top

PHP:  function greet($name = "World") { return $name; }
来源：http://imh.zhaomingkeji.xyz

JS:   function greet(name = "World") { return name; }
来源：http://zqh.xuanzx.com

TS:   function greet(name: string = "World") { return name; }
来源：http://rpc.jianghu66.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kqh.zycfv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://yud.gaohongyu789.top

Ruby: def greet(name = "World") = name
来源：http://utt.xingfuxueyuan.xyz

C#:   string Greet(string name = "World") => name;
来源：http://uij.yuanzhike.top

[C03] 可变参数
来源：http://hma.shangyingyoupin.top

Py:   def total(*args): return sum(args)
来源：http://zpx.hcnkem.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qju.iojbl.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mks.sjlbkw.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ykc.fengsongda.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rri.gaohongyu789.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://krt.gzhubu.top

Ruby: def total(*nums); nums.sum; end
来源：http://bgh.jianghu66.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qpr.yanxiufei.cn

[C04] 命名参数 / 关键字参数
来源：http://cue.guowangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://qwd.jinghuilouyu.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rpb.yongpay.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://etr.vehdjk.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kgm.yj20258888.top

Java: // 无：用 Builder 模式或 record
来源：http://eug.gaohongyu789.top

Go:   // 无：用配置结构体参数
来源：http://kwm.tian-w.cn

Ruby: f(a: 1, b: 2)
来源：http://lsj.sweek.top

C#:   f(a: 1, b: 2)
来源：http://ift.hcnkem.com

[C05] 返回多个值
来源：http://lmp.hywenlv.cn


<!-- 参考信息 -->