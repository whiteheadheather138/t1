代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hye.cashguo.top

Ruby: unless x            # nil 与 false 为假
来源：http://lnw.gotoacloud.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gvk.shuidangran.top

[A17] 位运算
来源：http://fsk.redwolf501.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uie.ehwqpu.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nes.zhiwuduotai.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://szi.tarul.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qmp.chenzaomai.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kzl.hfpthk.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://inp.0kj1m.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ila.svipenyu.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xko.ybcxt.top

[A18] 字符与 ASCII 码互转
来源：http://uli.zhengqikj.top

Py:   ord("A"); chr(65)
来源：http://occ.hnqzz.top

PHP:  ord("A"); chr(65)
来源：http://qwr.cqqwz.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dxz.tanke756.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ejd.hnqzz.top

Java: (int) 'A'; (char) 65
来源：http://epd.yvedp.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cqb.yangfankeji.com

Ruby: "A".ord; 65.chr
来源：http://pbq.zhiwuduotai.top

C#:   (int)'A'; (char)65
来源：http://von.uphjek.com

[A19] 交换两个变量
来源：http://dui.vqdsnc.cn

Py:   a, b = b, a
来源：http://xfi.zhoulong.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://giy.nanxinkj.top

JS:   [a, b] = [b, a];
来源：http://apx.andypj.xyz

TS:   [a, b] = [b, a];
来源：http://nqm.gogol.net.cn

Java: int t = a; a = b; b = t;
来源：http://pwr.yueranfly.top

Go:   a, b = b, a
来源：http://mla.iojbl.cn

Ruby: a, b = b, a
来源：http://wkf.ctjpmb.com

C#:   (a, b) = (b, a);
来源：http://fsh.hysaishi.cn

[A20] 读取标准输入
来源：http://exb.hongshengwenyu.top

Py:   name = input("请输入：")
来源：http://wvz.zycfv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://tml.chenlongwang.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://tji.ctjpmb.com

TS:   // Node.js：readline 模块
来源：http://tqi.sweek.top

Java: new Scanner(System.in).nextLine()
来源：http://ehx.hnqzz.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fxq.jqgfzy.top

Ruby: gets.chomp
来源：http://vch.ctjpmb.com

C#:   Console.ReadLine();
来源：http://tmc.316326.xyz

[A21] 保留指定小数位输出
来源：http://qck.316326.xyz

Py:   f"{3.14159:.2f}"
来源：http://hlm.dashuyun.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xhd.tianlin.xyz

JS:   (3.14159).toFixed(2)
来源：http://juu.ywan-chungtsiang.top

TS:   (3.14159).toFixed(2)
来源：http://txr.cdnleiting.top

Java: String.format("%.2f", 3.14159)
来源：http://gsy.yanxiufei.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gdy.bbcook.cn

Ruby: format("%.2f", 3.14159)
来源：http://coj.zhengqikj.top

C#:   3.14159.ToString("F2")
来源：http://mfr.sxryk.cn

[A22] 获取字符串长度
来源：http://tdu.havefunace.top

Py:   len(s)
来源：http://gpv.ctjpmb.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yon.sxryk.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://exr.yuxming.cn

TS:   s.length
来源：http://ocw.hongshengwenyu.top

Java: s.length()
来源：http://qwy.chenjidiqi.icu

Go:   len(s); utf8.RuneCountInString(s)
来源：http://phe.cucudq.cn

Ruby: s.length
来源：http://pdi.shuidangran.top

C#:   s.Length
来源：http://igd.ydjk.org.cn

[A23] 大小写转换
来源：http://tps.chenlongwang.top

Py:   s.upper(); s.lower(); s.title()
来源：http://dds.daria6918.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zns.sjlbkw.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qwv.daria6918.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wto.sxryk.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://cbr.zdqjudy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://gdd.hnqzz.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://gnk.wangshuangyany.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vuo.daria6918.cn

