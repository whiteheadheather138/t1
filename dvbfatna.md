代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://bhk.zhijiandao.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wuk.yfazqb.com

Go:   // 单行；/* 多行 */
来源：http://eba.dashuyun.cn

Ruby: # 单行；=begin 多行 =end
来源：http://dnn.zdbjq.cn

C#:   // 单行；/* 多行 */
来源：http://yic.shzxlz.cn

[A15] 空值判断与默认值
来源：http://kmt.zdbjq.cn

Py:   value = data or "默认值"
来源：http://xkv.hnqzz.top

PHP:  $value = $data ?? "默认值";
来源：http://wfz.chenjidiqi.icu

JS:   const value = data ?? "默认值";
来源：http://fux.gaohongyu789.top

TS:   const value = data ?? "默认值";
来源：http://rcd.shuidangran.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ftf.yj202588.top

Go:   if data == "" { data = "默认值" }
来源：http://ncf.dianchejie.cn

Ruby: value = data || "默认值"
来源：http://xrr.xingfuxueyuan.xyz

C#:   var value = data ?? "默认值";
来源：http://fen.jqgufenzy.top

[A16] 真假值判断规则
来源：http://sji.zhoulong.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://llr.cqqwz.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mbl.quarkkingdee.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rbt.wangdashe.top

TS:   if (!x) {}
来源：http://oaf.snrcjt.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pje.52xcode.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xpl.ivvv.top

Ruby: unless x            # nil 与 false 为假
来源：http://tnr.shanyushiyangtech.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wpv.zycfv.cn

[A17] 位运算
来源：http://not.yj20258.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qub.pycfn.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://agy.ehwqpu.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xbp.9152youxi.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cjx.havefunace.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gyh.tianlin.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://agv.hongshengwenyu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ttr.hcnkem.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jtl.yuxming.cn

[A18] 字符与 ASCII 码互转
来源：http://wsy.jqgufenzy.top

Py:   ord("A"); chr(65)
来源：http://ebj.zhixingplan.top

PHP:  ord("A"); chr(65)
来源：http://zlw.ctjpmb.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pqd.chenlongwang.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://own.xziqi.cn

Java: (int) 'A'; (char) 65
来源：http://ujk.pycfn.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xfp.yj20258.top

Ruby: "A".ord; 65.chr
来源：http://fyi.52xcode.cn

C#:   (int)'A'; (char)65
来源：http://qbk.hfpthk.cn

[A19] 交换两个变量
来源：http://lxe.yuxming.cn

Py:   a, b = b, a
来源：http://abi.sysykeji.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hem.hammf.cn

JS:   [a, b] = [b, a];
来源：http://zpp.pengpengdd.cyou

TS:   [a, b] = [b, a];
来源：http://imh.xziqi.cn

Java: int t = a; a = b; b = t;
来源：http://jkd.xuetiantiany.cn

Go:   a, b = b, a
来源：http://ywz.ywan-chungtsiang.top

Ruby: a, b = b, a
来源：http://jyw.jyoumei.cn

C#:   (a, b) = (b, a);
来源：http://gux.yj20258.top

[A20] 读取标准输入
来源：http://psa.xingfuxueyuan.xyz

Py:   name = input("请输入：")
来源：http://cir.hammf.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ygp.fktsv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://npk.zhiwuduotai.top

TS:   // Node.js：readline 模块
来源：http://mns.ywan-chungtsiang.top

Java: new Scanner(System.in).nextLine()
来源：http://php.sjlbkw.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nuk.andypj.xyz

Ruby: gets.chomp
来源：http://qae.tanke756.top

C#:   Console.ReadLine();
来源：http://vda.ybcxt.top

[A21] 保留指定小数位输出
来源：http://pnp.yongpay.top

Py:   f"{3.14159:.2f}"
来源：http://uwe.c1oappe.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://swc.meibo888.top

JS:   (3.14159).toFixed(2)
来源：http://lhh.jqgufenzy.top

TS:   (3.14159).toFixed(2)
来源：http://emn.snrcjt.cn

