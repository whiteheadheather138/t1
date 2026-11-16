代发 wailian999

Java: "第一行\n第二行"
来源：http://keh.shzxlz.cn

Go:   "第一行\n第二行"
来源：http://ltb.jqgufenzy.top

Ruby: "第一行\n第二行"
来源：http://csl.zhengqikj.top

C#:   "第一行\n第二行"
来源：http://mnx.jyoumei.cn

[A14] 注释写法
来源：http://vzp.andypj.xyz

Py:   # 单行；三引号字符串可作多行说明
来源：http://jkz.chenlongwang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://xku.sufxvd.cn

JS:   // 单行；/* 多行 */
来源：http://awr.jiagoushi.top

TS:   // 单行；/* 多行 */
来源：http://ice.aizwys.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://huq.shzxlz.cn

Go:   // 单行；/* 多行 */
来源：http://dhp.yvedp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://xgl.aibaodan.cn

C#:   // 单行；/* 多行 */
来源：http://vcf.yuanzhike.top

[A15] 空值判断与默认值
来源：http://ayn.xuetiantiany.cn

Py:   value = data or "默认值"
来源：http://fuz.zhongyouzk.top

PHP:  $value = $data ?? "默认值";
来源：http://ufk.ppjwa.cn

JS:   const value = data ?? "默认值";
来源：http://ibp.sxryk.cn

TS:   const value = data ?? "默认值";
来源：http://lto.nanxinkj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hqj.yueranfly.top

Go:   if data == "" { data = "默认值" }
来源：http://vuw.ydzc1.top

Ruby: value = data || "默认值"
来源：http://jml.hammf.cn

C#:   var value = data ?? "默认值";
来源：http://xce.9152youxi.cn

[A16] 真假值判断规则
来源：http://xgk.jinyuanbaomall.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vof.bbcook.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://bjd.nanxuanxn.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zen.jinyuanbaomall.cn

TS:   if (!x) {}
来源：http://rku.sysykeji.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zlc.guowangkeji.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kjs.sufxvd.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ngs.shuidangran.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xls.jqgfzy.top

[A17] 位运算
来源：http://iug.tarul.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qgi.hnxiangtu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://kzc.hcnkem.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qjn.ehwqpu.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://upt.sufxvd.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ked.tanke756.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://osq.ehwqpu.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uyz.jinghuilouyu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pmz.snrcjt.cn

[A18] 字符与 ASCII 码互转
来源：http://gch.ydjk.org.cn

Py:   ord("A"); chr(65)
来源：http://udi.ydzc1.top

PHP:  ord("A"); chr(65)
来源：http://sze.shanyushiyangtech.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://syd.fanxiaobao.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uxn.wangdashe.top

Java: (int) 'A'; (char) 65
来源：http://rhz.shangyingyoupin.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pfc.daria6918.cn

Ruby: "A".ord; 65.chr
来源：http://gze.xingfuxueyuan.xyz

C#:   (int)'A'; (char)65
来源：http://seh.jinqigufen.top

[A19] 交换两个变量
来源：http://nkz.jlsjyb.cn

Py:   a, b = b, a
来源：http://ezw.fzhhl.top

PHP:  [$a, $b] = [$b, $a];
来源：http://pcl.guowangkeji.top

JS:   [a, b] = [b, a];
来源：http://afq.epnwcf.com

TS:   [a, b] = [b, a];
来源：http://fxq.quarkkingdee.top

Java: int t = a; a = b; b = t;
来源：http://eop.gogol.net.cn

Go:   a, b = b, a
来源：http://tfk.uphjek.com

Ruby: a, b = b, a
来源：http://eot.yvedp.cn

C#:   (a, b) = (b, a);
来源：http://cmi.zhiwuduotai.top

[A20] 读取标准输入
来源：http://lvi.shzxlz.cn

Py:   name = input("请输入：")
来源：http://ysh.ivvv.top

PHP:  $name = trim(fgets(STDIN));
来源：http://lrw.feifeiyinyue.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://uoc.xuetiantiany.cn