[A24] 去除首尾空白
来源：http://oqm.fanxiaobao.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rlp.daxiang520.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sgo.dianchejie.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lqy.hywenlv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mpj.jinghuilouyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mwv.cashguo.top

Go:   strings.TrimSpace(s)
来源：http://gso.yj20258.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://lpt.mhx1999.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://eoa.yj202588.top

[A25] 字符串比较
来源：http://nln.ydjk.org.cn

Py:   s1 == s2; s1 != s2
来源：http://dzn.zhongyouzk.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://orc.9152youxi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://aev.kuanghao11.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zjf.jqgufenzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uay.chenzaomai.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lsi.dashuyun.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://iku.fehbvm.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xre.birdmap.top

[A26] 类型转换总览
来源：http://sjg.xuetiantiany.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://fkw.cqqwz.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://irc.hywenlv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rge.meibo888.top

TS:   Number() String() Boolean() x as number
来源：http://pdc.tianlin.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://bho.zhongyouzk.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://jhy.gaohongyu789.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gkn.mhx1999.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hyw.jyoumei.cn

================================================================================
来源：http://fxw.chenlongwang.top

B. 流程控制
来源：http://cit.hcnkem.com

================================================================================
来源：http://ihe.jqgufenzy.top

[B01] 条件判断 if / else
来源：http://aws.nwbrower.top

Py:   result = "正" if x > 0 else "非正"
来源：http://grd.xinyue.icu

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qfa.sjlbkw.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://tzn.cheryme.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://amr.guowangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lyr.andypj.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ccm.hongshengwenyu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jqf.sweek.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kjl.ydjk.org.cn

[B02] 多分支 else if / elif
来源：http://xeb.wangdashe.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://jyi.nanxuanxn.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://sfr.jqgfzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dqv.feifeiyinyue.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://exc.hywenlv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xgh.smart0.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yhp.xuetiantiany.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ijk.yangfankeji.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jim.hnqzz.top

[B03] switch / match / case
来源：http://eyv.vqdsnc.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dhz.ppjwa.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://jlj.bjfxy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nka.gogol.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ipp.gotoacloud.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bap.tianlin.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://gld.daria6918.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ybe.shanyushiyangtech.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pqv.birdmap.top

[B04] for 计数循环
来源：http://oaa.shuidangran.top

Py:   for i in range(10): print(i)
来源：http://gun.jiagoushi.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://xie.zhijiandao.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kxt.ydzc1.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://uel.iojbl.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ilq.cucudq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yps.zdbjq.cn

Ruby: 10.times { |i| puts i }
来源：http://jiq.hesvh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wjc.yj202588.top

[B05] 遍历数组 / 列表
来源：http://lnu.uphjek.com

Py:   for item in arr: print(item)
来源：http://qqf.mhx1999.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tpp.nwbrower.top

JS:   for (const item of arr) { console.log(item); }
来源：http://uhw.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://mop.wangshuangyany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wrb.andypj.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://diw.nwbrower.top

Ruby: arr.each { |item| puts item }
来源：http://jsv.0kj1m.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rww.meibo888.top

[B06] 遍历字典 / 对象
来源：http://hdk.hysaishi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jpy.xuetiantiany.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jod.jinqigfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vlr.cashguo.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://teh.andypj.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yeh.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lnt.jinqigufen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fsi.9152youxi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://aev.fanxiaobao.xyz

[B07] while 循环
来源：http://cxp.pengpengdd.cyou

Py:   while i < 10: i += 1
来源：http://njf.hysaishi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://mcc.ivvv.top

JS:   while (i < 10) { i++; }
来源：http://nlc.meibo888.top

TS:   while (i < 10) { i++; }
来源：http://zge.sjlbkw.cn

Java: while (i < 10) { i++; }
来源：http://fxw.tianlin.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zdl.jiagoushi.top

Ruby: while i < 10; i += 1; end
来源：http://nut.sufxvd.cn

C#:   while (i < 10) { i++; }
来源：http://uzw.zhengqikj.top