Java: String.format("%.2f", 3.14159)
来源：http://ulh.nanxuanxn.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rfq.yuanzhike.top

Ruby: format("%.2f", 3.14159)
来源：http://fom.nanxinkj.top

C#:   3.14159.ToString("F2")
来源：http://qhf.vqdsnc.cn

[A22] 获取字符串长度
来源：http://kzb.hywenlv.cn

Py:   len(s)
来源：http://khv.zhixingplan.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://oda.gaohongyu789.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ffa.jqgufenzy.top

TS:   s.length
来源：http://esz.zdqjudy.top

Java: s.length()
来源：http://vcn.uphjek.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bsz.yuanzhike.top

Ruby: s.length
来源：http://mzl.ydzc1.top

C#:   s.Length
来源：http://oxl.zhiwuduotai.top

[A23] 大小写转换
来源：http://hal.yvedp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ioe.xinyue.icu

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ycb.tarul.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://orv.yueranfly.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ugm.yangfankeji.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qgk.uphjek.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://oga.gzhubu.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://oue.gaohongyu789.top

C#:   s.ToUpper(); s.ToLower()
来源：http://yup.jiagoushi.top

[A24] 去除首尾空白
来源：http://ery.cdnleiting.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qes.yangfankeji.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://byx.fzhhl.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://upf.ybcxt.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://tbs.zycfv.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rwv.fktsv.cn

Go:   strings.TrimSpace(s)
来源：http://gcp.tanke756.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gyn.feifeiyinyue.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://pdh.xziqi.cn

[A25] 字符串比较
来源：http://amr.tianlin.xyz

Py:   s1 == s2; s1 != s2
来源：http://kvt.guowangkeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iea.9152youxi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gav.smart0.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gbs.zycfv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hqc.pycfn.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ftr.bbcook.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://exm.wangdashe.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cum.52xcode.cn

[A26] 类型转换总览
来源：http://iob.cashguo.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://int.shangyingyoupin.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zlc.hnxiangtu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gvb.zhongyouzk.top

TS:   Number() String() Boolean() x as number
来源：http://cdz.jlsjyb.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://eqm.yangfankeji.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bgz.mhx1999.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ith.yonumen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lkf.bbcook.cn

================================================================================
来源：http://pky.nwbrower.top

B. 流程控制
来源：http://oxr.jlsjyb.cn

================================================================================
来源：http://nko.ybcxt.top

[B01] 条件判断 if / else
来源：http://dwc.dianchejie.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://moa.aizwys.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rtd.fehbvm.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ybx.smart0.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://dqj.yuanzhike.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://apa.cdnleiting.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zfj.meibo888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://icy.andypj.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dev.tian-w.cn

[B02] 多分支 else if / elif
来源：http://evr.9152youxi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jrk.nanxinkj.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://duy.tarul.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ici.cashguo.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bqa.zhiwuduotai.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ain.ctjpmb.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gjk.svipenyu.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hcg.quarkkingdee.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mbj.shanyushiyangtech.top

[B03] switch / match / case
来源：http://lgn.wangdashe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fol.jianghu66.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hqh.yj202588.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oti.zhiwuduotai.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bfw.sxryk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zgi.fanxiaobao.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ulu.hnxiangtu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://bpv.xinyue.icu

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://suh.yvedp.cn

[B04] for 计数循环
来源：http://nbt.daxiang520.top

Py:   for i in range(10): print(i)
来源：http://ozl.snrcjt.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://egw.fehbvm.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://itu.zhoulong.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vyo.sjlbkw.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://iyr.pycfn.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://thx.mhx1999.top

Ruby: 10.times { |i| puts i }
来源：http://kzj.yanxiufei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jdm.chenjidiqi.icu

[B05] 遍历数组 / 列表
来源：http://qct.fengsongda.top

Py:   for item in arr: print(item)
来源：http://aen.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mgh.xingfuxueyuan.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://pmx.sweek.top

TS:   for (const item of arr) { console.log(item); }
来源：http://szo.52xcode.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jnk.cqqwz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ulb.tian-w.cn

