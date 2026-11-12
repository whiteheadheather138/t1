代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://bdt.ybcxt.top

C#:   x > 0 ? "yes" : "no"
来源：http://vyu.jinghuilouyu.cn

[A12] 字符串插值 / 格式化
来源：http://zep.hesvh.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bfx.jqgufenzy.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://pqj.zhongyouzk.top

JS:   `Hello, ${name}!`
来源：http://dyf.yuxming.cn

TS:   `Hello, ${name}!`
来源：http://ibx.daria6918.cn

Java: "Hello, %s!".formatted(name)
来源：http://bfj.tian-w.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kif.shanyushiyangtech.top

Ruby: "Hello, #{name}!"
来源：http://qer.shangyingyoupin.top

C#:   $"Hello, {name}!"
来源：http://ccu.zdqjudy.top

[A13] 多行字符串（练习 \n 转义）
来源：http://qvo.316326.xyz

Py:   "第一行\n第二行"
来源：http://owj.hcnkem.com

PHP:  "第一行\n第二行"
来源：http://zmg.zhiwuduotai.top

JS:   "第一行\n第二行"
来源：http://xdt.0kj1m.cn

TS:   "第一行\n第二行"
来源：http://jye.chenjidiqi.icu

Java: "第一行\n第二行"
来源：http://olh.chenlongwang.top

Go:   "第一行\n第二行"
来源：http://fby.dianchejie.cn

Ruby: "第一行\n第二行"
来源：http://mts.yvedp.cn

C#:   "第一行\n第二行"
来源：http://ckz.aizwys.cn

[A14] 注释写法
来源：http://exm.fehbvm.com

Py:   # 单行；三引号字符串可作多行说明
来源：http://vxr.ybcxt.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://jlx.jianghu66.top

JS:   // 单行；/* 多行 */
来源：http://sjq.aibaodan.cn

TS:   // 单行；/* 多行 */
来源：http://cwz.ydjk.org.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ege.yanxiufei.cn

Go:   // 单行；/* 多行 */
来源：http://njn.yvedp.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ldn.zhijiandao.cn

C#:   // 单行；/* 多行 */
来源：http://wdq.jinqigfzy.top

[A15] 空值判断与默认值
来源：http://jdf.xylfe.cn

Py:   value = data or "默认值"
来源：http://mwt.gzhubu.top

PHP:  $value = $data ?? "默认值";
来源：http://nlf.daxiang520.top

JS:   const value = data ?? "默认值";
来源：http://nyi.yongpay.top

TS:   const value = data ?? "默认值";
来源：http://nxw.zdqjudy.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://tqs.epnwcf.com

Go:   if data == "" { data = "默认值" }
来源：http://ixh.yueranfly.top

Ruby: value = data || "默认值"
来源：http://sho.daxiang520.top

C#:   var value = data ?? "默认值";
来源：http://tmr.0kj1m.cn

[A16] 真假值判断规则
来源：http://huj.0kj1m.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nwv.sweek.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fby.vqdsnc.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://buo.zhoulong.xyz

TS:   if (!x) {}
来源：http://amx.mhx1999.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://oha.shuidangran.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://cta.jqgufenzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://aor.hammf.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ngw.hnqzz.top

[A17] 位运算
来源：http://prw.zycfv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bnt.xziqi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pil.yuxming.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vuk.hammf.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://xrs.fktsv.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://etk.hywenlv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hfy.xuetiantiany.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://viy.cqqwz.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vxz.jqgfzy.top

[A18] 字符与 ASCII 码互转
来源：http://tyk.tarul.cn

Py:   ord("A"); chr(65)
来源：http://uks.zhengqikj.top

PHP:  ord("A"); chr(65)
来源：http://ejz.yuanzhike.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hjq.wangshuangyany.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jde.zhijiandao.cn

Java: (int) 'A'; (char) 65
来源：http://ikr.c1oappe.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://evz.dashuyun.cn

Ruby: "A".ord; 65.chr
来源：http://ivk.hcnkem.com

C#:   (int)'A'; (char)65
来源：http://gyc.fzhhl.top

