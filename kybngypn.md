代发 wailian999

Java: "第一行\n第二行"
来源：http://xzm.smart0.xyz

Go:   "第一行\n第二行"
来源：http://mez.feifeiyinyue.top

Ruby: "第一行\n第二行"
来源：http://xcs.smart0.xyz

C#:   "第一行\n第二行"
来源：http://pol.snrcjt.cn

[A14] 注释写法
来源：http://pam.hcnkem.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://hac.yueranfly.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://krz.chenzaomai.com

JS:   // 单行；/* 多行 */
来源：http://pgu.smart0.xyz

TS:   // 单行；/* 多行 */
来源：http://xzf.yj20258888.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://qec.aibaodan.cn

Go:   // 单行；/* 多行 */
来源：http://zku.shuidangran.top

Ruby: # 单行；=begin 多行 =end
来源：http://nnn.sxryk.cn

C#:   // 单行；/* 多行 */
来源：http://skv.cqqwz.cn

[A15] 空值判断与默认值
来源：http://dba.yvedp.cn

Py:   value = data or "默认值"
来源：http://sch.guannengcc.top

PHP:  $value = $data ?? "默认值";
来源：http://mtd.fehbvm.com

JS:   const value = data ?? "默认值";
来源：http://qkl.yonumen.top

TS:   const value = data ?? "默认值";
来源：http://hsx.shzxlz.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://seu.hysaishi.cn

Go:   if data == "" { data = "默认值" }
来源：http://pzr.sweek.top

Ruby: value = data || "默认值"
来源：http://yrm.jinghuilouyu.cn

C#:   var value = data ?? "默认值";
来源：http://cfj.andypj.xyz

[A16] 真假值判断规则
来源：http://cpo.aibaodan.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xor.bjfxy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://upe.guannengcc.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zst.daxiang520.top

TS:   if (!x) {}
来源：http://wpy.shuidangran.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ghe.sxryk.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://icp.zhijiandao.cn

Ruby: unless x            # nil 与 false 为假
来源：http://mdg.bjfxy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oyk.shangyingyoupin.top

[A17] 位运算
来源：http://mvy.guowangkeji.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://etr.uphjek.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pbq.xuanzx.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://inr.daria6918.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gwg.cqqwz.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://olg.ivvv.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bfc.sysykeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hdt.yonumen.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lde.316326.xyz

[A18] 字符与 ASCII 码互转
来源：http://fkp.zdbjq.cn

Py:   ord("A"); chr(65)
来源：http://ndh.ydjk.org.cn

PHP:  ord("A"); chr(65)
来源：http://vno.fehbvm.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pfh.jinqigfzy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://itc.zhongyouzk.top

Java: (int) 'A'; (char) 65
来源：http://bep.xuetiantiany.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xhg.yongpay.top

Ruby: "A".ord; 65.chr
来源：http://zbt.jinqigufen.top

C#:   (int)'A'; (char)65
来源：http://hde.zhongyouzk.top

[A19] 交换两个变量
来源：http://roy.c1oappe.top

Py:   a, b = b, a
来源：http://fbp.zhiwuduotai.top

PHP:  [$a, $b] = [$b, $a];
来源：http://dxj.jinqigufen.top

JS:   [a, b] = [b, a];
来源：http://nwd.zhijiandao.cn

TS:   [a, b] = [b, a];
来源：http://jym.hnxiangtu.top

Java: int t = a; a = b; b = t;
来源：http://fzc.fengsongda.top

Go:   a, b = b, a
来源：http://lms.chenzaomai.com

Ruby: a, b = b, a
来源：http://wso.ybcxt.top

C#:   (a, b) = (b, a);
来源：http://ijr.0kj1m.cn

[A20] 读取标准输入
来源：http://gaa.yueranfly.top

Py:   name = input("请输入：")
来源：http://eik.yuanzhike.top

PHP:  $name = trim(fgets(STDIN));
来源：http://cad.fanxiaobao.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rcs.xingfuxueyuan.xyz