Ruby: arr.each { |item| puts item }
来源：http://txn.gzhubu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gbs.birdmap.top

[B06] 遍历字典 / 对象
来源：http://dqa.kuanghao11.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jax.jqgfzy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mpk.meibo888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://uyw.bbcook.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ryd.yangfankeji.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wvn.hcnkem.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://beg.birdmap.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://uji.316326.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mro.tian-w.cn

[B07] while 循环
来源：http://fey.tarul.cn

Py:   while i < 10: i += 1
来源：http://rvc.nanxinkj.top

PHP:  while ($i < 10) { $i++; }
来源：http://mcm.yj202588.top

JS:   while (i < 10) { i++; }
来源：http://izp.jinqigfzy.top

TS:   while (i < 10) { i++; }
来源：http://xkq.sysykeji.top

Java: while (i < 10) { i++; }
来源：http://eno.ydjk.org.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bsz.bbcook.cn

Ruby: while i < 10; i += 1; end
来源：http://zzd.yueranfly.top

C#:   while (i < 10) { i++; }
来源：http://zdn.jqgufenzy.top

[B08] do-while（至少执行一次）
来源：http://qag.9152youxi.cn

Py:   # 无 do-while：用 while True + break
来源：http://hpq.c1oappe.top

PHP:  do { $i++; } while ($i < 10);
来源：http://nrf.zdqjudy.top

JS:   do { i++; } while (i < 10);
来源：http://ext.xuanzx.com

TS:   do { i++; } while (i < 10);
来源：http://qau.jinqigufen.top

Java: do { i++; } while (i < 10);
来源：http://ale.fengsongda.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hlh.zhixingplan.top

Ruby: begin; i += 1; end while i < 10
来源：http://vul.daxiang520.top

C#:   do { i++; } while (i < 10);
来源：http://qtx.sysykeji.top

[B09] break 与 continue
来源：http://mxm.hongshengwenyu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ust.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ypa.zhengqikj.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qbz.jqgfzy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iyv.bbcook.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://umv.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://saq.ydzc1.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vtf.ivvv.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lil.yuanzhike.top

[B10] 遍历同时拿索引
来源：http://vks.hysaishi.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qoz.zhengqikj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dwq.jiagoushi.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://asm.sxryk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dyh.zycfv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gcc.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yhj.pengpengdd.cyou

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cwg.ybcxt.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://exp.ctjpmb.com

[B11] 生成数字序列 / 区间
来源：http://vef.ywan-chungtsiang.top

Py:   list(range(0, 10, 2))
来源：http://wgh.xingfuxueyuan.xyz

PHP:  range(0, 10, 2);
来源：http://wck.haohaochexian.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nfj.jinyuanbaomall.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ygv.sjlbkw.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tap.zdbjq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://apl.ctjpmb.com

Ruby: (0...10).step(2).to_a
来源：http://lvn.yj20258888.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wrl.aibaodan.cn

[B12] 跳出多层循环
来源：http://spy.yvedp.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qce.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://fbb.jyoumei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tnm.9152youxi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hvw.xuetiantiany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uds.jinqigufen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mmm.chenlongwang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dvu.0kj1m.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rtq.iojbl.cn

[B13] 判断是否为数字
来源：http://vtz.cqqwz.cn

Py:   isinstance(x, (int, float))
来源：http://kgd.wangdashe.top

PHP:  is_numeric($x)
来源：http://tgf.yj20258888.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nof.hammf.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vgo.sweek.top

Java: x instanceof Number
来源：http://sie.xylfe.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fbl.guannengcc.top

Ruby: x.is_a?(Numeric)
来源：http://xie.jqgufenzy.top

C#:   x is int or double or decimal
来源：http://akf.pengpengdd.cyou

[B14] 判断值是否在集合内
来源：http://gjd.yangfankeji.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://khr.hesvh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://byx.fengsongda.top

JS:   [1, 2, 3].includes(x)
来源：http://txw.zycfv.cn

