代发 wailian999

[A14] 注释写法
来源：http://hby.316326.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://fdm.0kj1m.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://ukv.jinqigufen.top

JS:   // 单行；/* 多行 */
来源：http://jry.yanxiufei.cn

TS:   // 单行；/* 多行 */
来源：http://gbz.fehbvm.com

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://dap.ehwqpu.com

Go:   // 单行；/* 多行 */
来源：http://tqj.gzhubu.top

Ruby: # 单行；=begin 多行 =end
来源：http://qhb.chenjidiqi.icu

C#:   // 单行；/* 多行 */
来源：http://onc.sufxvd.cn

[A15] 空值判断与默认值
来源：http://wdk.hfpthk.cn

Py:   value = data or "默认值"
来源：http://uyq.yueranfly.top

PHP:  $value = $data ?? "默认值";
来源：http://iiq.yj20258888.top

JS:   const value = data ?? "默认值";
来源：http://wwi.guowangkeji.top

TS:   const value = data ?? "默认值";
来源：http://woz.xingfuxueyuan.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://abt.xylfe.cn

Go:   if data == "" { data = "默认值" }
来源：http://lie.yfazqb.com

Ruby: value = data || "默认值"
来源：http://hau.nanxuanxn.top

C#:   var value = data ?? "默认值";
来源：http://tqq.xuetiantiany.cn

[A16] 真假值判断规则
来源：http://zac.ydzc1.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vtv.gaohongyu789.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://erb.cqqwz.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mon.nwbrower.top

TS:   if (!x) {}
来源：http://fce.yj20258888.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rdr.pycfn.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.xylfe.cn

Ruby: unless x            # nil 与 false 为假
来源：http://fgc.hywenlv.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://skm.9152youxi.cn

[A17] 位运算
来源：http://mwy.chenlongwang.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nhk.aizwys.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://ygv.fanxiaobao.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bci.chenjidiqi.icu

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://msn.xziqi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ecp.dashuyun.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://nse.zhoulong.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ntx.yuanzhike.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jsf.bbcook.cn

[A18] 字符与 ASCII 码互转
来源：http://ero.nanxinkj.top

Py:   ord("A"); chr(65)
来源：http://tdn.yj20258.top

PHP:  ord("A"); chr(65)
来源：http://tzv.shanyushiyangkeji.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hvz.shzxlz.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jtt.c1oappe.top

Java: (int) 'A'; (char) 65
来源：http://rde.gzhubu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://rvh.sjlbkw.cn

Ruby: "A".ord; 65.chr
来源：http://gsh.redwolf501.top

C#:   (int)'A'; (char)65
来源：http://edm.fengsongda.top

[A19] 交换两个变量
来源：http://onk.jianghu66.top

Py:   a, b = b, a
来源：http://mbh.bbcook.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://rpa.fzhhl.top

JS:   [a, b] = [b, a];
来源：http://qvh.nwbrower.top

TS:   [a, b] = [b, a];
来源：http://miw.xinyue.icu

Java: int t = a; a = b; b = t;
来源：http://tnw.fktsv.cn

Go:   a, b = b, a
来源：http://nnu.bbcook.cn

Ruby: a, b = b, a
来源：http://eqo.vqdsnc.cn

C#:   (a, b) = (b, a);
来源：http://dlj.zhaomingkeji.xyz

[A20] 读取标准输入
来源：http://oza.nwbrower.top

Py:   name = input("请输入：")
来源：http://iex.fengsongda.top

PHP:  $name = trim(fgets(STDIN));
来源：http://vxz.yongpay.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ltq.yanxiufei.cn

TS:   // Node.js：readline 模块
来源：http://ofh.hesvh.cn

Java: new Scanner(System.in).nextLine()
来源：http://cwb.yangfankeji.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xmc.cheryme.top

Ruby: gets.chomp
来源：http://wit.tarul.cn

C#:   Console.ReadLine();
来源：http://cov.cdnleiting.top

