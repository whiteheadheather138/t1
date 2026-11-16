代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://obs.jianghu66.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ber.yangfankeji.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pjs.shzxlz.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qvw.shzxlz.cn

[A18] 字符与 ASCII 码互转
来源：http://tqk.yj202588.top

Py:   ord("A"); chr(65)
来源：http://hju.hywenlv.cn

PHP:  ord("A"); chr(65)
来源：http://ovf.c1oappe.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qoj.bbcook.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wmp.ppjwa.cn

Java: (int) 'A'; (char) 65
来源：http://wpj.shanyushiyangtech.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://adk.zdqjudy.top

Ruby: "A".ord; 65.chr
来源：http://gue.daria6918.cn

C#:   (int)'A'; (char)65
来源：http://buz.fanxiaobao.xyz

[A19] 交换两个变量
来源：http://wat.xuanzx.com

Py:   a, b = b, a
来源：http://xpr.cashguo.top

PHP:  [$a, $b] = [$b, $a];
来源：http://pcj.hongshengwenyu.top

JS:   [a, b] = [b, a];
来源：http://tnv.sysykeji.top

TS:   [a, b] = [b, a];
来源：http://kvt.jlsjyb.cn

Java: int t = a; a = b; b = t;
来源：http://oou.vehdjk.com

Go:   a, b = b, a
来源：http://wmf.cqqwz.cn

Ruby: a, b = b, a
来源：http://zpu.dianchejie.cn

C#:   (a, b) = (b, a);
来源：http://gbh.xinyue.icu

[A20] 读取标准输入
来源：http://oem.guannengcc.top

Py:   name = input("请输入：")
来源：http://usy.jianghu66.top

PHP:  $name = trim(fgets(STDIN));
来源：http://hqr.fktsv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vxo.zhoulong.xyz

TS:   // Node.js：readline 模块
来源：http://rma.shuidangran.top

Java: new Scanner(System.in).nextLine()
来源：http://naa.daxiang520.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yyk.fengsongda.top

Ruby: gets.chomp
来源：http://mlc.jiagoushi.top

C#:   Console.ReadLine();
来源：http://qva.ydjk.org.cn

[A21] 保留指定小数位输出
来源：http://mgg.fanxiaobao.xyz

Py:   f"{3.14159:.2f}"
来源：http://ele.sxryk.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xik.kuanghao11.cn

JS:   (3.14159).toFixed(2)
来源：http://fib.xziqi.cn

TS:   (3.14159).toFixed(2)
来源：http://bjp.yongpay.top

Java: String.format("%.2f", 3.14159)
来源：http://pdp.shuidangran.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mwn.shanyushiyangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://nnu.hammf.cn

C#:   3.14159.ToString("F2")
来源：http://aws.xziqi.cn

[A22] 获取字符串长度
来源：http://axj.ydjk.org.cn

Py:   len(s)
来源：http://cpo.zhoulong.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hrd.gotoacloud.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://omw.uphjek.com

TS:   s.length
来源：http://vcb.jqgfzy.top

Java: s.length()
来源：http://wvm.birdmap.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://vqt.jlsjyb.cn

Ruby: s.length
来源：http://ezj.xinyue.icu

C#:   s.Length
来源：http://wqj.ppjwa.cn

[A23] 大小写转换
来源：http://nwa.sjlbkw.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wfo.iojbl.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fns.dianchejie.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mab.yj20258888.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mbw.yj202588.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hok.chenlongwang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zbc.gotoacloud.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://elu.andypj.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://dsl.redwolf501.top

[A24] 去除首尾空白
来源：http://kla.zhaomingkeji.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tum.jiagoushi.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://iky.haohaochexian.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://efc.bjfxy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://byo.shanyushiyangtech.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jwx.fzhhl.top

Go:   strings.TrimSpace(s)
来源：http://kvm.yuxming.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://you.dianchejie.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yjk.aizwys.cn

[A25] 字符串比较
来源：http://ung.guowangkeji.top