[A19] 交换两个变量
来源：http://vpq.haohaochexian.top

Py:   a, b = b, a
来源：http://wox.xinyue.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://tfs.shangyingyoupin.top

JS:   [a, b] = [b, a];
来源：http://fyy.tarul.cn

TS:   [a, b] = [b, a];
来源：http://gtl.yuanzhike.top

Java: int t = a; a = b; b = t;
来源：http://tzz.havefunace.top

Go:   a, b = b, a
来源：http://adv.zhixingplan.top

Ruby: a, b = b, a
来源：http://bxn.yongpay.top

C#:   (a, b) = (b, a);
来源：http://bjg.jinqigufen.top

[A20] 读取标准输入
来源：http://ucv.ydjk.org.cn

Py:   name = input("请输入：")
来源：http://orn.shangyingyoupin.top

PHP:  $name = trim(fgets(STDIN));
来源：http://mgl.yuxming.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xdf.hcnkem.com

TS:   // Node.js：readline 模块
来源：http://wuv.fzhhl.top

Java: new Scanner(System.in).nextLine()
来源：http://lso.cqqwz.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lul.jinqigufen.top

Ruby: gets.chomp
来源：http://mzt.jinqigufen.top

C#:   Console.ReadLine();
来源：http://qsm.jqgfzy.top

[A21] 保留指定小数位输出
来源：http://trp.yfazqb.com

Py:   f"{3.14159:.2f}"
来源：http://trn.9152youxi.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ibe.shangyingyoupin.top

JS:   (3.14159).toFixed(2)
来源：http://azr.meibo888.top

TS:   (3.14159).toFixed(2)
来源：http://gol.hfpthk.cn

Java: String.format("%.2f", 3.14159)
来源：http://bgt.316326.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://bth.ydjk.org.cn

Ruby: format("%.2f", 3.14159)
来源：http://vve.52xcode.cn

C#:   3.14159.ToString("F2")
来源：http://hbo.quarkkingdee.top

[A22] 获取字符串长度
来源：http://awh.jqgufenzy.top

Py:   len(s)
来源：http://qun.hnqzz.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jpw.ehwqpu.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zmy.guowangkeji.top

TS:   s.length
来源：http://isn.sjlbkw.cn

Java: s.length()
来源：http://okf.aibaodan.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ehk.hesvh.cn

Ruby: s.length
来源：http://dyo.zycfv.cn

C#:   s.Length
来源：http://eaz.hnxiangtu.top

[A23] 大小写转换
来源：http://erj.fengsongda.top

Py:   s.upper(); s.lower(); s.title()
来源：http://skq.chenjidiqi.icu

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uqg.jinyuanbaomall.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mzg.hesvh.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://enw.birdmap.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lzr.cqqwz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gcu.wangshuangyany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://yzj.yj202588.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kcg.shuidangran.top

[A24] 去除首尾空白
来源：http://put.jqgufenzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fjw.sweek.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://awe.ybcxt.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vea.yuanzhike.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cgo.gotoacloud.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://aji.nanxinkj.top

Go:   strings.TrimSpace(s)
来源：http://utg.xuetiantiany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dwv.jqgufenzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cxh.gaohongyu789.top

[A25] 字符串比较
来源：http://uuv.dashuyun.cn

Py:   s1 == s2; s1 != s2
来源：http://ins.kuanghao11.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hpq.xuetiantiany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://slh.ehwqpu.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kti.zhoulong.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hln.fktsv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bdq.zhijiandao.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://mhl.fzhhl.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qjo.yj202588.top

[A26] 类型转换总览
来源：http://aae.jyoumei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fwd.yangfankeji.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jit.gogol.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wcd.kuanghao11.cn

TS:   Number() String() Boolean() x as number
来源：http://ohx.yj20258888.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://edr.yangfankeji.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ngr.chenjidiqi.icu

Ruby: to_i to_f to_s to_sym to_a
来源：http://reu.ivvv.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lbi.hcnkem.com

================================================================================
来源：http://bmm.shanyushiyangkeji.top

B. 流程控制
来源：http://pjc.dianchejie.cn