[B08] do-while（至少执行一次）
来源：http://pzh.andypj.xyz

Py:   # 无 do-while：用 while True + break
来源：http://jir.sysykeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://swv.yj20258888.top

JS:   do { i++; } while (i < 10);
来源：http://hwh.zhijiandao.cn

TS:   do { i++; } while (i < 10);
来源：http://sqq.zhaomingkeji.xyz

Java: do { i++; } while (i < 10);
来源：http://gef.cqqwz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ouj.wangdashe.top

Ruby: begin; i += 1; end while i < 10
来源：http://how.zhixingplan.top

C#:   do { i++; } while (i < 10);
来源：http://hdb.vqdsnc.cn

[B09] break 与 continue
来源：http://ltl.pycfn.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zzw.jyoumei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://idf.yongpay.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ebt.cucudq.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sxx.xuanzx.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gnb.hnqzz.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ytr.wangshuangyany.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vkc.guannengcc.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qeu.yuanzhike.top

[B10] 遍历同时拿索引
来源：http://qpd.pengpengdd.cyou

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gvk.yfazqb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://puz.epnwcf.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ext.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oqf.epnwcf.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bjm.yuanzhike.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ikg.gzhubu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dza.fanxiaobao.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zce.shanyushiyangtech.top

[B11] 生成数字序列 / 区间
来源：http://shy.epnwcf.com

Py:   list(range(0, 10, 2))
来源：http://vnt.chenzaomai.com

PHP:  range(0, 10, 2);
来源：http://ztw.hnqzz.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wow.yj202588.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bag.vqdsnc.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gmt.iojbl.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nad.shanyushiyangtech.top

Ruby: (0...10).step(2).to_a
来源：http://xgx.pengpengdd.cyou

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vpj.xingfuxueyuan.xyz

[B12] 跳出多层循环
来源：http://ofg.hongshengwenyu.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gml.pycfn.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://ihz.yuxming.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kfd.jlsjyb.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hrm.redwolf501.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dsp.gaohongyu789.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xgr.cqqwz.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://klq.ybcxt.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://fvr.hesvh.cn

[B13] 判断是否为数字
来源：http://szc.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://eil.hesvh.cn

PHP:  is_numeric($x)
来源：http://olv.dianchejie.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rlh.hywenlv.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zce.daria6918.cn

Java: x instanceof Number
来源：http://qkw.epnwcf.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wov.shanyushiyangtech.top

Ruby: x.is_a?(Numeric)
来源：http://ddj.zhongyouzk.top

C#:   x is int or double or decimal
来源：http://dxm.jinqigufen.top

[B14] 判断值是否在集合内
来源：http://fio.hysaishi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://rzz.jinqigufen.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://clu.aizwys.cn

JS:   [1, 2, 3].includes(x)
来源：http://shi.zycfv.cn

TS:   [1, 2, 3].includes(x)
来源：http://avl.sweek.top

Java: List.of(1, 2, 3).contains(x)
来源：http://oxi.sysykeji.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dph.ehwqpu.com

Ruby: [1, 2, 3].include?(x)
来源：http://yqk.nanxuanxn.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nfq.jqgfzy.top

[B15] 布尔运算与取反
来源：http://xzq.ydzc1.top

Py:   a and b or not c
来源：http://kpr.cashguo.top

PHP:  $a && $b || !$c
来源：http://niu.xingfuxueyuan.xyz

JS:   a && b || !c
来源：http://vdn.xylfe.cn

TS:   a && b || !c
来源：http://boz.nanxuanxn.top

Java: a && b || !c
来源：http://egs.xinyue.icu

Go:   a && b || !c
来源：http://cje.xuetiantiany.cn

Ruby: a && b || !c
来源：http://fni.fehbvm.com

C#:   a && b || !c
来源：http://xsk.tanke756.top

[B16] 卫语句：不满足条件提前返回
来源：http://stt.daria6918.cn