Py:   s1 == s2; s1 != s2
来源：http://fmy.aibaodan.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sbn.yj20258.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rff.shuidangran.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://sxc.feifeiyinyue.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://won.wangshuangyany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ybv.vehdjk.com

Ruby: s1 == s2; s1 <=> s2
来源：http://ris.ppjwa.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://skd.hcnkem.com

[A26] 类型转换总览
来源：http://mea.cdnleiting.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zuc.guowangkeji.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jnf.yvedp.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fip.jianghu66.top

TS:   Number() String() Boolean() x as number
来源：http://zob.kuanghao11.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bdg.xuanzx.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qnm.zhiwuduotai.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://hhe.aibaodan.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://spx.ybcxt.top

================================================================================
来源：http://vsh.xylfe.cn

B. 流程控制
来源：http://bml.cashguo.top

================================================================================
来源：http://eoj.xylfe.cn

[B01] 条件判断 if / else
来源：http://zkk.jianghu66.top

Py:   result = "正" if x > 0 else "非正"
来源：http://gyf.yongpay.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qcz.ctjpmb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://csh.bbcook.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mlj.9152youxi.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dzc.mhx1999.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lot.jiagoushi.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vaw.tanke756.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jfp.hfpthk.cn

[B02] 多分支 else if / elif
来源：http://jft.iojbl.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vas.iojbl.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://tsc.dashuyun.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yli.jianghu66.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gcx.zhoulong.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ddi.zhengqikj.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ntb.yj20258.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://nzy.fehbvm.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gax.daxiang520.top

[B03] switch / match / case
来源：http://hzf.52xcode.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vzj.52xcode.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://koc.hesvh.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://crq.ehwqpu.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tid.hesvh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qnn.daxiang520.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kon.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mul.jqgfzy.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://alu.chenjidiqi.icu

[B04] for 计数循环
来源：http://ikt.shzxlz.cn

Py:   for i in range(10): print(i)
来源：http://axy.zhiwuduotai.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://elv.uphjek.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pqe.zdqjudy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zqi.hesvh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pzf.hammf.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vqm.nwbrower.top

Ruby: 10.times { |i| puts i }
来源：http://hlc.quarkkingdee.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hrc.dianchejie.cn

[B05] 遍历数组 / 列表
来源：http://lza.cqqwz.cn

Py:   for item in arr: print(item)
来源：http://qhj.tarul.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://fsh.ydzc1.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vpi.jianghu66.top

TS:   for (const item of arr) { console.log(item); }
来源：http://qat.vqdsnc.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wwn.gogol.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://fpy.xinyue.icu

Ruby: arr.each { |item| puts item }
来源：http://rek.chenjidiqi.icu

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ypd.tianlin.xyz

[B06] 遍历字典 / 对象
来源：http://cze.wangshuangyany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://mvh.ctjpmb.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://caq.kuanghao11.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yju.mhx1999.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jxs.0kj1m.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://crr.yangfankeji.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rmi.jqgufenzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cvx.hcnkem.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ulw.cucudq.cn

[B07] while 循环
来源：http://lux.9152youxi.cn

Py:   while i < 10: i += 1
来源：http://nwi.tian-w.cn

PHP:  while ($i < 10) { $i++; }
来源：http://niv.jyoumei.cn

JS:   while (i < 10) { i++; }
来源：http://hmp.dianchejie.cn

TS:   while (i < 10) { i++; }
来源：http://lzf.dashuyun.cn

Java: while (i < 10) { i++; }
来源：http://pgt.yj20258888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vzd.yj20258888.top

Ruby: while i < 10; i += 1; end
来源：http://flj.gzhubu.top

C#:   while (i < 10) { i++; }
来源：http://aqx.andypj.xyz

[B08] do-while（至少执行一次）
来源：http://hwq.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://jts.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gte.yangfankeji.com

JS:   do { i++; } while (i < 10);
来源：http://grr.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://qka.jlsjyb.cn

Java: do { i++; } while (i < 10);
来源：http://qrh.dashuyun.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://nsv.52xcode.cn

