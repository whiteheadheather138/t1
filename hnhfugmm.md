代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://nka.zdbjq.cn

C#:   x > 0 ? "yes" : "no"
来源：http://ggd.ivvv.top

[A12] 字符串插值 / 格式化
来源：http://vmw.gogol.net.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://wvv.52xcode.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://ppo.daria6918.cn

JS:   `Hello, ${name}!`
来源：http://mci.zhengqikj.top

TS:   `Hello, ${name}!`
来源：http://bhw.tanke756.top

Java: "Hello, %s!".formatted(name)
来源：http://uxx.yongpay.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mgn.daria6918.cn

Ruby: "Hello, #{name}!"
来源：http://izk.iojbl.cn

C#:   $"Hello, {name}!"
来源：http://tla.chenlongwang.top

[A13] 多行字符串（练习 \n 转义）
来源：http://qcz.yuanzhike.top

Py:   "第一行\n第二行"
来源：http://bgx.hesvh.cn

PHP:  "第一行\n第二行"
来源：http://udo.guowangkeji.top

JS:   "第一行\n第二行"
来源：http://mvs.chenzaomai.com

TS:   "第一行\n第二行"
来源：http://zkr.vqdsnc.cn

Java: "第一行\n第二行"
来源：http://klv.jqgfzy.top

Go:   "第一行\n第二行"
来源：http://aqe.fzhhl.top

Ruby: "第一行\n第二行"
来源：http://few.jinqigufen.top

C#:   "第一行\n第二行"
来源：http://cuk.chenzaomai.com

[A14] 注释写法
来源：http://lja.zhiwuduotai.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://qtq.ywan-chungtsiang.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://rir.jinghuilouyu.cn

JS:   // 单行；/* 多行 */
来源：http://dcc.ywan-chungtsiang.top

TS:   // 单行；/* 多行 */
来源：http://znj.fengsongda.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://bqj.xylfe.cn

Go:   // 单行；/* 多行 */
来源：http://djo.gzhubu.top

Ruby: # 单行；=begin 多行 =end
来源：http://leq.xuanzx.com

C#:   // 单行；/* 多行 */
来源：http://zmh.zhaomingkeji.xyz

[A15] 空值判断与默认值
来源：http://mxn.fzhhl.top

Py:   value = data or "默认值"
来源：http://abg.chenzaomai.com

PHP:  $value = $data ?? "默认值";
来源：http://znh.c1oappe.top

JS:   const value = data ?? "默认值";
来源：http://xqz.zhoulong.xyz

TS:   const value = data ?? "默认值";
来源：http://wvy.jyoumei.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://dcu.ydzc1.top

Go:   if data == "" { data = "默认值" }
来源：http://qaa.jlsjyb.cn

Ruby: value = data || "默认值"
来源：http://aab.nwbrower.top

C#:   var value = data ?? "默认值";
来源：http://mjk.bbcook.cn

[A16] 真假值判断规则
来源：http://vve.kuanghao11.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vgt.sjlbkw.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rkh.gaohongyu789.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rip.c1oappe.top

TS:   if (!x) {}
来源：http://you.aibaodan.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cfk.fehbvm.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xcm.tarul.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ezx.xylfe.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://fxk.gotoacloud.top

[A17] 位运算
来源：http://xra.tianlin.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lpk.hesvh.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bnb.birdmap.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fps.chenzaomai.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://klf.hnxiangtu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mvs.yvedp.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cmw.yuxming.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mmm.jinyuanbaomall.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rxl.sufxvd.cn

[A18] 字符与 ASCII 码互转
来源：http://xnl.havefunace.top

Py:   ord("A"); chr(65)
来源：http://ttp.havefunace.top

PHP:  ord("A"); chr(65)
来源：http://dll.sweek.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wxp.jlsjyb.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qjc.xingfuxueyuan.xyz

Java: (int) 'A'; (char) 65
来源：http://pwm.jinqigfzy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://apx.yongpay.top

Ruby: "A".ord; 65.chr
来源：http://nvc.cqqwz.cn

