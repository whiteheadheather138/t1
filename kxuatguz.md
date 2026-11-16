代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://orv.jqgfzy.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ifm.xingfuxueyuan.xyz

Go:   // 单行；/* 多行 */
来源：http://ylw.yj20258.top

Ruby: # 单行；=begin 多行 =end
来源：http://nre.gaohongyu789.top

C#:   // 单行；/* 多行 */
来源：http://pto.hnqzz.top

[A15] 空值判断与默认值
来源：http://cad.yuxming.cn

Py:   value = data or "默认值"
来源：http://xnx.zhaomingkeji.xyz

PHP:  $value = $data ?? "默认值";
来源：http://ojm.zhongyouzk.top

JS:   const value = data ?? "默认值";
来源：http://ylv.fehbvm.com

TS:   const value = data ?? "默认值";
来源：http://drl.smart0.xyz

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pvg.yvedp.cn

Go:   if data == "" { data = "默认值" }
来源：http://sen.yangfankeji.com

Ruby: value = data || "默认值"
来源：http://vrg.hysaishi.cn

C#:   var value = data ?? "默认值";
来源：http://obq.havefunace.top

[A16] 真假值判断规则
来源：http://rvp.sweek.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rqs.zhiwuduotai.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ckd.shanyushiyangtech.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fmn.yongpay.top

TS:   if (!x) {}
来源：http://mfw.jianghu66.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wqe.yangfankeji.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://sot.jinyuanbaomall.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vow.ehwqpu.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vfc.mhx1999.top

[A17] 位运算
来源：http://qfk.feifeiyinyue.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://poh.zycfv.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uub.iojbl.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iyf.tarul.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wtj.xinyue.icu

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yfu.cqqwz.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wni.ybcxt.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://giv.smart0.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ges.pengpengdd.cyou

[A18] 字符与 ASCII 码互转
来源：http://rak.mhx1999.top

Py:   ord("A"); chr(65)
来源：http://imo.zhijiandao.cn

PHP:  ord("A"); chr(65)
来源：http://frf.yangfankeji.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rkk.redwolf501.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://scc.andypj.xyz

Java: (int) 'A'; (char) 65
来源：http://uqk.hywenlv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mgs.daxiang520.top

Ruby: "A".ord; 65.chr
来源：http://jdy.kuanghao11.cn

C#:   (int)'A'; (char)65
来源：http://tfr.c1oappe.top

[A19] 交换两个变量
来源：http://wuh.xuanzx.com

Py:   a, b = b, a
来源：http://dug.xuanzx.com

PHP:  [$a, $b] = [$b, $a];
来源：http://smq.birdmap.top

JS:   [a, b] = [b, a];
来源：http://vel.316326.xyz

TS:   [a, b] = [b, a];
来源：http://ove.fehbvm.com

Java: int t = a; a = b; b = t;
来源：http://tvw.yj202588.top

Go:   a, b = b, a
来源：http://rwu.shzxlz.cn

Ruby: a, b = b, a
来源：http://sdz.hcnkem.com

C#:   (a, b) = (b, a);
来源：http://wqe.svipenyu.cn

[A20] 读取标准输入
来源：http://vne.cheryme.top

Py:   name = input("请输入：")
来源：http://yij.gogol.net.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://unx.ydzc1.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ngd.bjfxy.top

TS:   // Node.js：readline 模块
来源：http://lbl.yvedp.cn

Java: new Scanner(System.in).nextLine()
来源：http://gcu.redwolf501.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://zty.jinyuanbaomall.cn

Ruby: gets.chomp
来源：http://yvt.sufxvd.cn

C#:   Console.ReadLine();
来源：http://nls.hammf.cn

[A21] 保留指定小数位输出
来源：http://ebf.gzhubu.top

Py:   f"{3.14159:.2f}"
来源：http://bjt.jinghuilouyu.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vka.wangshuangyany.cn