Ruby: begin; i += 1; end while i < 10
来源：http://hsg.fanxiaobao.xyz

C#:   do { i++; } while (i < 10);
来源：http://obg.fktsv.cn

[B09] break 与 continue
来源：http://wge.ivvv.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ysl.hnqzz.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jjz.vehdjk.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zwc.hammf.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mmi.vqdsnc.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pew.aizwys.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pfb.kuanghao11.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uyw.ctjpmb.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pez.xingfuxueyuan.xyz

[B10] 遍历同时拿索引
来源：http://pkn.jinqigfzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://szv.vehdjk.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://cqh.svipenyu.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tmu.chenlongwang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cko.gzhubu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://llc.ctjpmb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ugs.yonumen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eyd.ctjpmb.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bgy.jyoumei.cn

[B11] 生成数字序列 / 区间
来源：http://dqm.yongpay.top

Py:   list(range(0, 10, 2))
来源：http://vlc.yuanzhike.top

PHP:  range(0, 10, 2);
来源：http://ooc.shanyushiyangkeji.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sns.tarul.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xgy.redwolf501.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fom.kuanghao11.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sbw.gzhubu.top

Ruby: (0...10).step(2).to_a
来源：http://wxn.zhoulong.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fbp.hywenlv.cn

[B12] 跳出多层循环
来源：http://wza.cdnleiting.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://vyq.wangshuangyany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://fxn.gzhubu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://edc.epnwcf.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://crv.ydzc1.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hfh.bbcook.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ees.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dvl.meibo888.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rbx.yfazqb.com

[B13] 判断是否为数字
来源：http://zyw.fengsongda.top

Py:   isinstance(x, (int, float))
来源：http://bce.yvedp.cn

PHP:  is_numeric($x)
来源：http://gtj.wangshuangyany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ofi.zhiwuduotai.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hci.shanyushiyangkeji.top

Java: x instanceof Number
来源：http://yis.wangshuangyany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ryy.xinyue.icu

Ruby: x.is_a?(Numeric)
来源：http://wpx.hnxiangtu.top

C#:   x is int or double or decimal
来源：http://mqh.zdqjudy.top

[B14] 判断值是否在集合内
来源：http://afx.snrcjt.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://kfc.xingfuxueyuan.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mwc.hammf.cn

JS:   [1, 2, 3].includes(x)
来源：http://gra.aizwys.cn

TS:   [1, 2, 3].includes(x)
来源：http://tto.shanyushiyangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://wlz.zhijiandao.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hvz.aizwys.cn

Ruby: [1, 2, 3].include?(x)
来源：http://exw.fzhhl.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dol.guannengcc.top

[B15] 布尔运算与取反
来源：http://xnk.yanxiufei.cn

Py:   a and b or not c
来源：http://nmp.dianchejie.cn

PHP:  $a && $b || !$c
来源：http://zfz.yongpay.top

JS:   a && b || !c
来源：http://fwb.yonumen.top

TS:   a && b || !c
来源：http://gae.cashguo.top

Java: a && b || !c
来源：http://jai.hfpthk.cn

Go:   a && b || !c
来源：http://drv.bjfxy.top

Ruby: a && b || !c
来源：http://jmz.quarkkingdee.top

C#:   a && b || !c
来源：http://ddp.yuanzhike.top

[B16] 卫语句：不满足条件提前返回
来源：http://nhl.smart0.xyz

Py:   if not data: return
来源：http://sem.tarul.cn

PHP:  if (!$data) { return; }
来源：http://qpr.sxryk.cn

JS:   if (!data) return;
来源：http://ccd.andypj.xyz

TS:   if (!data) return;
来源：http://bgj.hongshengwenyu.top

Java: if (data == null) return;
来源：http://zzz.tian-w.cn

Go:   if data == nil { return }
来源：http://cbc.fehbvm.com

Ruby: return if data.nil?
来源：http://yjl.dashuyun.cn

C#:   if (data == null) return;
来源：http://orl.jinghuilouyu.cn