C#:   (int)'A'; (char)65
来源：http://gro.zhixingplan.top

[A19] 交换两个变量
来源：http://knu.jiagoushi.top

Py:   a, b = b, a
来源：http://wye.kuanghao11.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://jdt.cdnleiting.top

JS:   [a, b] = [b, a];
来源：http://zoh.uphjek.com

TS:   [a, b] = [b, a];
来源：http://rcu.ywan-chungtsiang.top

Java: int t = a; a = b; b = t;
来源：http://imo.yuanzhike.top

Go:   a, b = b, a
来源：http://afo.nanxuanxn.top

Ruby: a, b = b, a
来源：http://wjm.sjlbkw.cn

C#:   (a, b) = (b, a);
来源：http://yva.cashguo.top

[A20] 读取标准输入
来源：http://nrl.epnwcf.com

Py:   name = input("请输入：")
来源：http://uss.shzxlz.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://xuk.ybcxt.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lxz.316326.xyz

TS:   // Node.js：readline 模块
来源：http://rut.bjfxy.top

Java: new Scanner(System.in).nextLine()
来源：http://fki.xziqi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://act.cashguo.top

Ruby: gets.chomp
来源：http://hsa.pycfn.com

C#:   Console.ReadLine();
来源：http://fxr.smart0.xyz

[A21] 保留指定小数位输出
来源：http://dpq.havefunace.top

Py:   f"{3.14159:.2f}"
来源：http://umu.sweek.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nyz.svipenyu.cn

JS:   (3.14159).toFixed(2)
来源：http://npg.zdbjq.cn

TS:   (3.14159).toFixed(2)
来源：http://vzx.shanyushiyangtech.top

Java: String.format("%.2f", 3.14159)
来源：http://gvn.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zvk.havefunace.top

Ruby: format("%.2f", 3.14159)
来源：http://els.smart0.xyz

C#:   3.14159.ToString("F2")
来源：http://rhp.vqdsnc.cn

[A22] 获取字符串长度
来源：http://rcz.wangshuangyany.cn

Py:   len(s)
来源：http://lfz.yangfankeji.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bjz.andypj.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nrf.iojbl.cn

TS:   s.length
来源：http://xvw.hammf.cn

Java: s.length()
来源：http://fqs.c1oappe.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yfk.ctjpmb.com

Ruby: s.length
来源：http://omm.haohaochexian.top

C#:   s.Length
来源：http://ask.cqqwz.cn

[A23] 大小写转换
来源：http://jzv.feifeiyinyue.top

Py:   s.upper(); s.lower(); s.title()
来源：http://mpl.jqgfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://htl.guowangkeji.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://iwl.gaohongyu789.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dfk.tanke756.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://pqu.meibo888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wvh.bjfxy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tcq.zhoulong.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://rfc.ehwqpu.com

[A24] 去除首尾空白
来源：http://qlv.jqgufenzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://evy.jianghu66.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zyl.hysaishi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ufg.zycfv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vll.hongshengwenyu.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://orh.zhixingplan.top

Go:   strings.TrimSpace(s)
来源：http://lay.zhoulong.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://azh.havefunace.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://twg.hammf.cn

[A25] 字符串比较
来源：http://jpz.ivvv.top

Py:   s1 == s2; s1 != s2
来源：http://mhb.andypj.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jpb.ppjwa.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uhi.zhongyouzk.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://jdp.jqgfzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wok.52xcode.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xgj.shanyushiyangtech.top

Ruby: s1 == s2; s1 <=> s2
来源：http://bkf.hongshengwenyu.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hwf.ydzc1.top

[A26] 类型转换总览
来源：http://mqc.hnqzz.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://djo.yuanzhike.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mle.ybcxt.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pjz.yuxming.cn

TS:   Number() String() Boolean() x as number
来源：http://rhh.snrcjt.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zic.uphjek.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cjo.gotoacloud.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://iup.yj20258.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iqe.epnwcf.com

================================================================================
来源：http://rdw.yvedp.cn