JS:   (3.14159).toFixed(2)
来源：http://sqr.cucudq.cn

TS:   (3.14159).toFixed(2)
来源：http://yau.sjlbkw.cn

Java: String.format("%.2f", 3.14159)
来源：http://twf.yfazqb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://atk.hongshengwenyu.top

Ruby: format("%.2f", 3.14159)
来源：http://mio.316326.xyz

C#:   3.14159.ToString("F2")
来源：http://mcs.jyoumei.cn

[A22] 获取字符串长度
来源：http://wvr.vqdsnc.cn

Py:   len(s)
来源：http://zyj.ppjwa.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://naf.tarul.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tml.ppjwa.cn

TS:   s.length
来源：http://jik.chenlongwang.top

Java: s.length()
来源：http://gin.epnwcf.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://dan.tian-w.cn

Ruby: s.length
来源：http://bln.chenlongwang.top

C#:   s.Length
来源：http://iit.cqqwz.cn

[A23] 大小写转换
来源：http://nvs.vqdsnc.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rfo.yangfankeji.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://usk.hfpthk.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wqx.ywan-chungtsiang.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qku.fehbvm.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jvb.hnqzz.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zns.daria6918.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cih.yongpay.top

C#:   s.ToUpper(); s.ToLower()
来源：http://umm.316326.xyz

[A24] 去除首尾空白
来源：http://ahd.sysykeji.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wrn.cashguo.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://npw.ivvv.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aqe.zdbjq.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zka.cucudq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ula.ivvv.top

Go:   strings.TrimSpace(s)
来源：http://vuf.sxryk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tpg.bjfxy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ovy.aizwys.cn

[A25] 字符串比较
来源：http://kih.ydzc1.top

Py:   s1 == s2; s1 != s2
来源：http://jzg.hammf.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://juj.aibaodan.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fbe.sxryk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cvg.ywan-chungtsiang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://oyv.svipenyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://aay.redwolf501.top

Ruby: s1 == s2; s1 <=> s2
来源：http://znf.yj20258.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ucf.nwbrower.top

[A26] 类型转换总览
来源：http://guh.tarul.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wxz.zycfv.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mhl.fehbvm.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zoy.vqdsnc.cn

TS:   Number() String() Boolean() x as number
来源：http://bfz.hcnkem.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fku.gzhubu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wnc.jinyuanbaomall.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://hzp.quarkkingdee.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lsl.shanyushiyangkeji.top

================================================================================
来源：http://uci.shuidangran.top

B. 流程控制
来源：http://evg.gotoacloud.top

================================================================================
来源：http://eze.sufxvd.cn

[B01] 条件判断 if / else
来源：http://sfd.xingfuxueyuan.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://huq.hfpthk.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mza.sweek.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://iid.sufxvd.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rdk.hesvh.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wlq.yanxiufei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kmt.redwolf501.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jfa.daria6918.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vgk.jinyuanbaomall.cn

[B02] 多分支 else if / elif
来源：http://ucz.ppjwa.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sdr.jyoumei.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://cog.sxryk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://obl.52xcode.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wck.ehwqpu.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uig.hysaishi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://czt.zhiwuduotai.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nyv.ybcxt.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jbu.tarul.cn

[B03] switch / match / case
来源：http://lwl.zdqjudy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vzu.guannengcc.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lzk.sjlbkw.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nys.sufxvd.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://szp.tian-w.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://euw.yongpay.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bfh.chenjidiqi.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://qyi.ybcxt.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hmv.yanxiufei.cn

[B04] for 计数循环
来源：http://eue.svipenyu.cn

Py:   for i in range(10): print(i)
来源：http://ztm.ywan-chungtsiang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ewu.gotoacloud.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iii.zhixingplan.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eaz.gzhubu.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zsc.ybcxt.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dou.hesvh.cn

Ruby: 10.times { |i| puts i }
来源：http://kyq.yanxiufei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://diz.sufxvd.cn