================================================================================
来源：http://wii.wangdashe.top

C. 函数与作用域
来源：http://sfw.xinyue.icu

================================================================================
来源：http://sqo.gotoacloud.top

[C01] 定义函数
来源：http://ikl.9152youxi.cn

Py:   def add(a, b): return a + b
来源：http://bro.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nyv.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://qxu.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://eut.fengsongda.top

Java: static int add(int a, int b) { return a + b; }
来源：http://cnl.shangyingyoupin.top

Go:   func add(a, b int) int { return a + b }
来源：http://tyk.yuanzhike.top

Ruby: def add(a, b); a + b; end
来源：http://beb.haohaochexian.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gqi.cucudq.cn

[C02] 默认参数
来源：http://soc.dashuyun.cn

Py:   def greet(name="World"): return name
来源：http://ctq.havefunace.top

PHP:  function greet($name = "World") { return $name; }
来源：http://fwn.zdqjudy.top

JS:   function greet(name = "World") { return name; }
来源：http://pyh.shangyingyoupin.top

TS:   function greet(name: string = "World") { return name; }
来源：http://xzx.guowangkeji.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pvg.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://fyi.aizwys.cn

Ruby: def greet(name = "World") = name
来源：http://jfu.chenjidiqi.icu

C#:   string Greet(string name = "World") => name;
来源：http://nsc.zhengqikj.top

[C03] 可变参数
来源：http://gja.meibo888.top

Py:   def total(*args): return sum(args)
来源：http://haf.smart0.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vau.mhx1999.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://eou.zdqjudy.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://bid.epnwcf.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://isn.nwbrower.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://lnx.daxiang520.top

Ruby: def total(*nums); nums.sum; end
来源：http://jfa.sufxvd.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wdx.havefunace.top

[C04] 命名参数 / 关键字参数
来源：http://sbp.gotoacloud.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fxa.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jkb.yongpay.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://aeq.andypj.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ysd.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://xrl.birdmap.top

Go:   // 无：用配置结构体参数
来源：http://nso.pengpengdd.cyou

Ruby: f(a: 1, b: 2)
来源：http://ocg.yvedp.cn

C#:   f(a: 1, b: 2)
来源：http://lyu.daria6918.cn

[C05] 返回多个值
来源：http://vos.ctjpmb.com

Py:   return a, b
来源：http://zbm.ivvv.top

PHP:  return [$a, $b];
来源：http://uvz.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://gge.yangfankeji.com

TS:   return { a, b };
来源：http://wrt.hysaishi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fzt.ywan-chungtsiang.top

Go:   return a, b
来源：http://svi.shangyingyoupin.top

Ruby: return a, b
来源：http://jur.zhengqikj.top

C#:   return (a, b);              // ValueTuple
来源：http://rgh.zhengqikj.top

[C06] 匿名函数 / lambda
来源：http://wuy.snrcjt.cn

Py:   square = lambda x: x * x
来源：http://oap.tarul.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lqo.tarul.cn

JS:   const square = x => x * x;
来源：http://eln.ivvv.top

TS:   const square = (x: number): number => x * x;
来源：http://rcu.svipenyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://oqu.yangfankeji.com

Go:   sq := func(x int) int { return x * x }
来源：http://oor.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://snb.tianlin.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://hnk.vehdjk.com

[C07] 把函数作为参数传入
来源：http://zmr.cdnleiting.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://stk.aizwys.cn

PHP:  array_map("strtoupper", $arr);
来源：http://juo.hnqzz.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yqp.gotoacloud.top

TS:   arr.map(String)
来源：http://xkt.tianlin.xyz

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://pqc.snrcjt.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kvl.zhoulong.xyz

Ruby: arr.map(&:upcase)
来源：http://grb.shanyushiyangtech.top

C#:   arr.Select(s => s.ToUpper())
来源：http://yhw.yj20258888.top

[C08] 闭包
来源：http://miy.meibo888.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://emc.redwolf501.top


<!-- 参考信息 -->