TS:   [1, 2, 3].includes(x)
来源：http://ruk.haohaochexian.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hbx.hcnkem.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ahw.jinqigufen.top

Ruby: [1, 2, 3].include?(x)
来源：http://sha.hammf.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nbe.zdqjudy.top

[B15] 布尔运算与取反
来源：http://hnr.nanxinkj.top

Py:   a and b or not c
来源：http://nrz.jinqigfzy.top

PHP:  $a && $b || !$c
来源：http://edf.guannengcc.top

JS:   a && b || !c
来源：http://mtg.xingfuxueyuan.xyz

TS:   a && b || !c
来源：http://yek.ctjpmb.com

Java: a && b || !c
来源：http://crf.zhongyouzk.top

Go:   a && b || !c
来源：http://wgk.aizwys.cn

Ruby: a && b || !c
来源：http://ozd.yongpay.top

C#:   a && b || !c
来源：http://oef.hongshengwenyu.top

[B16] 卫语句：不满足条件提前返回
来源：http://eqf.shanyushiyangkeji.top

Py:   if not data: return
来源：http://val.yueranfly.top

PHP:  if (!$data) { return; }
来源：http://zgo.ywan-chungtsiang.top

JS:   if (!data) return;
来源：http://sam.quarkkingdee.top

TS:   if (!data) return;
来源：http://pmo.yj20258.top

Java: if (data == null) return;
来源：http://xia.zhijiandao.cn

Go:   if data == nil { return }
来源：http://axe.nanxuanxn.top

Ruby: return if data.nil?
来源：http://uwx.jqgufenzy.top

C#:   if (data == null) return;
来源：http://xak.zhongyouzk.top

================================================================================
来源：http://wnz.snrcjt.cn

C. 函数与作用域
来源：http://ahm.yfazqb.com

================================================================================
来源：http://eao.dianchejie.cn

[C01] 定义函数
来源：http://jts.nanxinkj.top

Py:   def add(a, b): return a + b
来源：http://zky.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gkf.c1oappe.top

JS:   function add(a, b) { return a + b; }
来源：http://suc.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uzv.gotoacloud.top

Java: static int add(int a, int b) { return a + b; }
来源：http://luy.zhaomingkeji.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://tmo.cqqwz.cn

Ruby: def add(a, b); a + b; end
来源：http://cgx.chenjidiqi.icu

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ypf.shzxlz.cn

[C02] 默认参数
来源：http://tmh.quarkkingdee.top

Py:   def greet(name="World"): return name
来源：http://lzd.yuxming.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://eds.sufxvd.cn

JS:   function greet(name = "World") { return name; }
来源：http://agi.yj202588.top

TS:   function greet(name: string = "World") { return name; }
来源：http://adq.yuanzhike.top

Java: // 无默认参数：方法重载或 Optional
来源：http://alh.quarkkingdee.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://anq.jinqigfzy.top

Ruby: def greet(name = "World") = name
来源：http://kvu.zdqjudy.top

C#:   string Greet(string name = "World") => name;
来源：http://kww.xylfe.cn

[C03] 可变参数
来源：http://guv.yangfankeji.com

Py:   def total(*args): return sum(args)
来源：http://ytn.jqgfzy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://avr.sxryk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://icx.yonumen.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lgr.zhengqikj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qzs.shanyushiyangkeji.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://urc.tian-w.cn

Ruby: def total(*nums); nums.sum; end
来源：http://nlj.jqgufenzy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bkv.jianghu66.top

[C04] 命名参数 / 关键字参数
来源：http://qmi.smart0.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://flq.gogol.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xjh.yonumen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ali.shangyingyoupin.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xov.guannengcc.top

Java: // 无：用 Builder 模式或 record
来源：http://cwn.jiagoushi.top

Go:   // 无：用配置结构体参数
来源：http://fzu.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://pyb.52xcode.cn

C#:   f(a: 1, b: 2)
来源：http://pwb.hywenlv.cn

[C05] 返回多个值
来源：http://prz.xingfuxueyuan.xyz


<!-- 参考信息 -->