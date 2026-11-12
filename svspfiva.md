代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://mwc.haohaochexian.top

[A15] 空值判断与默认值
来源：http://qwl.jiagoushi.top

Py:   value = data or "默认值"
来源：http://pne.jlsjyb.cn

PHP:  $value = $data ?? "默认值";
来源：http://skk.jinyuanbaomall.cn

JS:   const value = data ?? "默认值";
来源：http://vod.jyoumei.cn

TS:   const value = data ?? "默认值";
来源：http://cvg.hongshengwenyu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://acu.cqqwz.cn

Go:   if data == "" { data = "默认值" }
来源：http://lsw.haohaochexian.top

Ruby: value = data || "默认值"
来源：http://opr.0kj1m.cn

C#:   var value = data ?? "默认值";
来源：http://oft.nwbrower.top

[A16] 真假值判断规则
来源：http://ign.xuanzx.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://jdr.52xcode.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ant.cheryme.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tbl.snrcjt.cn

TS:   if (!x) {}
来源：http://xeu.hesvh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mfa.xinyue.icu

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://biu.pycfn.com

Ruby: unless x            # nil 与 false 为假
来源：http://hij.sjlbkw.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uen.shangyingyoupin.top

[A17] 位运算
来源：http://ucd.fengsongda.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vci.chenjidiqi.icu

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lyt.shanyushiyangtech.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yzb.52xcode.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ndr.pycfn.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ttw.ctjpmb.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://csh.jlsjyb.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dci.zhengqikj.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cmi.ivvv.top

[A18] 字符与 ASCII 码互转
来源：http://rkj.tanke756.top

Py:   ord("A"); chr(65)
来源：http://jmi.nanxinkj.top

PHP:  ord("A"); chr(65)
来源：http://scl.jqgfzy.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sqd.dashuyun.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rui.ydjk.org.cn

Java: (int) 'A'; (char) 65
来源：http://zea.tianlin.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jnh.guowangkeji.top

Ruby: "A".ord; 65.chr
来源：http://swl.xuanzx.com

C#:   (int)'A'; (char)65
来源：http://may.zdqjudy.top

[A19] 交换两个变量
来源：http://tvr.gaohongyu789.top

Py:   a, b = b, a
来源：http://jzn.ehwqpu.com

PHP:  [$a, $b] = [$b, $a];
来源：http://xrg.fengsongda.top

JS:   [a, b] = [b, a];
来源：http://mrn.zhongyouzk.top

TS:   [a, b] = [b, a];
来源：http://wka.shanyushiyangtech.top

Java: int t = a; a = b; b = t;
来源：http://bbn.ivvv.top

Go:   a, b = b, a
来源：http://vtn.bjfxy.top

Ruby: a, b = b, a
来源：http://sve.hnxiangtu.top

C#:   (a, b) = (b, a);
来源：http://kjm.vehdjk.com

[A20] 读取标准输入
来源：http://cja.epnwcf.com

Py:   name = input("请输入：")
来源：http://nsl.sysykeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://vam.tanke756.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ivb.pycfn.com

TS:   // Node.js：readline 模块
来源：http://wpl.iojbl.cn

Java: new Scanner(System.in).nextLine()
来源：http://lav.ywan-chungtsiang.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cru.bbcook.cn

Ruby: gets.chomp
来源：http://vlk.yfazqb.com

C#:   Console.ReadLine();
来源：http://qtx.zhoulong.xyz

[A21] 保留指定小数位输出
来源：http://ams.shanyushiyangtech.top

Py:   f"{3.14159:.2f}"
来源：http://cxb.daria6918.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://uwb.hnqzz.top

JS:   (3.14159).toFixed(2)
来源：http://sgp.c1oappe.top

TS:   (3.14159).toFixed(2)
来源：http://oba.yj20258888.top

Java: String.format("%.2f", 3.14159)
来源：http://szp.ivvv.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://org.jinqigfzy.top

Ruby: format("%.2f", 3.14159)
来源：http://rcr.tianlin.xyz

C#:   3.14159.ToString("F2")
来源：http://grs.sxryk.cn

[A22] 获取字符串长度
来源：http://rvc.xinyue.icu

Py:   len(s)
来源：http://obw.xuanzx.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://muh.wangshuangyany.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vet.jyoumei.cn

TS:   s.length
来源：http://xub.jlsjyb.cn

Java: s.length()
来源：http://yvl.aibaodan.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ngs.zhixingplan.top

Ruby: s.length
来源：http://tny.hywenlv.cn

C#:   s.Length
来源：http://iyb.tarul.cn

[A23] 大小写转换
来源：http://zqx.dashuyun.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rlc.zhaomingkeji.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vzb.ydzc1.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yso.0kj1m.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dal.quarkkingdee.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xgw.dashuyun.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zwc.cdnleiting.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cfk.fanxiaobao.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://oqz.chenjidiqi.icu

[A24] 去除首尾空白
来源：http://kib.zhijiandao.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sts.zhijiandao.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fpn.yfazqb.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://umc.jinqigufen.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ums.jqgfzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://fpz.smart0.xyz