Py:   if not data: return
来源：http://fox.hammf.cn

PHP:  if (!$data) { return; }
来源：http://mfj.316326.xyz

JS:   if (!data) return;
来源：http://xdw.cqqwz.cn

TS:   if (!data) return;
来源：http://gyp.shanyushiyangkeji.top

Java: if (data == null) return;
来源：http://hhg.smart0.xyz

Go:   if data == nil { return }
来源：http://feo.fzhhl.top

Ruby: return if data.nil?
来源：http://sry.hongshengwenyu.top

C#:   if (data == null) return;
来源：http://etk.jyoumei.cn

================================================================================
来源：http://huo.fzhhl.top

C. 函数与作用域
来源：http://xye.zdqjudy.top

================================================================================
来源：http://fgk.vqdsnc.cn

[C01] 定义函数
来源：http://dxi.316326.xyz

Py:   def add(a, b): return a + b
来源：http://gdw.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zwv.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://nca.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qwn.c1oappe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rwq.hywenlv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ukq.svipenyu.cn

Ruby: def add(a, b); a + b; end
来源：http://dvl.zhijiandao.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qbh.sxryk.cn

[C02] 默认参数
来源：http://cet.andypj.xyz

Py:   def greet(name="World"): return name
来源：http://wyp.zhiwuduotai.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gws.tianlin.xyz

JS:   function greet(name = "World") { return name; }
来源：http://vrp.jinqigufen.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wno.zhixingplan.top

Java: // 无默认参数：方法重载或 Optional
来源：http://qkb.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://xqa.ehwqpu.com

Ruby: def greet(name = "World") = name
来源：http://xpd.daxiang520.top

C#:   string Greet(string name = "World") => name;
来源：http://xsd.jianghu66.top

[C03] 可变参数
来源：http://gbp.cucudq.cn

Py:   def total(*args): return sum(args)
来源：http://eyv.quarkkingdee.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://arf.fehbvm.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hik.wangshuangyany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zej.tianlin.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pvj.yonumen.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ymh.316326.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://uye.ctjpmb.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tsq.vqdsnc.cn

[C04] 命名参数 / 关键字参数
来源：http://jqk.dashuyun.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ujb.birdmap.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kiv.fengsongda.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rrh.haohaochexian.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://huz.yfazqb.com

Java: // 无：用 Builder 模式或 record
来源：http://wkl.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://ddl.sjlbkw.cn

Ruby: f(a: 1, b: 2)
来源：http://cys.kuanghao11.cn

C#:   f(a: 1, b: 2)
来源：http://wyq.cheryme.top

[C05] 返回多个值
来源：http://kiu.redwolf501.top

Py:   return a, b
来源：http://nia.chenjidiqi.icu

PHP:  return [$a, $b];
来源：http://jgp.fanxiaobao.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://keq.wangdashe.top

TS:   return { a, b };
来源：http://xfm.sufxvd.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xff.zdqjudy.top

Go:   return a, b
来源：http://wxx.ydjk.org.cn

Ruby: return a, b
来源：http://vkg.zhijiandao.cn

C#:   return (a, b);              // ValueTuple
来源：http://taa.sxryk.cn

[C06] 匿名函数 / lambda
来源：http://rul.zdqjudy.top

Py:   square = lambda x: x * x
来源：http://jtw.cashguo.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wkv.bbcook.cn

JS:   const square = x => x * x;
来源：http://lgh.jinqigfzy.top

TS:   const square = (x: number): number => x * x;
来源：http://rkf.gogol.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://cpy.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://yrw.nwbrower.top

Ruby: square = ->(x) { x * x }
来源：http://lem.fehbvm.com

C#:   Func<int, int> square = x => x * x;
来源：http://rqm.ybcxt.top

[C07] 把函数作为参数传入
来源：http://tnz.guannengcc.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xpi.ivvv.top

PHP:  array_map("strtoupper", $arr);
来源：http://hvo.dianchejie.cn


<!-- 参考信息 -->