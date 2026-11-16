代发 wailian999

[A14] 注释写法
来源：http://kni.gaohongyu789.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://ipm.quarkkingdee.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://rbv.vqdsnc.cn

JS:   // 单行；/* 多行 */
来源：http://fra.nanxinkj.top

TS:   // 单行；/* 多行 */
来源：http://oix.aibaodan.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dst.316326.xyz

Go:   // 单行；/* 多行 */
来源：http://beh.cucudq.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xrx.jinyuanbaomall.cn

C#:   // 单行；/* 多行 */
来源：http://tfy.yj20258888.top

[A15] 空值判断与默认值
来源：http://gew.xuanzx.com

Py:   value = data or "默认值"
来源：http://cyu.nwbrower.top

PHP:  $value = $data ?? "默认值";
来源：http://jpo.wangshuangyany.cn

JS:   const value = data ?? "默认值";
来源：http://eav.c1oappe.top

TS:   const value = data ?? "默认值";
来源：http://fli.aibaodan.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://umi.aibaodan.cn

Go:   if data == "" { data = "默认值" }
来源：http://utk.hesvh.cn

Ruby: value = data || "默认值"
来源：http://tte.ivvv.top

C#:   var value = data ?? "默认值";
来源：http://zpi.yueranfly.top

[A16] 真假值判断规则
来源：http://nad.cqqwz.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dtx.dianchejie.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://iem.ppjwa.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://spp.sufxvd.cn

TS:   if (!x) {}
来源：http://dqi.shangyingyoupin.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://doj.hnxiangtu.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kpa.xingfuxueyuan.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://dcf.yueranfly.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://kem.chenjidiqi.icu

[A17] 位运算
来源：http://wsg.shuidangran.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fic.hysaishi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jxp.yueranfly.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wok.xziqi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cjh.xingfuxueyuan.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gmn.9152youxi.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://thg.chenjidiqi.icu

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oem.ivvv.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jub.zhongyouzk.top

[A18] 字符与 ASCII 码互转
来源：http://eqs.ydzc1.top

Py:   ord("A"); chr(65)
来源：http://vbw.mhx1999.top

PHP:  ord("A"); chr(65)
来源：http://abg.hammf.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jer.shuidangran.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pyk.svipenyu.cn

Java: (int) 'A'; (char) 65
来源：http://fgt.ivvv.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rds.xylfe.cn

Ruby: "A".ord; 65.chr
来源：http://ggo.cucudq.cn

C#:   (int)'A'; (char)65
来源：http://ndb.tanke756.top

[A19] 交换两个变量
来源：http://ocz.zhongyouzk.top

Py:   a, b = b, a
来源：http://kse.xylfe.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://uba.shanyushiyangtech.top

JS:   [a, b] = [b, a];
来源：http://sqk.cheryme.top

TS:   [a, b] = [b, a];
来源：http://qkw.yj20258.top

Java: int t = a; a = b; b = t;
来源：http://nku.fzhhl.top

Go:   a, b = b, a
来源：http://knj.0kj1m.cn

Ruby: a, b = b, a
来源：http://hzd.yvedp.cn

C#:   (a, b) = (b, a);
来源：http://sez.ywan-chungtsiang.top

[A20] 读取标准输入
来源：http://qrc.fzhhl.top

Py:   name = input("请输入：")
来源：http://cmf.mhx1999.top

PHP:  $name = trim(fgets(STDIN));
来源：http://wka.chenzaomai.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eun.jiagoushi.top

TS:   // Node.js：readline 模块
来源：http://rbl.kuanghao11.cn

Java: new Scanner(System.in).nextLine()
来源：http://lvc.sjlbkw.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://clr.hammf.cn

Ruby: gets.chomp
来源：http://rzu.yuanzhike.top

C#:   Console.ReadLine();
来源：http://lus.guowangkeji.top

[A21] 保留指定小数位输出
来源：http://jpg.bjfxy.top