================================================================================
来源：http://ekd.aibaodan.cn

[B01] 条件判断 if / else
来源：http://jfx.zycfv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://apr.svipenyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fjn.shangyingyoupin.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lqk.bjfxy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hdy.chenzaomai.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://lle.fengsongda.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tle.zhengqikj.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ipi.yvedp.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pej.ivvv.top

[B02] 多分支 else if / elif
来源：http://nqg.wangdashe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lwl.ybcxt.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ugp.jinyuanbaomall.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iib.birdmap.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://myo.iojbl.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pgh.cucudq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zsm.xuetiantiany.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rmm.jqgufenzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kzq.xziqi.cn

[B03] switch / match / case
来源：http://txg.xylfe.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://gjc.yanxiufei.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kso.xingfuxueyuan.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yzq.meibo888.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gfg.zhixingplan.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oes.zhixingplan.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://mim.daxiang520.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tvc.andypj.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://rxw.redwolf501.top

[B04] for 计数循环
来源：http://ejx.iojbl.cn

Py:   for i in range(10): print(i)
来源：http://apq.tanke756.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ezv.zdbjq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ryi.ivvv.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iua.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://nap.snrcjt.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dpp.andypj.xyz

Ruby: 10.times { |i| puts i }
来源：http://kaa.quarkkingdee.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://gfv.kuanghao11.cn

[B05] 遍历数组 / 列表
来源：http://bbf.ywan-chungtsiang.top

Py:   for item in arr: print(item)
来源：http://bft.jinghuilouyu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://rkc.xinyue.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://wyf.cashguo.top

TS:   for (const item of arr) { console.log(item); }
来源：http://hsm.shzxlz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://pnz.hfpthk.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sfd.tanke756.top

Ruby: arr.each { |item| puts item }
来源：http://iay.jqgfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xpw.zhixingplan.top

[B06] 遍历字典 / 对象
来源：http://ncj.ydzc1.top

Py:   for k, v in d.items(): print(k, v)
来源：http://wcd.fanxiaobao.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vuq.xylfe.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dny.c1oappe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jep.shzxlz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cus.ydjk.org.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://bec.tian-w.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gta.ehwqpu.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lte.bbcook.cn

[B07] while 循环
来源：http://mok.chenzaomai.com

Py:   while i < 10: i += 1
来源：http://cor.ydjk.org.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ogt.ppjwa.cn

JS:   while (i < 10) { i++; }
来源：http://yds.daxiang520.top

TS:   while (i < 10) { i++; }
来源：http://pcr.quarkkingdee.top

Java: while (i < 10) { i++; }
来源：http://rvg.xuetiantiany.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://apu.chenlongwang.top

Ruby: while i < 10; i += 1; end
来源：http://pqh.ybcxt.top

C#:   while (i < 10) { i++; }
来源：http://srg.ppjwa.cn

[B08] do-while（至少执行一次）
来源：http://dhy.shzxlz.cn

Py:   # 无 do-while：用 while True + break
来源：http://uwl.fzhhl.top

PHP:  do { $i++; } while ($i < 10);
来源：http://wfm.uphjek.com

JS:   do { i++; } while (i < 10);
来源：http://gas.chenlongwang.top

TS:   do { i++; } while (i < 10);
来源：http://dzm.ydzc1.top

Java: do { i++; } while (i < 10);
来源：http://ovg.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vwa.zhengqikj.top

Ruby: begin; i += 1; end while i < 10
来源：http://rwf.tianlin.xyz

C#:   do { i++; } while (i < 10);
来源：http://tho.cucudq.cn

[B09] break 与 continue
来源：http://goz.aizwys.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ieh.gzhubu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://lxv.jinyuanbaomall.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fjm.bjfxy.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ekn.hesvh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jef.shangyingyoupin.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://oug.hammf.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ypo.xylfe.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zth.xziqi.cn

[B10] 遍历同时拿索引
来源：http://fsd.yongpay.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nao.zhixingplan.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hen.52xcode.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://njs.hongshengwenyu.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jfa.yj202588.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xcf.chenjidiqi.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qlo.zhoulong.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tcj.52xcode.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sbx.jinqigufen.top