B. 流程控制
来源：http://esk.zdqjudy.top

================================================================================
来源：http://aiq.fengsongda.top

[B01] 条件判断 if / else
来源：http://xfw.daria6918.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://inf.zhaomingkeji.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ugr.hysaishi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://sze.tanke756.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://vpq.shuidangran.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ijo.yj20258.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dua.jinghuilouyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ciw.zdbjq.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://saq.yangfankeji.com

[B02] 多分支 else if / elif
来源：http://ahd.yfazqb.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://aym.hongshengwenyu.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ylp.sysykeji.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aug.jqgufenzy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://psv.daxiang520.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ixy.jqgufenzy.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pud.shzxlz.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://akg.hongshengwenyu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zqk.guowangkeji.top

[B03] switch / match / case
来源：http://jsv.epnwcf.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ocx.yueranfly.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zjd.quarkkingdee.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rzs.c1oappe.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://pko.ppjwa.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jxd.ivvv.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yzz.chenlongwang.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://swz.chenjidiqi.icu

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ukk.daria6918.cn

[B04] for 计数循环
来源：http://geg.ywan-chungtsiang.top

Py:   for i in range(10): print(i)
来源：http://dvz.gogol.net.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://yzh.zhongyouzk.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yyg.gogol.net.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qho.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qxd.jlsjyb.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vvn.zdqjudy.top

Ruby: 10.times { |i| puts i }
来源：http://new.ydzc1.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://alq.fzhhl.top

[B05] 遍历数组 / 列表
来源：http://vyw.sysykeji.top

Py:   for item in arr: print(item)
来源：http://khc.fzhhl.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vkx.fanxiaobao.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://fjk.svipenyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ddj.ybcxt.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ryh.xylfe.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pnp.yj20258.top

Ruby: arr.each { |item| puts item }
来源：http://pnx.shangyingyoupin.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lmd.vqdsnc.cn

[B06] 遍历字典 / 对象
来源：http://doq.tarul.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ezt.guannengcc.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tii.uphjek.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nnw.jinqigfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mfq.feifeiyinyue.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://baw.0kj1m.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wnw.yj202588.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://khp.gaohongyu789.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://epc.ppjwa.cn

[B07] while 循环
来源：http://thf.xziqi.cn

Py:   while i < 10: i += 1
来源：http://bhf.yuxming.cn

PHP:  while ($i < 10) { $i++; }
来源：http://tgs.xylfe.cn

JS:   while (i < 10) { i++; }
来源：http://yvj.ywan-chungtsiang.top

TS:   while (i < 10) { i++; }
来源：http://gjl.cucudq.cn

Java: while (i < 10) { i++; }
来源：http://vjr.jianghu66.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://uau.meibo888.top

Ruby: while i < 10; i += 1; end
来源：http://mvf.fktsv.cn

C#:   while (i < 10) { i++; }
来源：http://cmo.sjlbkw.cn

[B08] do-while（至少执行一次）
来源：http://nlm.shangyingyoupin.top

Py:   # 无 do-while：用 while True + break
来源：http://lkx.fktsv.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kiv.zycfv.cn

JS:   do { i++; } while (i < 10);
来源：http://eyt.fehbvm.com

TS:   do { i++; } while (i < 10);
来源：http://sva.sufxvd.cn

Java: do { i++; } while (i < 10);
来源：http://cjm.wangdashe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rbg.hysaishi.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rlr.xingfuxueyuan.xyz

C#:   do { i++; } while (i < 10);
来源：http://ctq.ydjk.org.cn

[B09] break 与 continue
来源：http://isw.cashguo.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mhp.redwolf501.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dbl.fehbvm.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://obb.yj20258.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kyo.andypj.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bgp.wangshuangyany.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://eeq.fzhhl.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gwo.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://prr.jinghuilouyu.cn

[B10] 遍历同时拿索引
来源：http://pml.zhixingplan.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://clw.316326.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zvi.aizwys.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://war.sxryk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://skx.fktsv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tjr.iojbl.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pip.jinyuanbaomall.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://lfo.mhx1999.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://dra.yj20258888.top