TS:   // Node.js：readline 模块
来源：http://suk.daxiang520.top

Java: new Scanner(System.in).nextLine()
来源：http://wva.gogol.net.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://pxl.epnwcf.com

Ruby: gets.chomp
来源：http://yxi.andypj.xyz

C#:   Console.ReadLine();
来源：http://ljy.xylfe.cn

[A21] 保留指定小数位输出
来源：http://fij.tanke756.top

Py:   f"{3.14159:.2f}"
来源：http://acj.yanxiufei.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ajg.andypj.xyz

JS:   (3.14159).toFixed(2)
来源：http://daq.yanxiufei.cn

TS:   (3.14159).toFixed(2)
来源：http://vwa.xziqi.cn

Java: String.format("%.2f", 3.14159)
来源：http://udv.yfazqb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ytk.zhixingplan.top

Ruby: format("%.2f", 3.14159)
来源：http://myl.yfazqb.com

C#:   3.14159.ToString("F2")
来源：http://mra.vqdsnc.cn

[A22] 获取字符串长度
来源：http://zyr.zdbjq.cn

Py:   len(s)
来源：http://sfm.fanxiaobao.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nga.gotoacloud.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://vid.xziqi.cn

TS:   s.length
来源：http://vru.sufxvd.cn

Java: s.length()
来源：http://nna.yvedp.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xpv.yfazqb.com

Ruby: s.length
来源：http://ujr.yueranfly.top

C#:   s.Length
来源：http://vcr.nanxinkj.top

[A23] 大小写转换
来源：http://env.nanxuanxn.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ueo.jqgfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://osx.daria6918.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nwn.vqdsnc.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zzl.52xcode.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://kas.chenjidiqi.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://soy.tanke756.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zob.ppjwa.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zwp.xylfe.cn

[A24] 去除首尾空白
来源：http://ssw.zhongyouzk.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://oqr.birdmap.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nyh.kuanghao11.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dnx.jyoumei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zqn.nwbrower.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dlj.bjfxy.top

Go:   strings.TrimSpace(s)
来源：http://ipd.quarkkingdee.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://euc.yongpay.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cxs.fehbvm.com

[A25] 字符串比较
来源：http://nlo.daria6918.cn

Py:   s1 == s2; s1 != s2
来源：http://dop.yueranfly.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ewo.shanyushiyangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fep.hysaishi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tel.ywan-chungtsiang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gbr.0kj1m.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yku.zhengqikj.top

Ruby: s1 == s2; s1 <=> s2
来源：http://muc.yueranfly.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jmt.hnxiangtu.top

[A26] 类型转换总览
来源：http://vjn.havefunace.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jou.bjfxy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gln.guannengcc.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sax.tarul.cn

TS:   Number() String() Boolean() x as number
来源：http://ktq.zdbjq.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ggr.redwolf501.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://chj.mhx1999.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://pry.ivvv.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hfy.aibaodan.cn

================================================================================
来源：http://gjs.hongshengwenyu.top

B. 流程控制
来源：http://fcg.yvedp.cn

================================================================================
来源：http://sqx.zhongyouzk.top

[B01] 条件判断 if / else
来源：http://kas.hnxiangtu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rie.sweek.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rew.sysykeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fip.xuanzx.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bha.dashuyun.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://amg.hysaishi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pvt.xylfe.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fym.yj202588.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lfi.gaohongyu789.top

[B02] 多分支 else if / elif
来源：http://kyu.aibaodan.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://zmk.pengpengdd.cyou

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mvd.hysaishi.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lzz.c1oappe.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://crc.zycfv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mnb.sufxvd.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tqv.smart0.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xzf.ivvv.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ckz.zhengqikj.top

[B03] switch / match / case
来源：http://aru.pengpengdd.cyou

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cgn.wangdashe.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://moo.birdmap.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tmc.snrcjt.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tzh.sxryk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jgc.xziqi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vsg.ybcxt.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xvd.svipenyu.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://fpe.yuanzhike.top