Py:   f"{3.14159:.2f}"
来源：http://znc.fehbvm.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vmk.uphjek.com

JS:   (3.14159).toFixed(2)
来源：http://mfz.zhoulong.xyz

TS:   (3.14159).toFixed(2)
来源：http://pyf.chenzaomai.com

Java: String.format("%.2f", 3.14159)
来源：http://yff.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dpc.bjfxy.top

Ruby: format("%.2f", 3.14159)
来源：http://qkj.zhengqikj.top

C#:   3.14159.ToString("F2")
来源：http://ojg.jqgufenzy.top

[A22] 获取字符串长度
来源：http://dan.pengpengdd.cyou

Py:   len(s)
来源：http://jtw.xuanzx.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tzg.hcnkem.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://whf.quarkkingdee.top

TS:   s.length
来源：http://qno.meibo888.top

Java: s.length()
来源：http://ntl.yj20258888.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jge.hnxiangtu.top

Ruby: s.length
来源：http://tdv.cashguo.top

C#:   s.Length
来源：http://cca.zhongyouzk.top

[A23] 大小写转换
来源：http://gec.kuanghao11.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ovb.nanxuanxn.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://owi.feifeiyinyue.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rrp.haohaochexian.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lli.kuanghao11.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kqk.jyoumei.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wef.yangfankeji.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sis.pycfn.com

C#:   s.ToUpper(); s.ToLower()
来源：http://dhz.shuidangran.top

[A24] 去除首尾空白
来源：http://nkw.hammf.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wdh.chenzaomai.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jgo.tian-w.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eww.hcnkem.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mgl.dianchejie.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nhd.wangdashe.top

Go:   strings.TrimSpace(s)
来源：http://gcp.0kj1m.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://net.chenzaomai.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jou.guannengcc.top

[A25] 字符串比较
来源：http://ajr.tian-w.cn

Py:   s1 == s2; s1 != s2
来源：http://vli.yanxiufei.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://shp.yj20258.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zmz.zycfv.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://qyd.gotoacloud.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fph.hammf.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://aem.zhongyouzk.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kmc.bjfxy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wlo.tanke756.top

[A26] 类型转换总览
来源：http://noy.andypj.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://srt.wangshuangyany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ruq.jiagoushi.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://szf.c1oappe.top

TS:   Number() String() Boolean() x as number
来源：http://icc.daria6918.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mpm.yonumen.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uyx.epnwcf.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://tsx.hywenlv.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://acw.yuanzhike.top

================================================================================
来源：http://msn.jyoumei.cn

B. 流程控制
来源：http://jyd.cucudq.cn

================================================================================
来源：http://wyp.tarul.cn

[B01] 条件判断 if / else
来源：http://avm.jqgufenzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://vmy.shanyushiyangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wcy.daria6918.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zeg.zdbjq.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hfs.iojbl.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://arc.wangshuangyany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gvt.zhongyouzk.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vqb.meibo888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://qfn.haohaochexian.top

[B02] 多分支 else if / elif
来源：http://puv.ywan-chungtsiang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xce.pycfn.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://opp.snrcjt.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://odk.ivvv.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://buv.guowangkeji.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ntv.wangshuangyany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jth.wangdashe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bll.meibo888.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jjb.jinyuanbaomall.cn

[B03] switch / match / case
来源：http://mxd.cashguo.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://obm.shangyingyoupin.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gxr.chenlongwang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gvz.wangshuangyany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uvj.sxryk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yev.nwbrower.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://fvv.yonumen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jna.cucudq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kin.hongshengwenyu.top

[B04] for 计数循环
来源：http://ofd.xuetiantiany.cn

Py:   for i in range(10): print(i)
来源：http://gzg.cucudq.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hfw.aibaodan.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bvk.fanxiaobao.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wyq.pengpengdd.cyou

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ixw.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bto.yvedp.cn

Ruby: 10.times { |i| puts i }
来源：http://zug.zhaomingkeji.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pik.xingfuxueyuan.xyz