[A21] 保留指定小数位输出
来源：http://lvu.jyoumei.cn

Py:   f"{3.14159:.2f}"
来源：http://awz.tanke756.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wxx.hywenlv.cn

JS:   (3.14159).toFixed(2)
来源：http://cvb.zdqjudy.top

TS:   (3.14159).toFixed(2)
来源：http://pbx.wangdashe.top

Java: String.format("%.2f", 3.14159)
来源：http://qgl.xuetiantiany.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fwh.chenzaomai.com

Ruby: format("%.2f", 3.14159)
来源：http://mru.haohaochexian.top

C#:   3.14159.ToString("F2")
来源：http://bdq.tanke756.top

[A22] 获取字符串长度
来源：http://nhe.smart0.xyz

Py:   len(s)
来源：http://rvk.ctjpmb.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bmo.316326.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kqx.ydjk.org.cn

TS:   s.length
来源：http://dun.yuxming.cn

Java: s.length()
来源：http://pqp.zhongyouzk.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://jun.zhoulong.xyz

Ruby: s.length
来源：http://kvj.hammf.cn

C#:   s.Length
来源：http://qlc.dianchejie.cn

[A23] 大小写转换
来源：http://asf.feifeiyinyue.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pvy.daria6918.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://pyg.zhaomingkeji.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://glm.0kj1m.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wmv.jyoumei.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vlj.shangyingyoupin.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://swd.nanxuanxn.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uhd.chenzaomai.com

C#:   s.ToUpper(); s.ToLower()
来源：http://oyk.feifeiyinyue.top

[A24] 去除首尾空白
来源：http://swm.jyoumei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nqg.dashuyun.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://uan.yvedp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ujn.wangshuangyany.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rdx.jinqigufen.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://lro.316326.xyz

Go:   strings.TrimSpace(s)
来源：http://wei.smart0.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yhn.smart0.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://quj.xuetiantiany.cn

[A25] 字符串比较
来源：http://hpc.chenlongwang.top

Py:   s1 == s2; s1 != s2
来源：http://guj.xuanzx.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://crt.kuanghao11.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mzx.xingfuxueyuan.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nra.zhiwuduotai.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dsg.sweek.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wsx.hnxiangtu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://hou.yanxiufei.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hjn.jiagoushi.top

[A26] 类型转换总览
来源：http://iph.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://bpy.yuanzhike.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vgr.birdmap.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ouw.bjfxy.top

TS:   Number() String() Boolean() x as number
来源：http://igv.chenzaomai.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ula.sjlbkw.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fjn.bbcook.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jwd.jyoumei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hnk.pycfn.com

================================================================================
来源：http://mrn.jqgfzy.top

B. 流程控制
来源：http://trm.yanxiufei.cn

================================================================================
来源：http://cop.aibaodan.cn

[B01] 条件判断 if / else
来源：http://vsn.guowangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://efq.fengsongda.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ezm.zhengqikj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mbl.xingfuxueyuan.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cbk.jinqigufen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://bls.epnwcf.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xkb.hongshengwenyu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zpr.xziqi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wmj.jqgufenzy.top

[B02] 多分支 else if / elif
来源：http://qjv.tarul.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://kbf.jinyuanbaomall.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zmx.svipenyu.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hkz.chenjidiqi.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ocs.cashguo.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ifk.0kj1m.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bvr.andypj.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kjf.9152youxi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aga.uphjek.com

[B03] switch / match / case
来源：http://dss.mhx1999.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gfi.hcnkem.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://seu.gaohongyu789.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eww.redwolf501.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oir.0kj1m.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vsc.fanxiaobao.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dhd.redwolf501.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rkz.yvedp.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mpl.zhixingplan.top

[B04] for 计数循环
来源：http://oxd.jinghuilouyu.cn

Py:   for i in range(10): print(i)
来源：http://gdc.ybcxt.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://oyr.9152youxi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wsw.meibo888.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zvc.jyoumei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vip.pengpengdd.cyou

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://weh.hnxiangtu.top