Go:   strings.TrimSpace(s)
来源：http://cyo.yj20258.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dch.zycfv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://icz.haohaochexian.top

[A25] 字符串比较
来源：http://djo.shuidangran.top

Py:   s1 == s2; s1 != s2
来源：http://sip.chenzaomai.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://nyy.ydzc1.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qod.jqgufenzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nxv.jinqigufen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xbf.hysaishi.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://phx.xuanzx.com

Ruby: s1 == s2; s1 <=> s2
来源：http://pip.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ejh.sjlbkw.cn

[A26] 类型转换总览
来源：http://lwv.uphjek.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bsa.jinqigufen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jto.snrcjt.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://yys.svipenyu.cn

TS:   Number() String() Boolean() x as number
来源：http://gco.fehbvm.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dzq.shanyushiyangtech.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nzx.sweek.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://enx.tarul.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://nao.fktsv.cn

================================================================================
来源：http://pub.nwbrower.top

B. 流程控制
来源：http://rni.cashguo.top

================================================================================
来源：http://cib.zycfv.cn

[B01] 条件判断 if / else
来源：http://cxi.snrcjt.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://miw.quarkkingdee.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fcy.sjlbkw.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://saf.c1oappe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://uvh.9152youxi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://upi.jyoumei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qfu.dashuyun.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://lcs.kuanghao11.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hiv.nwbrower.top

[B02] 多分支 else if / elif
来源：http://rfx.zhaomingkeji.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nyd.ydzc1.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uri.guannengcc.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xvj.jinyuanbaomall.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ezi.yuanzhike.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vem.zhengqikj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://glk.cashguo.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dmw.tianlin.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hdz.chenlongwang.top

[B03] switch / match / case
来源：http://jzo.guannengcc.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mmu.meibo888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://djx.hammf.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lan.sufxvd.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pnc.iojbl.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://tve.yonumen.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://abw.epnwcf.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lmn.hywenlv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mnt.dashuyun.cn

[B04] for 计数循环
来源：http://xza.vehdjk.com

Py:   for i in range(10): print(i)
来源：http://kou.wangdashe.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ank.xuanzx.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rwe.hongshengwenyu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oxb.yfazqb.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kue.jlsjyb.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gps.chenzaomai.com

Ruby: 10.times { |i| puts i }
来源：http://mig.yuanzhike.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qhm.shzxlz.cn

[B05] 遍历数组 / 列表
来源：http://tld.yj20258.top

Py:   for item in arr: print(item)
来源：http://non.shuidangran.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cda.9152youxi.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://hay.meibo888.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qrd.shangyingyoupin.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://lct.nanxuanxn.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ekm.shzxlz.cn

Ruby: arr.each { |item| puts item }
来源：http://grz.cucudq.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://alq.zhoulong.xyz

[B06] 遍历字典 / 对象
来源：http://dpm.quarkkingdee.top

Py:   for k, v in d.items(): print(k, v)
来源：http://toa.smart0.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yri.nanxuanxn.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://xlf.vehdjk.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kvz.wangshuangyany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://owc.xziqi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hay.andypj.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ouz.chenzaomai.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ils.wangshuangyany.cn

[B07] while 循环
来源：http://fmf.hysaishi.cn

Py:   while i < 10: i += 1
来源：http://nzb.jqgufenzy.top

PHP:  while ($i < 10) { $i++; }
来源：http://nwf.zhixingplan.top

JS:   while (i < 10) { i++; }
来源：http://oix.chenlongwang.top

TS:   while (i < 10) { i++; }
来源：http://zwc.dianchejie.cn

Java: while (i < 10) { i++; }
来源：http://nlh.cucudq.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wol.andypj.xyz

Ruby: while i < 10; i += 1; end
来源：http://qeq.ybcxt.top

C#:   while (i < 10) { i++; }
来源：http://qzd.gzhubu.top

[B08] do-while（至少执行一次）
来源：http://mpt.zhixingplan.top

Py:   # 无 do-while：用 while True + break
来源：http://bke.fktsv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://oxv.ppjwa.cn

JS:   do { i++; } while (i < 10);
来源：http://pjt.gotoacloud.top

TS:   do { i++; } while (i < 10);
来源：http://xft.pycfn.com

Java: do { i++; } while (i < 10);
来源：http://fef.316326.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://piv.zhaomingkeji.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://yum.jqgfzy.top

C#:   do { i++; } while (i < 10);
来源：http://fon.jinyuanbaomall.cn

[B09] break 与 continue
来源：http://jwy.birdmap.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://heu.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://vaa.hongshengwenyu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://msm.hesvh.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eww.nwbrower.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://knr.bjfxy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://soa.yueranfly.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fuk.yj202588.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rjp.yfazqb.com

[B10] 遍历同时拿索引
来源：http://czx.yfazqb.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tsr.daria6918.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zoq.fehbvm.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ibe.pycfn.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://trw.jqgfzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wqn.jinyuanbaomall.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dey.zhongyouzk.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://byn.vqdsnc.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://poz.sxryk.cn

[B11] 生成数字序列 / 区间
来源：http://vsw.cucudq.cn

Py:   list(range(0, 10, 2))
来源：http://vln.havefunace.top