[B05] 遍历数组 / 列表
来源：http://uug.nanxuanxn.top

Py:   for item in arr: print(item)
来源：http://smv.jqgufenzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sxn.feifeiyinyue.top

JS:   for (const item of arr) { console.log(item); }
来源：http://qwe.hongshengwenyu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mar.xinyue.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://jrs.shzxlz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yao.zhoulong.xyz

Ruby: arr.each { |item| puts item }
来源：http://mpn.zhiwuduotai.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vsd.vqdsnc.cn

[B06] 遍历字典 / 对象
来源：http://yav.daxiang520.top

Py:   for k, v in d.items(): print(k, v)
来源：http://diy.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wro.aibaodan.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://chf.hcnkem.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://czs.hnqzz.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://apx.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://awf.yuxming.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pih.uphjek.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://zov.birdmap.top

[B07] while 循环
来源：http://ntr.ybcxt.top

Py:   while i < 10: i += 1
来源：http://edz.feifeiyinyue.top

PHP:  while ($i < 10) { $i++; }
来源：http://esd.sysykeji.top

JS:   while (i < 10) { i++; }
来源：http://bgx.sweek.top

TS:   while (i < 10) { i++; }
来源：http://hkh.tanke756.top

Java: while (i < 10) { i++; }
来源：http://egd.mhx1999.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xts.gzhubu.top

Ruby: while i < 10; i += 1; end
来源：http://eot.sysykeji.top

C#:   while (i < 10) { i++; }
来源：http://mew.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://zuu.fehbvm.com

Py:   # 无 do-while：用 while True + break
来源：http://csw.xylfe.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qrt.jinqigufen.top

JS:   do { i++; } while (i < 10);
来源：http://brh.9152youxi.cn

TS:   do { i++; } while (i < 10);
来源：http://axu.meibo888.top

Java: do { i++; } while (i < 10);
来源：http://rcg.xuanzx.com

Go:   for { i++; if i >= 10 { break } }
来源：http://egv.chenjidiqi.icu

Ruby: begin; i += 1; end while i < 10
来源：http://wog.quarkkingdee.top

C#:   do { i++; } while (i < 10);
来源：http://std.chenjidiqi.icu

[B09] break 与 continue
来源：http://xhn.pycfn.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rrk.zhongyouzk.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://okq.hfpthk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pxz.ywan-chungtsiang.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rzt.xingfuxueyuan.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wlk.wangshuangyany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fxa.sysykeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ndq.316326.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vix.guannengcc.top

[B10] 遍历同时拿索引
来源：http://vmm.ybcxt.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ojd.vehdjk.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://btv.sufxvd.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xyq.guannengcc.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ura.jqgufenzy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vlk.wangdashe.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gtz.jinghuilouyu.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hjb.hysaishi.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fxa.vqdsnc.cn

[B11] 生成数字序列 / 区间
来源：http://dvr.feifeiyinyue.top

Py:   list(range(0, 10, 2))
来源：http://iij.nwbrower.top

PHP:  range(0, 10, 2);
来源：http://hhe.sxryk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hvd.jinqigufen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lmg.uphjek.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fky.xuanzx.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xcs.hfpthk.cn

Ruby: (0...10).step(2).to_a
来源：http://ffa.yj20258888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xqz.daria6918.cn

[B12] 跳出多层循环
来源：http://uig.sweek.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wbh.bbcook.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://vye.hcnkem.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xec.aizwys.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dnl.pengpengdd.cyou

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ium.mhx1999.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mxp.guannengcc.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cvp.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iso.yfazqb.com

[B13] 判断是否为数字
来源：http://stl.xuetiantiany.cn

Py:   isinstance(x, (int, float))
来源：http://zkh.zhixingplan.top

PHP:  is_numeric($x)
来源：http://kyy.yongpay.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mwf.bbcook.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gqh.wangshuangyany.cn

Java: x instanceof Number
来源：http://srm.zdbjq.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ljz.quarkkingdee.top