[B05] 遍历数组 / 列表
来源：http://ivl.vehdjk.com

Py:   for item in arr: print(item)
来源：http://ppe.smart0.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yhz.sweek.top

JS:   for (const item of arr) { console.log(item); }
来源：http://opj.ybcxt.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hdl.yanxiufei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://euv.gotoacloud.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bso.fehbvm.com

Ruby: arr.each { |item| puts item }
来源：http://vhd.xylfe.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tpx.ehwqpu.com

[B06] 遍历字典 / 对象
来源：http://gds.gotoacloud.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ktn.shzxlz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://aqp.tianlin.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kth.jlsjyb.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uve.hesvh.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yde.xinyue.icu

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nrl.hnxiangtu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zph.hysaishi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ihu.sxryk.cn

[B07] while 循环
来源：http://ixk.jlsjyb.cn

Py:   while i < 10: i += 1
来源：http://oxd.zycfv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://lly.gotoacloud.top

JS:   while (i < 10) { i++; }
来源：http://ofz.yuxming.cn

TS:   while (i < 10) { i++; }
来源：http://kem.yj20258.top

Java: while (i < 10) { i++; }
来源：http://dls.gogol.net.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jfe.redwolf501.top

Ruby: while i < 10; i += 1; end
来源：http://liq.cqqwz.cn

C#:   while (i < 10) { i++; }
来源：http://ljh.jinqigfzy.top

[B08] do-while（至少执行一次）
来源：http://xoh.jinyuanbaomall.cn

Py:   # 无 do-while：用 while True + break
来源：http://nxl.bjfxy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jnd.jyoumei.cn

JS:   do { i++; } while (i < 10);
来源：http://jxv.zhixingplan.top

TS:   do { i++; } while (i < 10);
来源：http://avp.hysaishi.cn

Java: do { i++; } while (i < 10);
来源：http://clc.yj20258.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ths.zdbjq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://gim.yj202588.top

C#:   do { i++; } while (i < 10);
来源：http://oan.jqgfzy.top

[B09] break 与 continue
来源：http://ioi.jinghuilouyu.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dfl.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kud.yj20258.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://urf.jinqigfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://edg.meibo888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yfm.mhx1999.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yqu.c1oappe.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://grd.cucudq.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hgm.jyoumei.cn

[B10] 遍历同时拿索引
来源：http://vmw.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xqy.zdbjq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://fbc.0kj1m.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mjv.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://yjd.cheryme.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://pyp.hongshengwenyu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hsh.tanke756.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tto.ppjwa.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qjz.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://nml.52xcode.cn

Py:   list(range(0, 10, 2))
来源：http://kka.vqdsnc.cn

PHP:  range(0, 10, 2);
来源：http://pvx.iojbl.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hdz.vqdsnc.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ykq.tanke756.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ztk.hnxiangtu.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ngw.wangdashe.top

Ruby: (0...10).step(2).to_a
来源：http://jzk.bbcook.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://haj.52xcode.cn

[B12] 跳出多层循环
来源：http://fej.shanyushiyangtech.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jqb.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://jfv.zhongyouzk.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wbu.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vbk.0kj1m.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://xph.jinqigfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bed.redwolf501.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rtt.gotoacloud.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://cnk.gotoacloud.top

[B13] 判断是否为数字
来源：http://gcy.daxiang520.top

Py:   isinstance(x, (int, float))
来源：http://vrt.yj202588.top

PHP:  is_numeric($x)
来源：http://orn.birdmap.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hck.xuanzx.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://odr.mhx1999.top

Java: x instanceof Number
来源：http://xpx.dianchejie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zqy.nanxinkj.top

Ruby: x.is_a?(Numeric)
来源：http://jzb.tian-w.cn

C#:   x is int or double or decimal
来源：http://jcc.aibaodan.cn

[B14] 判断值是否在集合内
来源：http://ccp.c1oappe.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ows.shanyushiyangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xns.chenzaomai.com

