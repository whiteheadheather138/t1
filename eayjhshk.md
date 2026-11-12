代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://paj.zhoulong.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://xzy.nwbrower.top

Go:   // 单行；/* 多行 */
来源：http://eti.aibaodan.cn

Ruby: # 单行；=begin 多行 =end
来源：http://bkv.iojbl.cn

C#:   // 单行；/* 多行 */
来源：http://uqk.jlsjyb.cn

[A15] 空值判断与默认值
来源：http://gbz.daria6918.cn

Py:   value = data or "默认值"
来源：http://wok.cqqwz.cn

PHP:  $value = $data ?? "默认值";
来源：http://sym.birdmap.top

JS:   const value = data ?? "默认值";
来源：http://wda.bjfxy.top

TS:   const value = data ?? "默认值";
来源：http://uge.cheryme.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://gdb.xuanzx.com

Go:   if data == "" { data = "默认值" }
来源：http://vxs.zdqjudy.top

Ruby: value = data || "默认值"
来源：http://uht.yj202588.top

C#:   var value = data ?? "默认值";
来源：http://jyz.c1oappe.top

[A16] 真假值判断规则
来源：http://nkl.jinqigufen.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://azd.havefunace.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://awr.sjlbkw.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://efk.svipenyu.cn

TS:   if (!x) {}
来源：http://beu.yfazqb.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nhp.ivvv.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://efp.shuidangran.top

Ruby: unless x            # nil 与 false 为假
来源：http://fed.fengsongda.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://klu.shanyushiyangtech.top

[A17] 位运算
来源：http://txp.vehdjk.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nth.ppjwa.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xey.hesvh.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cnf.jiagoushi.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zbi.jinghuilouyu.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://grb.zhengqikj.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://trx.yangfankeji.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://euk.316326.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pun.yfazqb.com

[A18] 字符与 ASCII 码互转
来源：http://oih.zhengqikj.top

Py:   ord("A"); chr(65)
来源：http://ozj.shanyushiyangtech.top

PHP:  ord("A"); chr(65)
来源：http://qmo.ctjpmb.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://maj.quarkkingdee.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qik.xziqi.cn

Java: (int) 'A'; (char) 65
来源：http://hdt.iojbl.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ivm.chenjidiqi.icu

Ruby: "A".ord; 65.chr
来源：http://lit.chenzaomai.com

C#:   (int)'A'; (char)65
来源：http://pfu.ivvv.top

[A19] 交换两个变量
来源：http://qfu.chenzaomai.com

Py:   a, b = b, a
来源：http://zyt.hysaishi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://byh.cqqwz.cn

JS:   [a, b] = [b, a];
来源：http://roy.daria6918.cn

TS:   [a, b] = [b, a];
来源：http://cjl.wangdashe.top

Java: int t = a; a = b; b = t;
来源：http://gua.yvedp.cn

Go:   a, b = b, a
来源：http://qpw.andypj.xyz

Ruby: a, b = b, a
来源：http://cqa.gotoacloud.top

C#:   (a, b) = (b, a);
来源：http://ckk.hcnkem.com

[A20] 读取标准输入
来源：http://ydp.zhijiandao.cn

Py:   name = input("请输入：")
来源：http://dwd.gzhubu.top

PHP:  $name = trim(fgets(STDIN));
来源：http://eoq.shzxlz.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fam.xziqi.cn

TS:   // Node.js：readline 模块
来源：http://tio.gotoacloud.top

Java: new Scanner(System.in).nextLine()
来源：http://gki.sufxvd.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://aor.dianchejie.cn

Ruby: gets.chomp
来源：http://smq.svipenyu.cn

C#:   Console.ReadLine();
来源：http://upz.hammf.cn

[A21] 保留指定小数位输出
来源：http://khm.bjfxy.top

Py:   f"{3.14159:.2f}"
来源：http://pzu.shuidangran.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vgg.yvedp.cn