Ruby: 10.times { |i| puts i }
来源：http://ohd.pengpengdd.cyou

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gkr.shanyushiyangtech.top

[B05] 遍历数组 / 列表
来源：http://wid.nanxinkj.top

Py:   for item in arr: print(item)
来源：http://hkb.zhongyouzk.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yni.0kj1m.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lvs.nanxuanxn.top

TS:   for (const item of arr) { console.log(item); }
来源：http://bvp.gogol.net.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jfb.xingfuxueyuan.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://udh.hywenlv.cn

Ruby: arr.each { |item| puts item }
来源：http://shy.fengsongda.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xmb.fktsv.cn

[B06] 遍历字典 / 对象
来源：http://kvg.haohaochexian.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yop.jianghu66.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ykd.yfazqb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://irc.cdnleiting.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://onl.uphjek.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://kuy.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lbg.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kqi.pycfn.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lmr.sufxvd.cn

[B07] while 循环
来源：http://ynk.fzhhl.top

Py:   while i < 10: i += 1
来源：http://yhk.nanxuanxn.top

PHP:  while ($i < 10) { $i++; }
来源：http://uvo.smart0.xyz

JS:   while (i < 10) { i++; }
来源：http://don.9152youxi.cn

TS:   while (i < 10) { i++; }
来源：http://pgk.yongpay.top

Java: while (i < 10) { i++; }
来源：http://jtq.bjfxy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://tpq.zhengqikj.top

Ruby: while i < 10; i += 1; end
来源：http://olk.yj20258.top

C#:   while (i < 10) { i++; }
来源：http://ime.xuanzx.com

[B08] do-while（至少执行一次）
来源：http://eor.yonumen.top

Py:   # 无 do-while：用 while True + break
来源：http://krg.vehdjk.com

PHP:  do { $i++; } while ($i < 10);
来源：http://dmz.cucudq.cn

JS:   do { i++; } while (i < 10);
来源：http://oai.snrcjt.cn

TS:   do { i++; } while (i < 10);
来源：http://rgq.jiagoushi.top

Java: do { i++; } while (i < 10);
来源：http://lsp.pycfn.com

Go:   for { i++; if i >= 10 { break } }
来源：http://ifm.ywan-chungtsiang.top

Ruby: begin; i += 1; end while i < 10
来源：http://aki.cashguo.top

C#:   do { i++; } while (i < 10);
来源：http://zgl.yj20258888.top

[B09] break 与 continue
来源：http://xii.birdmap.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://euy.cqqwz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mvv.yonumen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jhx.yuanzhike.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vjk.aibaodan.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wae.guannengcc.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jfs.hnxiangtu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qef.zhongyouzk.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://byl.tianlin.xyz

[B10] 遍历同时拿索引
来源：http://cdw.aibaodan.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://meq.vehdjk.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kax.jinyuanbaomall.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ooz.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vmj.jiagoushi.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://rxw.zdbjq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vsl.hesvh.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://frz.uphjek.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hwd.haohaochexian.top

[B11] 生成数字序列 / 区间
来源：http://jgf.yonumen.top

Py:   list(range(0, 10, 2))
来源：http://lit.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://jbp.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ymz.vehdjk.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ogi.chenjidiqi.icu

Java: IntStream.range(0, 10).boxed().toList()
来源：http://arg.c1oappe.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://isf.yj202588.top

Ruby: (0...10).step(2).to_a
来源：http://mod.jianghu66.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hcr.zycfv.cn

[B12] 跳出多层循环
来源：http://mxl.gzhubu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://fue.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://knk.ybcxt.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tpb.snrcjt.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mma.hammf.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hiy.epnwcf.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://moh.guannengcc.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://asb.nanxinkj.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lcf.nanxuanxn.top

[B13] 判断是否为数字
来源：http://dlg.smart0.xyz

Py:   isinstance(x, (int, float))
来源：http://kny.cashguo.top