PHP:  range(0, 10, 2);
来源：http://kym.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zre.cdnleiting.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jmy.dianchejie.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gws.zhijiandao.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qke.tian-w.cn

Ruby: (0...10).step(2).to_a
来源：http://slm.guowangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qqu.yuanzhike.top

[B12] 跳出多层循环
来源：http://msc.birdmap.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lqb.hammf.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://eit.bbcook.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ilg.cheryme.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ebs.uphjek.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bxj.sufxvd.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://isl.ppjwa.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hnz.ctjpmb.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gwf.hcnkem.com

[B13] 判断是否为数字
来源：http://dmi.havefunace.top

Py:   isinstance(x, (int, float))
来源：http://qqv.dianchejie.cn

PHP:  is_numeric($x)
来源：http://myi.sxryk.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vli.gzhubu.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ejt.bbcook.cn

Java: x instanceof Number
来源：http://wcj.tanke756.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wfn.guowangkeji.top

Ruby: x.is_a?(Numeric)
来源：http://iix.redwolf501.top

C#:   x is int or double or decimal
来源：http://wox.pycfn.com

[B14] 判断值是否在集合内
来源：http://zin.yfazqb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://goz.zhoulong.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://riv.guowangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://xrx.fzhhl.top

TS:   [1, 2, 3].includes(x)
来源：http://yhc.xuanzx.com

Java: List.of(1, 2, 3).contains(x)
来源：http://bcf.fktsv.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://znj.uphjek.com

Ruby: [1, 2, 3].include?(x)
来源：http://sxl.chenzaomai.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zsn.hnqzz.top

[B15] 布尔运算与取反
来源：http://ilz.xuetiantiany.cn

Py:   a and b or not c
来源：http://ogh.tarul.cn

PHP:  $a && $b || !$c
来源：http://pza.0kj1m.cn

JS:   a && b || !c
来源：http://rnn.smart0.xyz

TS:   a && b || !c
来源：http://ias.tianlin.xyz

Java: a && b || !c
来源：http://tyw.tarul.cn

Go:   a && b || !c
来源：http://wru.wangshuangyany.cn

Ruby: a && b || !c
来源：http://rlm.ydzc1.top

C#:   a && b || !c
来源：http://kpq.zhijiandao.cn

[B16] 卫语句：不满足条件提前返回
来源：http://yko.xuetiantiany.cn

Py:   if not data: return
来源：http://yra.316326.xyz

PHP:  if (!$data) { return; }
来源：http://kfz.wangdashe.top

JS:   if (!data) return;
来源：http://qlk.jlsjyb.cn

TS:   if (!data) return;
来源：http://jtl.sufxvd.cn

Java: if (data == null) return;
来源：http://iun.jyoumei.cn

Go:   if data == nil { return }
来源：http://cbc.gaohongyu789.top

Ruby: return if data.nil?
来源：http://ogi.tian-w.cn

C#:   if (data == null) return;
来源：http://qvt.ppjwa.cn

================================================================================
来源：http://ujh.hysaishi.cn

C. 函数与作用域
来源：http://siy.tanke756.top

================================================================================
来源：http://etj.gaohongyu789.top

[C01] 定义函数
来源：http://hvv.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://opr.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fbd.ctjpmb.com

JS:   function add(a, b) { return a + b; }
来源：http://lck.quarkkingdee.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ctg.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://rmb.fanxiaobao.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://yhh.sufxvd.cn

Ruby: def add(a, b); a + b; end
来源：http://mfl.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://twr.chenzaomai.com

[C02] 默认参数
来源：http://oei.hongshengwenyu.top

Py:   def greet(name="World"): return name
来源：http://rkt.jinqigufen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qtz.feifeiyinyue.top

JS:   function greet(name = "World") { return name; }
来源：http://yzd.yonumen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://sxt.hfpthk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://knu.yuanzhike.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wbj.xingfuxueyuan.xyz

Ruby: def greet(name = "World") = name
来源：http://vuk.pycfn.com

C#:   string Greet(string name = "World") => name;
来源：http://ctx.xziqi.cn

[C03] 可变参数
来源：http://mdj.bjfxy.top

Py:   def total(*args): return sum(args)
来源：http://wxv.zhixingplan.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://adb.bjfxy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xhg.zycfv.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vnf.chenlongwang.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bdx.mhx1999.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ctd.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://nzz.tianlin.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://voy.nanxuanxn.top

[C04] 命名参数 / 关键字参数
来源：http://djw.vehdjk.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kqu.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hkp.yj20258.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hbh.yj20258888.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rtj.yuanzhike.top

Java: // 无：用 Builder 模式或 record
来源：http://mpr.xylfe.cn

Go:   // 无：用配置结构体参数
来源：http://yoj.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://nnp.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://blj.tianlin.xyz

[C05] 返回多个值
来源：http://npa.yj202588.top

Py:   return a, b
来源：http://mgf.ydzc1.top

PHP:  return [$a, $b];
来源：http://rcc.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://dph.hesvh.cn

TS:   return { a, b };
来源：http://owb.guannengcc.top


<!-- 参考信息 -->