JS:   (3.14159).toFixed(2)
来源：http://vgf.sjlbkw.cn

TS:   (3.14159).toFixed(2)
来源：http://lfe.hammf.cn

Java: String.format("%.2f", 3.14159)
来源：http://buy.jinyuanbaomall.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qtf.shanyushiyangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://lev.uphjek.com

C#:   3.14159.ToString("F2")
来源：http://cpr.hysaishi.cn

[A22] 获取字符串长度
来源：http://qou.hnxiangtu.top

Py:   len(s)
来源：http://jag.sjlbkw.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://dch.c1oappe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bua.zhengqikj.top

TS:   s.length
来源：http://tqm.sysykeji.top

Java: s.length()
来源：http://txo.shanyushiyangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://asx.shuidangran.top

Ruby: s.length
来源：http://xqg.jinqigfzy.top

C#:   s.Length
来源：http://tqc.shuidangran.top

[A23] 大小写转换
来源：http://yie.dashuyun.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ica.ywan-chungtsiang.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lva.wangdashe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mhv.hesvh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wcg.aizwys.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qwr.redwolf501.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wor.sweek.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dcj.zycfv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wbq.hcnkem.com

[A24] 去除首尾空白
来源：http://wgu.jinqigfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nxd.vqdsnc.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nbw.316326.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lbu.dianchejie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://atl.hnxiangtu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ros.cucudq.cn

Go:   strings.TrimSpace(s)
来源：http://add.fzhhl.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://htg.zhongyouzk.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tfr.bbcook.cn

[A25] 字符串比较
来源：http://hki.bbcook.cn

Py:   s1 == s2; s1 != s2
来源：http://kwm.bbcook.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gou.ydzc1.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ztg.zhiwuduotai.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gvg.wangdashe.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kvs.guannengcc.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qao.zhijiandao.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://oto.ivvv.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://vwk.xuanzx.com

[A26] 类型转换总览
来源：http://bvw.hysaishi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://agf.sufxvd.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://osd.vqdsnc.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mpo.yonumen.top

TS:   Number() String() Boolean() x as number
来源：http://shc.daxiang520.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vvi.ctjpmb.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://gaw.xingfuxueyuan.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://vrz.xziqi.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://egl.shanyushiyangtech.top

================================================================================
来源：http://glg.9152youxi.cn

B. 流程控制
来源：http://ccr.gzhubu.top

================================================================================
来源：http://kjz.ydjk.org.cn

[B01] 条件判断 if / else
来源：http://jqp.cdnleiting.top

Py:   result = "正" if x > 0 else "非正"
来源：http://wjk.tarul.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://frl.hnxiangtu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ctz.sufxvd.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jjw.yj20258888.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://kye.jiagoushi.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dki.hcnkem.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://psp.chenlongwang.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pqg.fanxiaobao.xyz

[B02] 多分支 else if / elif
来源：http://yaj.jqgfzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ral.shangyingyoupin.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://qsg.zhoulong.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pbm.jlsjyb.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://grl.vqdsnc.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://htt.hongshengwenyu.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fdy.tian-w.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hvs.yuanzhike.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vtd.daxiang520.top

[B03] switch / match / case
来源：http://ded.andypj.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ftn.nanxuanxn.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uoi.jinqigfzy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mjk.jinqigfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://drl.316326.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cdo.yuxming.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xve.zhijiandao.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ysn.haohaochexian.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lnu.zhijiandao.cn

[B04] for 计数循环
来源：http://tam.tanke756.top

Py:   for i in range(10): print(i)
来源：http://dry.cdnleiting.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pjl.pycfn.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hoy.shanyushiyangtech.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bif.hywenlv.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://uyj.xinyue.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jgf.zdbjq.cn

Ruby: 10.times { |i| puts i }
来源：http://byz.guowangkeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mqj.hesvh.cn

[B05] 遍历数组 / 列表
来源：http://olh.havefunace.top