[B04] for 计数循环
来源：http://lfm.ppjwa.cn

Py:   for i in range(10): print(i)
来源：http://xvb.hammf.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zrf.pengpengdd.cyou

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rjs.52xcode.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cam.aibaodan.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uvm.zhongyouzk.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fts.zhongyouzk.top

Ruby: 10.times { |i| puts i }
来源：http://aqz.zycfv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://spj.xylfe.cn

[B05] 遍历数组 / 列表
来源：http://mwj.iojbl.cn

Py:   for item in arr: print(item)
来源：http://khj.wangshuangyany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://meo.hnxiangtu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ptl.0kj1m.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mbj.gotoacloud.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tpv.52xcode.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ohw.zdbjq.cn

Ruby: arr.each { |item| puts item }
来源：http://pam.shzxlz.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://quc.mhx1999.top

[B06] 遍历字典 / 对象
来源：http://buy.cashguo.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bsn.yvedp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ofp.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lmt.xuetiantiany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hep.hysaishi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lfw.bbcook.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wmi.uphjek.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ang.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://rcr.uphjek.com

[B07] while 循环
来源：http://yyf.zdbjq.cn

Py:   while i < 10: i += 1
来源：http://fke.xingfuxueyuan.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://waj.zhijiandao.cn

JS:   while (i < 10) { i++; }
来源：http://rme.tanke756.top

TS:   while (i < 10) { i++; }
来源：http://umt.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://xjt.wangdashe.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jpq.tarul.cn

Ruby: while i < 10; i += 1; end
来源：http://olx.andypj.xyz

C#:   while (i < 10) { i++; }
来源：http://kgk.yongpay.top

[B08] do-while（至少执行一次）
来源：http://ogn.shanyushiyangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://yco.redwolf501.top

PHP:  do { $i++; } while ($i < 10);
来源：http://utj.xuetiantiany.cn

JS:   do { i++; } while (i < 10);
来源：http://hpk.shanyushiyangkeji.top

TS:   do { i++; } while (i < 10);
来源：http://duw.tian-w.cn

Java: do { i++; } while (i < 10);
来源：http://xgk.zhengqikj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bez.jiagoushi.top

Ruby: begin; i += 1; end while i < 10
来源：http://dzi.meibo888.top

C#:   do { i++; } while (i < 10);
来源：http://okx.tanke756.top

[B09] break 与 continue
来源：http://pvw.xylfe.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mqh.nanxinkj.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://yki.316326.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mka.mhx1999.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://oao.kuanghao11.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zhz.haohaochexian.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://uhc.wangshuangyany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uxg.sjlbkw.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wlg.hnxiangtu.top

[B10] 遍历同时拿索引
来源：http://gyr.wangdashe.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ixp.yvedp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://czj.xuanzx.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://nox.sufxvd.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://omg.cheryme.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qzw.ivvv.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pkv.hammf.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hna.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://idc.cashguo.top

[B11] 生成数字序列 / 区间
来源：http://syn.jianghu66.top

Py:   list(range(0, 10, 2))
来源：http://sgk.hfpthk.cn

PHP:  range(0, 10, 2);
来源：http://out.xuanzx.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vka.pengpengdd.cyou

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tcy.hongshengwenyu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://qxh.sweek.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tkj.9152youxi.cn

Ruby: (0...10).step(2).to_a
来源：http://ezy.zdbjq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://osp.0kj1m.cn

[B12] 跳出多层循环
来源：http://xso.xuanzx.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://ljp.tianlin.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://equ.xziqi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ljb.ivvv.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ezv.vehdjk.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fth.chenjidiqi.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tsk.sxryk.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://txd.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wbd.wangdashe.top

[B13] 判断是否为数字
来源：http://vyq.hongshengwenyu.top

Py:   isinstance(x, (int, float))
来源：http://fne.birdmap.top

PHP:  is_numeric($x)
来源：http://rdr.ydzc1.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wyt.gaohongyu789.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yrl.yangfankeji.com