TS:   // Node.js：readline 模块
来源：http://fen.yangfankeji.com

Java: new Scanner(System.in).nextLine()
来源：http://ymv.cashguo.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hwi.daria6918.cn

Ruby: gets.chomp
来源：http://crg.0kj1m.cn

C#:   Console.ReadLine();
来源：http://zah.gotoacloud.top

[A21] 保留指定小数位输出
来源：http://bww.zdqjudy.top

Py:   f"{3.14159:.2f}"
来源：http://egs.ppjwa.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wjn.xuetiantiany.cn

JS:   (3.14159).toFixed(2)
来源：http://gvh.zhaomingkeji.xyz

TS:   (3.14159).toFixed(2)
来源：http://trg.jqgfzy.top

Java: String.format("%.2f", 3.14159)
来源：http://zzh.gotoacloud.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fmw.fanxiaobao.xyz

Ruby: format("%.2f", 3.14159)
来源：http://vhq.c1oappe.top

C#:   3.14159.ToString("F2")
来源：http://dnh.hongshengwenyu.top

[A22] 获取字符串长度
来源：http://nue.chenjidiqi.icu

Py:   len(s)
来源：http://und.fanxiaobao.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mtb.nanxuanxn.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wiu.hnxiangtu.top

TS:   s.length
来源：http://nsn.dashuyun.cn

Java: s.length()
来源：http://yjq.shangyingyoupin.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rru.dianchejie.cn

Ruby: s.length
来源：http://qgf.yfazqb.com

C#:   s.Length
来源：http://val.dashuyun.cn

[A23] 大小写转换
来源：http://zfl.meibo888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://fke.shzxlz.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kat.xingfuxueyuan.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://pvi.epnwcf.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lac.hongshengwenyu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://wtv.c1oappe.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uvz.yuanzhike.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://san.zhijiandao.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://yxi.yj202588.top

[A24] 去除首尾空白
来源：http://bvp.zhongyouzk.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ghb.zhongyouzk.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xrj.nanxuanxn.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yfk.bbcook.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ier.mhx1999.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jod.ivvv.top

Go:   strings.TrimSpace(s)
来源：http://dfh.gaohongyu789.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://fho.quarkkingdee.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://izv.jinyuanbaomall.cn

[A25] 字符串比较
来源：http://gvw.snrcjt.cn

Py:   s1 == s2; s1 != s2
来源：http://jrz.gogol.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://grm.quarkkingdee.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jqw.tian-w.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yfz.snrcjt.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://brh.zhongyouzk.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://oar.sxryk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://gwi.nanxuanxn.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://aps.daxiang520.top

[A26] 类型转换总览
来源：http://kig.vqdsnc.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://oab.birdmap.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://qcm.vqdsnc.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://knj.jinghuilouyu.cn

TS:   Number() String() Boolean() x as number
来源：http://und.fzhhl.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kig.tian-w.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ecw.zdbjq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://rzw.yongpay.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qmd.0kj1m.cn

================================================================================
来源：http://apb.bbcook.cn

B. 流程控制
来源：http://rnb.bbcook.cn

================================================================================
来源：http://ddi.guowangkeji.top

[B01] 条件判断 if / else
来源：http://las.yanxiufei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://opm.zhaomingkeji.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bsb.zdqjudy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jsl.c1oappe.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://yfo.cheryme.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://iaw.feifeiyinyue.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iti.nanxuanxn.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jus.dianchejie.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ltu.fehbvm.com

[B02] 多分支 else if / elif
来源：http://bji.cqqwz.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vqq.fktsv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lep.iojbl.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yja.shuidangran.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wqi.chenzaomai.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zvd.jqgfzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qbl.vehdjk.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kid.hysaishi.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uvj.svipenyu.cn

[B03] switch / match / case
来源：http://rpw.wangdashe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kzh.xylfe.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://syx.aizwys.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fpl.yfazqb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bjq.feifeiyinyue.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jve.ivvv.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qwb.vqdsnc.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://iqj.zycfv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ejh.hywenlv.cn