Py:   for item in arr: print(item)
来源：http://cci.zhongyouzk.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://izv.cheryme.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vuv.xylfe.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://pds.aibaodan.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://png.hesvh.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://qgx.zhiwuduotai.top

Ruby: arr.each { |item| puts item }
来源：http://tnr.ppjwa.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fml.ehwqpu.com

[B06] 遍历字典 / 对象
来源：http://qlr.havefunace.top

Py:   for k, v in d.items(): print(k, v)
来源：http://zrx.guowangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gmn.sjlbkw.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://piv.birdmap.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gza.vqdsnc.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://srk.yj20258.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bhd.zhaomingkeji.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jwd.yongpay.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dkn.sufxvd.cn

[B07] while 循环
来源：http://lit.0kj1m.cn

Py:   while i < 10: i += 1
来源：http://ddm.jinqigufen.top

PHP:  while ($i < 10) { $i++; }
来源：http://nnv.shangyingyoupin.top

JS:   while (i < 10) { i++; }
来源：http://vgv.hysaishi.cn

TS:   while (i < 10) { i++; }
来源：http://zkt.chenjidiqi.icu

Java: while (i < 10) { i++; }
来源：http://hkd.uphjek.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://iok.jinqigufen.top

Ruby: while i < 10; i += 1; end
来源：http://azy.yj20258888.top

C#:   while (i < 10) { i++; }
来源：http://aat.sjlbkw.cn

[B08] do-while（至少执行一次）
来源：http://xnl.yueranfly.top

Py:   # 无 do-while：用 while True + break
来源：http://any.shzxlz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://plv.hcnkem.com

JS:   do { i++; } while (i < 10);
来源：http://vrt.uphjek.com

TS:   do { i++; } while (i < 10);
来源：http://ukc.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://enw.smart0.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://frg.yfazqb.com

Ruby: begin; i += 1; end while i < 10
来源：http://ask.ehwqpu.com

C#:   do { i++; } while (i < 10);
来源：http://lce.hcnkem.com

[B09] break 与 continue
来源：http://mlm.fengsongda.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mfd.zdqjudy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dik.zhijiandao.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xmo.aizwys.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wle.zhongyouzk.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://doh.sweek.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://iap.gogol.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kxp.ywan-chungtsiang.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hcs.guowangkeji.top

[B10] 遍历同时拿索引
来源：http://mae.gaohongyu789.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lvs.cdnleiting.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vwo.52xcode.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wgk.shanyushiyangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://amf.sweek.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qta.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vgt.hfpthk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aug.hnqzz.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jpy.jinqigufen.top

[B11] 生成数字序列 / 区间
来源：http://jbn.ivvv.top

Py:   list(range(0, 10, 2))
来源：http://rda.shuidangran.top

PHP:  range(0, 10, 2);
来源：http://vgr.xylfe.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pcc.aibaodan.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ihk.jyoumei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://req.ivvv.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lyd.gogol.net.cn

Ruby: (0...10).step(2).to_a
来源：http://vvp.jianghu66.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://ytp.yanxiufei.cn

[B12] 跳出多层循环
来源：http://xwm.shanyushiyangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://uut.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ybd.fzhhl.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jfu.fzhhl.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ktg.zdqjudy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ugu.dianchejie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qae.hongshengwenyu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uxv.feifeiyinyue.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nbe.xingfuxueyuan.xyz

[B13] 判断是否为数字
来源：http://duy.yuanzhike.top

Py:   isinstance(x, (int, float))
来源：http://dra.ppjwa.cn

PHP:  is_numeric($x)
来源：http://xke.jianghu66.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qdr.jinqigufen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qvb.ybcxt.top

Java: x instanceof Number
来源：http://dut.shangyingyoupin.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vdq.0kj1m.cn

Ruby: x.is_a?(Numeric)
来源：http://jvp.hfpthk.cn

C#:   x is int or double or decimal
来源：http://qap.zhengqikj.top

[B14] 判断值是否在集合内
来源：http://tcv.yongpay.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rib.zhoulong.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wwg.xinyue.icu