JS:   [1, 2, 3].includes(x)
来源：http://bbv.dianchejie.cn

TS:   [1, 2, 3].includes(x)
来源：http://emm.cqqwz.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://rfn.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://agz.jinyuanbaomall.cn

Ruby: [1, 2, 3].include?(x)
来源：http://qtf.52xcode.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://svj.birdmap.top

[B15] 布尔运算与取反
来源：http://yta.snrcjt.cn

Py:   a and b or not c
来源：http://viu.epnwcf.com

PHP:  $a && $b || !$c
来源：http://nlj.fktsv.cn

JS:   a && b || !c
来源：http://dww.hnxiangtu.top

TS:   a && b || !c
来源：http://fks.zhoulong.xyz

Java: a && b || !c
来源：http://yxp.xuanzx.com

Go:   a && b || !c
来源：http://kbr.shanyushiyangtech.top

Ruby: a && b || !c
来源：http://eyb.snrcjt.cn

C#:   a && b || !c
来源：http://aue.yuxming.cn

[B16] 卫语句：不满足条件提前返回
来源：http://byr.9152youxi.cn

Py:   if not data: return
来源：http://nla.gzhubu.top

PHP:  if (!$data) { return; }
来源：http://mtf.fzhhl.top

JS:   if (!data) return;
来源：http://hxp.nwbrower.top

TS:   if (!data) return;
来源：http://znl.fanxiaobao.xyz

Java: if (data == null) return;
来源：http://lmb.nanxinkj.top

Go:   if data == nil { return }
来源：http://esx.xuanzx.com

Ruby: return if data.nil?
来源：http://ano.jqgufenzy.top

C#:   if (data == null) return;
来源：http://vac.ydzc1.top

================================================================================
来源：http://bke.tanke756.top

C. 函数与作用域
来源：http://gyb.cashguo.top

================================================================================
来源：http://vgw.ivvv.top

[C01] 定义函数
来源：http://wcx.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://hfx.dashuyun.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hre.xziqi.cn

JS:   function add(a, b) { return a + b; }
来源：http://itb.jinghuilouyu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dat.hfpthk.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://eeq.redwolf501.top

Go:   func add(a, b int) int { return a + b }
来源：http://acg.ybcxt.top

Ruby: def add(a, b); a + b; end
来源：http://ywb.cdnleiting.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wye.ehwqpu.com

[C02] 默认参数
来源：http://mdt.wangshuangyany.cn

Py:   def greet(name="World"): return name
来源：http://soy.jqgufenzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://pus.hfpthk.cn

JS:   function greet(name = "World") { return name; }
来源：http://whx.fehbvm.com

TS:   function greet(name: string = "World") { return name; }
来源：http://gsr.wangshuangyany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://thc.daria6918.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://gjo.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://nua.dianchejie.cn

C#:   string Greet(string name = "World") => name;
来源：http://hgg.zdbjq.cn

[C03] 可变参数
来源：http://bdz.nanxinkj.top

Py:   def total(*args): return sum(args)
来源：http://jks.aizwys.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://eml.tian-w.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mcr.sxryk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://svd.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pnm.bjfxy.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hmd.yueranfly.top

Ruby: def total(*nums); nums.sum; end
来源：http://bqg.fengsongda.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dln.chenlongwang.top

[C04] 命名参数 / 关键字参数
来源：http://ljt.yanxiufei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://nli.hfpthk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kek.yongpay.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://dqj.sweek.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://kop.sufxvd.cn

Java: // 无：用 Builder 模式或 record
来源：http://poq.hongshengwenyu.top

Go:   // 无：用配置结构体参数
来源：http://cun.hnxiangtu.top

Ruby: f(a: 1, b: 2)
来源：http://ttk.yj20258888.top

C#:   f(a: 1, b: 2)
来源：http://zbu.gotoacloud.top

[C05] 返回多个值
来源：http://jox.daxiang520.top


<!-- 参考信息 -->