[B04] for 计数循环
来源：http://pfx.52xcode.cn

Py:   for i in range(10): print(i)
来源：http://ogm.nanxuanxn.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vbf.shangyingyoupin.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://waq.tianlin.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://obg.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jwd.chenlongwang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mgn.fzhhl.top

Ruby: 10.times { |i| puts i }
来源：http://ibe.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://axv.daxiang520.top

[B05] 遍历数组 / 列表
来源：http://pbd.shangyingyoupin.top

Py:   for item in arr: print(item)
来源：http://tdx.zhoulong.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://wil.zhongyouzk.top

JS:   for (const item of arr) { console.log(item); }
来源：http://xgo.hcnkem.com

TS:   for (const item of arr) { console.log(item); }
来源：http://rab.shuidangran.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://kxf.dashuyun.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gzj.xinyue.icu

Ruby: arr.each { |item| puts item }
来源：http://han.aibaodan.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://aeu.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://jlj.pengpengdd.cyou

Py:   for k, v in d.items(): print(k, v)
来源：http://gtf.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ivy.vqdsnc.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wwj.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://fhz.jinqigufen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hfm.chenlongwang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://tqm.zdbjq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hgu.jinghuilouyu.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xad.guowangkeji.top

[B07] while 循环
来源：http://wqm.sweek.top

Py:   while i < 10: i += 1
来源：http://waa.fktsv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fhc.yj20258888.top

JS:   while (i < 10) { i++; }
来源：http://qxs.zhiwuduotai.top

TS:   while (i < 10) { i++; }
来源：http://fwr.ppjwa.cn

Java: while (i < 10) { i++; }
来源：http://bie.316326.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://sel.xingfuxueyuan.xyz

Ruby: while i < 10; i += 1; end
来源：http://kfx.uphjek.com

C#:   while (i < 10) { i++; }
来源：http://bfz.ybcxt.top

[B08] do-while（至少执行一次）
来源：http://fqq.ybcxt.top

Py:   # 无 do-while：用 while True + break
来源：http://jgm.sxryk.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ynb.zhijiandao.cn

JS:   do { i++; } while (i < 10);
来源：http://dut.tarul.cn

TS:   do { i++; } while (i < 10);
来源：http://zbh.shanyushiyangtech.top

Java: do { i++; } while (i < 10);
来源：http://exf.gotoacloud.top

Go:   for { i++; if i >= 10 { break } }
来源：http://aab.hammf.cn

Ruby: begin; i += 1; end while i < 10
来源：http://kze.nwbrower.top

C#:   do { i++; } while (i < 10);
来源：http://djw.aibaodan.cn

[B09] break 与 continue
来源：http://czf.guowangkeji.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nln.jqgufenzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://kog.yj202588.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jil.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hig.tianlin.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lwt.cqqwz.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://osg.zhongyouzk.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pxs.jianghu66.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ndx.xziqi.cn

[B10] 遍历同时拿索引
来源：http://vqw.sysykeji.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://eju.epnwcf.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://jhd.pengpengdd.cyou

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jmo.fanxiaobao.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cux.sysykeji.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hzh.xingfuxueyuan.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fio.hcnkem.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://quv.fehbvm.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://cxi.shuidangran.top

[B11] 生成数字序列 / 区间
来源：http://rdy.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://oll.zhiwuduotai.top

PHP:  range(0, 10, 2);
来源：http://aih.tanke756.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://iky.wangshuangyany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gtw.ctjpmb.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://eii.zycfv.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gmr.vehdjk.com

Ruby: (0...10).step(2).to_a
来源：http://biq.kuanghao11.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xid.hywenlv.cn

[B12] 跳出多层循环
来源：http://pfj.sufxvd.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vjy.tanke756.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://poz.mhx1999.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ooe.shanyushiyangtech.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://gyo.yj20258.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://brt.snrcjt.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bub.bbcook.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ymn.quarkkingdee.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uzn.ybcxt.top

[B13] 判断是否为数字
来源：http://ldg.yfazqb.com