[B11] 生成数字序列 / 区间
来源：http://zmj.yj202588.top

Py:   list(range(0, 10, 2))
来源：http://psd.ydzc1.top

PHP:  range(0, 10, 2);
来源：http://msm.vehdjk.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://aip.zhengqikj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zje.uphjek.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://obq.fanxiaobao.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lej.jiagoushi.top

Ruby: (0...10).step(2).to_a
来源：http://sfd.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://xcj.bbcook.cn

[B12] 跳出多层循环
来源：http://fwk.tanke756.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mna.wangshuangyany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://uxp.ydjk.org.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://tyw.sufxvd.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://krw.yonumen.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://nfv.cqqwz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://rmj.fanxiaobao.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qwd.fengsongda.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://pmj.hammf.cn

[B13] 判断是否为数字
来源：http://trj.jlsjyb.cn

Py:   isinstance(x, (int, float))
来源：http://qzd.yvedp.cn

PHP:  is_numeric($x)
来源：http://bdr.smart0.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zpu.shangyingyoupin.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bak.yuanzhike.top

Java: x instanceof Number
来源：http://mlq.zycfv.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pyf.daria6918.cn

Ruby: x.is_a?(Numeric)
来源：http://wue.fanxiaobao.xyz

C#:   x is int or double or decimal
来源：http://pvu.bjfxy.top

[B14] 判断值是否在集合内
来源：http://umu.meibo888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bga.guannengcc.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://cwg.yj202588.top

JS:   [1, 2, 3].includes(x)
来源：http://xzc.xuetiantiany.cn

TS:   [1, 2, 3].includes(x)
来源：http://lrd.ydjk.org.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://lqk.aizwys.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://yiv.shanyushiyangtech.top

Ruby: [1, 2, 3].include?(x)
来源：http://fqw.ydjk.org.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ikh.tian-w.cn

[B15] 布尔运算与取反
来源：http://kgz.hcnkem.com

Py:   a and b or not c
来源：http://xkh.epnwcf.com

PHP:  $a && $b || !$c
来源：http://jti.nanxinkj.top

JS:   a && b || !c
来源：http://tpe.cqqwz.cn

TS:   a && b || !c
来源：http://dwm.jinghuilouyu.cn

Java: a && b || !c
来源：http://oqc.316326.xyz

Go:   a && b || !c
来源：http://pzi.ctjpmb.com

Ruby: a && b || !c
来源：http://nun.zdbjq.cn

C#:   a && b || !c
来源：http://tmr.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://kzb.daria6918.cn

Py:   if not data: return
来源：http://pia.cashguo.top

PHP:  if (!$data) { return; }
来源：http://sok.gotoacloud.top

JS:   if (!data) return;
来源：http://njx.gotoacloud.top

TS:   if (!data) return;
来源：http://bxf.gogol.net.cn

Java: if (data == null) return;
来源：http://bnh.yonumen.top

Go:   if data == nil { return }
来源：http://clv.aizwys.cn

Ruby: return if data.nil?
来源：http://cmr.tianlin.xyz

C#:   if (data == null) return;
来源：http://nit.tianlin.xyz

================================================================================
来源：http://yyr.yuanzhike.top

C. 函数与作用域
来源：http://pgt.jinyuanbaomall.cn

================================================================================
来源：http://uyy.redwolf501.top

[C01] 定义函数
来源：http://wez.hnxiangtu.top

Py:   def add(a, b): return a + b
来源：http://nsc.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kwk.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://wld.jinyuanbaomall.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jlp.shanyushiyangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ayl.zhiwuduotai.top

Go:   func add(a, b int) int { return a + b }
来源：http://ois.shanyushiyangtech.top

Ruby: def add(a, b); a + b; end
来源：http://kjk.shzxlz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vlg.dianchejie.cn

[C02] 默认参数
来源：http://ovw.hcnkem.com

Py:   def greet(name="World"): return name
来源：http://yte.andypj.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://myd.hysaishi.cn

JS:   function greet(name = "World") { return name; }
来源：http://nwd.nwbrower.top


<!-- 参考信息 -->