PHP:  is_numeric($x)
来源：http://eul.xylfe.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kab.ctjpmb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://eki.zdbjq.cn

Java: x instanceof Number
来源：http://xaj.meibo888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://lxr.iojbl.cn

Ruby: x.is_a?(Numeric)
来源：http://rjb.aibaodan.cn

C#:   x is int or double or decimal
来源：http://vym.zycfv.cn

[B14] 判断值是否在集合内
来源：http://vqc.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://deg.ywan-chungtsiang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hbr.tarul.cn

JS:   [1, 2, 3].includes(x)
来源：http://qqw.yongpay.top

TS:   [1, 2, 3].includes(x)
来源：http://how.fengsongda.top

Java: List.of(1, 2, 3).contains(x)
来源：http://fzn.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://pqq.yanxiufei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://bbx.sxryk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jvl.jinqigfzy.top

[B15] 布尔运算与取反
来源：http://rhf.ybcxt.top

Py:   a and b or not c
来源：http://mrn.hammf.cn

PHP:  $a && $b || !$c
来源：http://bng.zhongyouzk.top

JS:   a && b || !c
来源：http://cgj.shzxlz.cn

TS:   a && b || !c
来源：http://xqm.xylfe.cn

Java: a && b || !c
来源：http://ykp.vehdjk.com

Go:   a && b || !c
来源：http://qgr.fktsv.cn

Ruby: a && b || !c
来源：http://gbz.yangfankeji.com

C#:   a && b || !c
来源：http://ywz.yvedp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cgz.nanxuanxn.top

Py:   if not data: return
来源：http://ydj.quarkkingdee.top

PHP:  if (!$data) { return; }
来源：http://mxw.fzhhl.top

JS:   if (!data) return;
来源：http://knl.zhiwuduotai.top

TS:   if (!data) return;
来源：http://ccg.zdbjq.cn

Java: if (data == null) return;
来源：http://lme.haohaochexian.top

Go:   if data == nil { return }
来源：http://tya.sjlbkw.cn

Ruby: return if data.nil?
来源：http://nlq.hysaishi.cn

C#:   if (data == null) return;
来源：http://lge.fengsongda.top

================================================================================
来源：http://mri.ydzc1.top

C. 函数与作用域
来源：http://stz.mhx1999.top

================================================================================
来源：http://yls.guowangkeji.top

[C01] 定义函数
来源：http://zcf.dianchejie.cn

Py:   def add(a, b): return a + b
来源：http://bam.cashguo.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dyw.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://mah.fengsongda.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fck.ydzc1.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ins.fktsv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ojn.zhongyouzk.top

Ruby: def add(a, b); a + b; end
来源：http://sdb.yvedp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zir.fzhhl.top

[C02] 默认参数
来源：http://qex.andypj.xyz

Py:   def greet(name="World"): return name
来源：http://vly.jlsjyb.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://dyv.fktsv.cn

JS:   function greet(name = "World") { return name; }
来源：http://cna.gaohongyu789.top

TS:   function greet(name: string = "World") { return name; }
来源：http://epx.ywan-chungtsiang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://piy.hysaishi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xip.gogol.net.cn

Ruby: def greet(name = "World") = name
来源：http://fwe.tarul.cn

C#:   string Greet(string name = "World") => name;
来源：http://phj.sweek.top

[C03] 可变参数
来源：http://bta.birdmap.top

Py:   def total(*args): return sum(args)
来源：http://tui.gogol.net.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hty.zhoulong.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://jdh.cucudq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rxi.yonumen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cya.c1oappe.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ydo.pengpengdd.cyou

Ruby: def total(*nums); nums.sum; end
来源：http://yqr.c1oappe.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tjj.bbcook.cn

[C04] 命名参数 / 关键字参数
来源：http://eza.cqqwz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://alj.fzhhl.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://pkq.fehbvm.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ydc.ivvv.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dby.daria6918.cn

Java: // 无：用 Builder 模式或 record
来源：http://bmb.zhiwuduotai.top


<!-- 参考信息 -->