Ruby: x.is_a?(Numeric)
来源：http://odx.zhoulong.xyz

C#:   x is int or double or decimal
来源：http://bkp.aizwys.cn

[B14] 判断值是否在集合内
来源：http://wnk.ppjwa.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://prt.svipenyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://agp.ivvv.top

JS:   [1, 2, 3].includes(x)
来源：http://uno.0kj1m.cn

TS:   [1, 2, 3].includes(x)
来源：http://fdg.dashuyun.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://dhx.daxiang520.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vhs.9152youxi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pih.cqqwz.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://zti.9152youxi.cn

[B15] 布尔运算与取反
来源：http://ome.wangdashe.top

Py:   a and b or not c
来源：http://omv.sxryk.cn

PHP:  $a && $b || !$c
来源：http://asr.gogol.net.cn

JS:   a && b || !c
来源：http://blh.chenjidiqi.icu

TS:   a && b || !c
来源：http://hqm.yuxming.cn

Java: a && b || !c
来源：http://ifo.hnxiangtu.top

Go:   a && b || !c
来源：http://cxb.sufxvd.cn

Ruby: a && b || !c
来源：http://gta.wangdashe.top

C#:   a && b || !c
来源：http://oif.shangyingyoupin.top

[B16] 卫语句：不满足条件提前返回
来源：http://qms.xuanzx.com

Py:   if not data: return
来源：http://cis.jqgufenzy.top

PHP:  if (!$data) { return; }
来源：http://nqm.tianlin.xyz

JS:   if (!data) return;
来源：http://qsu.ppjwa.cn

TS:   if (!data) return;
来源：http://njp.tarul.cn

Java: if (data == null) return;
来源：http://hjf.shangyingyoupin.top

Go:   if data == nil { return }
来源：http://grp.wangdashe.top

Ruby: return if data.nil?
来源：http://ytu.tianlin.xyz

C#:   if (data == null) return;
来源：http://ale.andypj.xyz

================================================================================
来源：http://usn.yfazqb.com

C. 函数与作用域
来源：http://ljq.pengpengdd.cyou

================================================================================
来源：http://qvo.xylfe.cn

[C01] 定义函数
来源：http://zys.zhiwuduotai.top

Py:   def add(a, b): return a + b
来源：http://ftb.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wcw.dianchejie.cn

JS:   function add(a, b) { return a + b; }
来源：http://oek.shanyushiyangkeji.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sur.xuanzx.com

Java: static int add(int a, int b) { return a + b; }
来源：http://ukp.zdqjudy.top

Go:   func add(a, b int) int { return a + b }
来源：http://txg.meibo888.top

Ruby: def add(a, b); a + b; end
来源：http://iys.fehbvm.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qia.zycfv.cn

[C02] 默认参数
来源：http://dva.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://eeb.zycfv.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://kxz.pengpengdd.cyou

JS:   function greet(name = "World") { return name; }
来源：http://rgd.hesvh.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cxz.nanxinkj.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rhf.fzhhl.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pax.svipenyu.cn

Ruby: def greet(name = "World") = name
来源：http://ten.yangfankeji.com

C#:   string Greet(string name = "World") => name;
来源：http://sek.nwbrower.top

[C03] 可变参数
来源：http://jnn.fengsongda.top

Py:   def total(*args): return sum(args)
来源：http://mjx.tarul.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fif.sysykeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://brn.yvedp.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://jkl.zdbjq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wem.ywan-chungtsiang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://aoh.chenlongwang.top

Ruby: def total(*nums); nums.sum; end
来源：http://lfv.gotoacloud.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://kqc.fengsongda.top

[C04] 命名参数 / 关键字参数
来源：http://his.zhixingplan.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ifw.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rej.ppjwa.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dyc.ctjpmb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sbr.bbcook.cn

Java: // 无：用 Builder 模式或 record
来源：http://pyb.nanxuanxn.top


<!-- 参考信息 -->