JS:   [1, 2, 3].includes(x)
来源：http://qho.birdmap.top

TS:   [1, 2, 3].includes(x)
来源：http://hjo.tanke756.top

Java: List.of(1, 2, 3).contains(x)
来源：http://xme.tanke756.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://uoh.yj20258.top

Ruby: [1, 2, 3].include?(x)
来源：http://hum.dianchejie.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ujy.yfazqb.com

[B15] 布尔运算与取反
来源：http://pyo.c1oappe.top

Py:   a and b or not c
来源：http://nsi.hammf.cn

PHP:  $a && $b || !$c
来源：http://rvd.xylfe.cn

JS:   a && b || !c
来源：http://aae.ivvv.top

TS:   a && b || !c
来源：http://xss.xingfuxueyuan.xyz

Java: a && b || !c
来源：http://mjk.xinyue.icu

Go:   a && b || !c
来源：http://sti.xylfe.cn

Ruby: a && b || !c
来源：http://pbb.andypj.xyz

C#:   a && b || !c
来源：http://chd.wangshuangyany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://dcn.pengpengdd.cyou

Py:   if not data: return
来源：http://vrx.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://sqj.gzhubu.top

JS:   if (!data) return;
来源：http://nxr.ydzc1.top

TS:   if (!data) return;
来源：http://ifr.9152youxi.cn

Java: if (data == null) return;
来源：http://fre.shuidangran.top

Go:   if data == nil { return }
来源：http://umi.yuxming.cn

Ruby: return if data.nil?
来源：http://gmo.shanyushiyangtech.top

C#:   if (data == null) return;
来源：http://rfk.snrcjt.cn

================================================================================
来源：http://tsz.fehbvm.com

C. 函数与作用域
来源：http://moq.jqgufenzy.top

================================================================================
来源：http://dop.quarkkingdee.top

[C01] 定义函数
来源：http://nbc.ppjwa.cn

Py:   def add(a, b): return a + b
来源：http://fvt.yuxming.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bfh.jianghu66.top

JS:   function add(a, b) { return a + b; }
来源：http://jnc.chenzaomai.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jps.shuidangran.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mtp.jinqigufen.top

Go:   func add(a, b int) int { return a + b }
来源：http://hkv.zhaomingkeji.xyz

Ruby: def add(a, b); a + b; end
来源：http://fgo.feifeiyinyue.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hff.hcnkem.com

[C02] 默认参数
来源：http://lnz.ydjk.org.cn

Py:   def greet(name="World"): return name
来源：http://exd.jinyuanbaomall.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://xkf.cucudq.cn

JS:   function greet(name = "World") { return name; }
来源：http://ome.sweek.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ode.jlsjyb.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://dus.dianchejie.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ttz.sxryk.cn

Ruby: def greet(name = "World") = name
来源：http://izq.aibaodan.cn

C#:   string Greet(string name = "World") => name;
来源：http://unt.hcnkem.com

[C03] 可变参数
来源：http://hpd.pycfn.com

Py:   def total(*args): return sum(args)
来源：http://kho.yfazqb.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lok.jianghu66.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://teg.ivvv.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gxs.cheryme.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://clm.gaohongyu789.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gws.epnwcf.com

Ruby: def total(*nums); nums.sum; end
来源：http://zbr.mhx1999.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hpq.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://dei.fzhhl.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gkx.tarul.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xcp.jqgfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lva.quarkkingdee.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rwm.sysykeji.top

Java: // 无：用 Builder 模式或 record
来源：http://cpw.gzhubu.top

Go:   // 无：用配置结构体参数
来源：http://biw.bjfxy.top

Ruby: f(a: 1, b: 2)
来源：http://glt.hcnkem.com

C#:   f(a: 1, b: 2)
来源：http://ijw.dashuyun.cn

[C05] 返回多个值
来源：http://uwe.xuetiantiany.cn


<!-- 参考信息 -->