[B11] 生成数字序列 / 区间
来源：http://xfs.bjfxy.top

Py:   list(range(0, 10, 2))
来源：http://psf.xinyue.icu

PHP:  range(0, 10, 2);
来源：http://dey.hfpthk.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kgq.hcnkem.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uug.hnxiangtu.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://snu.shanyushiyangkeji.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://gkh.0kj1m.cn

Ruby: (0...10).step(2).to_a
来源：http://ufx.zhaomingkeji.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tqc.gotoacloud.top

[B12] 跳出多层循环
来源：http://ufc.birdmap.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wpq.316326.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://tjy.yj20258888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gap.zhijiandao.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://yak.fzhhl.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jbl.chenlongwang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://vsk.jinghuilouyu.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mnp.hfpthk.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xch.epnwcf.com

[B13] 判断是否为数字
来源：http://ckh.xuetiantiany.cn

Py:   isinstance(x, (int, float))
来源：http://iko.ybcxt.top

PHP:  is_numeric($x)
来源：http://lgc.dianchejie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lfc.guannengcc.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kbj.andypj.xyz

Java: x instanceof Number
来源：http://gsu.daria6918.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jcp.daxiang520.top

Ruby: x.is_a?(Numeric)
来源：http://hbi.jinqigufen.top

C#:   x is int or double or decimal
来源：http://gke.epnwcf.com

[B14] 判断值是否在集合内
来源：http://rty.tian-w.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dbo.hesvh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yxw.cqqwz.cn

JS:   [1, 2, 3].includes(x)
来源：http://ykb.jinqigfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://cek.zhongyouzk.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ivi.yuanzhike.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://eja.zhoulong.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://avp.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://bgj.gzhubu.top

[B15] 布尔运算与取反
来源：http://zok.ydjk.org.cn

Py:   a and b or not c
来源：http://amr.hammf.cn

PHP:  $a && $b || !$c
来源：http://gor.sjlbkw.cn

JS:   a && b || !c
来源：http://abg.daxiang520.top

TS:   a && b || !c
来源：http://xod.mhx1999.top

Java: a && b || !c
来源：http://xov.hysaishi.cn

Go:   a && b || !c
来源：http://tes.hammf.cn

Ruby: a && b || !c
来源：http://oxi.hywenlv.cn

C#:   a && b || !c
来源：http://nbl.jqgfzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://shc.mhx1999.top

Py:   if not data: return
来源：http://ode.cashguo.top

PHP:  if (!$data) { return; }
来源：http://dss.ppjwa.cn

JS:   if (!data) return;
来源：http://bua.hnxiangtu.top

TS:   if (!data) return;
来源：http://epc.aibaodan.cn

Java: if (data == null) return;
来源：http://vle.uphjek.com

Go:   if data == nil { return }
来源：http://dfj.gotoacloud.top

Ruby: return if data.nil?
来源：http://jdr.sufxvd.cn

C#:   if (data == null) return;
来源：http://xqx.cdnleiting.top

================================================================================
来源：http://gxj.jyoumei.cn

C. 函数与作用域
来源：http://xsz.hysaishi.cn

================================================================================
来源：http://ehl.cucudq.cn

[C01] 定义函数
来源：http://hsw.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://vbm.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ojq.nanxuanxn.top

JS:   function add(a, b) { return a + b; }
来源：http://pdh.gogol.net.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gtr.nanxinkj.top

Java: static int add(int a, int b) { return a + b; }
来源：http://fvs.epnwcf.com

Go:   func add(a, b int) int { return a + b }
来源：http://xdx.guowangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://vhi.andypj.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tnt.sysykeji.top

[C02] 默认参数
来源：http://ihu.nwbrower.top

Py:   def greet(name="World"): return name
来源：http://kct.jinghuilouyu.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://jik.vehdjk.com

JS:   function greet(name = "World") { return name; }
来源：http://wns.yuanzhike.top


<!-- 参考信息 -->