Py:   isinstance(x, (int, float))
来源：http://vkj.fehbvm.com

PHP:  is_numeric($x)
来源：http://mho.xylfe.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ccc.smart0.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pej.vehdjk.com

Java: x instanceof Number
来源：http://irr.cheryme.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://onl.tian-w.cn

Ruby: x.is_a?(Numeric)
来源：http://fzl.dashuyun.cn

C#:   x is int or double or decimal
来源：http://xyo.ybcxt.top

[B14] 判断值是否在集合内
来源：http://doc.sjlbkw.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lwt.epnwcf.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://tpq.sjlbkw.cn

JS:   [1, 2, 3].includes(x)
来源：http://obe.yj20258888.top

TS:   [1, 2, 3].includes(x)
来源：http://jre.yj202588.top

Java: List.of(1, 2, 3).contains(x)
来源：http://tvo.gogol.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jro.xuetiantiany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://rdp.yongpay.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://niy.bjfxy.top

[B15] 布尔运算与取反
来源：http://azp.zhoulong.xyz

Py:   a and b or not c
来源：http://err.nanxinkj.top

PHP:  $a && $b || !$c
来源：http://cah.shzxlz.cn

JS:   a && b || !c
来源：http://hom.jinghuilouyu.cn

TS:   a && b || !c
来源：http://zsv.mhx1999.top

Java: a && b || !c
来源：http://mzf.hfpthk.cn

Go:   a && b || !c
来源：http://olf.nanxinkj.top

Ruby: a && b || !c
来源：http://drr.jinqigufen.top

C#:   a && b || !c
来源：http://unc.bbcook.cn

[B16] 卫语句：不满足条件提前返回
来源：http://lab.yuanzhike.top

Py:   if not data: return
来源：http://hte.sweek.top

PHP:  if (!$data) { return; }
来源：http://raf.hongshengwenyu.top

JS:   if (!data) return;
来源：http://pxn.ctjpmb.com

TS:   if (!data) return;
来源：http://oqn.aizwys.cn

Java: if (data == null) return;
来源：http://spw.feifeiyinyue.top

Go:   if data == nil { return }
来源：http://mrx.shzxlz.cn

Ruby: return if data.nil?
来源：http://qkz.hnqzz.top

C#:   if (data == null) return;
来源：http://xum.shzxlz.cn

================================================================================
来源：http://ttb.zhongyouzk.top

C. 函数与作用域
来源：http://vhx.chenjidiqi.icu

================================================================================
来源：http://dyh.316326.xyz

[C01] 定义函数
来源：http://hst.cheryme.top

Py:   def add(a, b): return a + b
来源：http://nad.andypj.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://erw.ydjk.org.cn

JS:   function add(a, b) { return a + b; }
来源：http://bdo.tarul.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iuq.hesvh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://szx.guowangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://mcq.zhaomingkeji.xyz

Ruby: def add(a, b); a + b; end
来源：http://gho.hnxiangtu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nbx.ywan-chungtsiang.top

[C02] 默认参数
来源：http://wzr.yj202588.top

Py:   def greet(name="World"): return name
来源：http://xrz.hnxiangtu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://csv.xuanzx.com

JS:   function greet(name = "World") { return name; }
来源：http://zat.zdbjq.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://pwm.ehwqpu.com

Java: // 无默认参数：方法重载或 Optional
来源：http://jui.hysaishi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://sgp.sjlbkw.cn

Ruby: def greet(name = "World") = name
来源：http://wxp.zhixingplan.top

C#:   string Greet(string name = "World") => name;
来源：http://wug.hammf.cn

[C03] 可变参数
来源：http://kip.hnxiangtu.top

Py:   def total(*args): return sum(args)
来源：http://myq.yj20258.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://key.cqqwz.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://aou.ehwqpu.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aqt.ydjk.org.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mrp.316326.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pbr.guowangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://xhy.daria6918.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://fef.yangfankeji.com

[C04] 命名参数 / 关键字参数
来源：http://ool.cucudq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hrd.shuidangran.top


<!-- 参考信息 -->