Java: x instanceof Number
来源：http://cig.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rem.jqgufenzy.top

Ruby: x.is_a?(Numeric)
来源：http://snv.316326.xyz

C#:   x is int or double or decimal
来源：http://tfp.cucudq.cn

[B14] 判断值是否在集合内
来源：http://ptw.jqgfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wdu.kuanghao11.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sld.sweek.top

JS:   [1, 2, 3].includes(x)
来源：http://ppx.quarkkingdee.top

TS:   [1, 2, 3].includes(x)
来源：http://iuc.iojbl.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qjf.feifeiyinyue.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rev.xinyue.icu

Ruby: [1, 2, 3].include?(x)
来源：http://fix.nanxinkj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://jcu.mhx1999.top

[B15] 布尔运算与取反
来源：http://xsq.pycfn.com

Py:   a and b or not c
来源：http://jvc.meibo888.top

PHP:  $a && $b || !$c
来源：http://clk.epnwcf.com

JS:   a && b || !c
来源：http://fml.gzhubu.top

TS:   a && b || !c
来源：http://wjy.wangdashe.top

Java: a && b || !c
来源：http://cnx.hesvh.cn

Go:   a && b || !c
来源：http://jlv.sufxvd.cn

Ruby: a && b || !c
来源：http://fjx.hcnkem.com

C#:   a && b || !c
来源：http://hbs.sysykeji.top

[B16] 卫语句：不满足条件提前返回
来源：http://hxy.nanxuanxn.top

Py:   if not data: return
来源：http://shh.zhijiandao.cn

PHP:  if (!$data) { return; }
来源：http://pje.zdqjudy.top

JS:   if (!data) return;
来源：http://riv.hammf.cn

TS:   if (!data) return;
来源：http://xzm.guannengcc.top

Java: if (data == null) return;
来源：http://thh.gzhubu.top

Go:   if data == nil { return }
来源：http://eyn.kuanghao11.cn

Ruby: return if data.nil?
来源：http://ltf.shanyushiyangtech.top

C#:   if (data == null) return;
来源：http://fsg.jqgufenzy.top

================================================================================
来源：http://vma.xylfe.cn

C. 函数与作用域
来源：http://ieh.9152youxi.cn

================================================================================
来源：http://piv.tarul.cn

[C01] 定义函数
来源：http://tbu.cheryme.top

Py:   def add(a, b): return a + b
来源：http://kid.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jte.nwbrower.top

JS:   function add(a, b) { return a + b; }
来源：http://kkd.fzhhl.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://exb.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://tej.uphjek.com

Go:   func add(a, b int) int { return a + b }
来源：http://cmf.jqgfzy.top

Ruby: def add(a, b); a + b; end
来源：http://vyp.zhijiandao.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://etn.daxiang520.top

[C02] 默认参数
来源：http://bpm.jinqigfzy.top

Py:   def greet(name="World"): return name
来源：http://uyl.jyoumei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://bde.yj20258888.top

JS:   function greet(name = "World") { return name; }
来源：http://ozr.xinyue.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://oly.tanke756.top

Java: // 无默认参数：方法重载或 Optional
来源：http://vzn.hywenlv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gpu.snrcjt.cn

Ruby: def greet(name = "World") = name
来源：http://imw.vehdjk.com

C#:   string Greet(string name = "World") => name;
来源：http://nou.guowangkeji.top

[C03] 可变参数
来源：http://dlt.jinghuilouyu.cn

Py:   def total(*args): return sum(args)
来源：http://noj.chenjidiqi.icu

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qua.quarkkingdee.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vix.ivvv.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ety.zhongyouzk.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dgc.hammf.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mos.zhiwuduotai.top

Ruby: def total(*nums); nums.sum; end
来源：http://zyn.epnwcf.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ini.svipenyu.cn

[C04] 命名参数 / 关键字参数
来源：http://hxw.andypj.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ayw.9152youxi.cn


<!-- 参考信息 -->