代发 wailian999

[A14] 注释写法
来源：http://gsz.yj20258888.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://mqk.zycfv.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://kdn.zhoulong.xyz

JS:   // 单行；/* 多行 */
来源：http://daf.cashguo.top

TS:   // 单行；/* 多行 */
来源：http://knc.zhiwuduotai.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ytv.guannengcc.top

Go:   // 单行；/* 多行 */
来源：http://vyh.cheryme.top

Ruby: # 单行；=begin 多行 =end
来源：http://htq.bbcook.cn

C#:   // 单行；/* 多行 */
来源：http://ukt.xinyue.icu

[A15] 空值判断与默认值
来源：http://lpa.hongshengwenyu.top

Py:   value = data or "默认值"
来源：http://udw.316326.xyz

PHP:  $value = $data ?? "默认值";
来源：http://hmy.ywan-chungtsiang.top

JS:   const value = data ?? "默认值";
来源：http://qco.fzhhl.top

TS:   const value = data ?? "默认值";
来源：http://gco.gzhubu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sln.cashguo.top

Go:   if data == "" { data = "默认值" }
来源：http://aow.xziqi.cn

Ruby: value = data || "默认值"
来源：http://zre.wangshuangyany.cn

C#:   var value = data ?? "默认值";
来源：http://gtu.yvedp.cn

[A16] 真假值判断规则
来源：http://xub.epnwcf.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://lou.nwbrower.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://vro.ivvv.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hxf.jiagoushi.top

TS:   if (!x) {}
来源：http://jtw.ppjwa.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cui.snrcjt.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vpl.yvedp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://hxa.quarkkingdee.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ysp.9152youxi.cn

[A17] 位运算
来源：http://iqe.nanxinkj.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bhk.yangfankeji.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rek.meibo888.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zpv.hammf.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yvj.bjfxy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sua.svipenyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gdi.yonumen.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jrj.hywenlv.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gvk.feifeiyinyue.top

[A18] 字符与 ASCII 码互转
来源：http://epu.vehdjk.com

Py:   ord("A"); chr(65)
来源：http://aad.smart0.xyz

PHP:  ord("A"); chr(65)
来源：http://qow.wangdashe.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yxh.svipenyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tfp.feifeiyinyue.top

Java: (int) 'A'; (char) 65
来源：http://sko.nanxinkj.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://xuf.hysaishi.cn

Ruby: "A".ord; 65.chr
来源：http://aap.tanke756.top

C#:   (int)'A'; (char)65
来源：http://ycs.chenlongwang.top

[A19] 交换两个变量
来源：http://afc.gaohongyu789.top

Py:   a, b = b, a
来源：http://ucc.hammf.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://hge.shangyingyoupin.top

JS:   [a, b] = [b, a];
来源：http://yfd.sxryk.cn

TS:   [a, b] = [b, a];
来源：http://rpc.ywan-chungtsiang.top

Java: int t = a; a = b; b = t;
来源：http://son.fengsongda.top

Go:   a, b = b, a
来源：http://pya.ywan-chungtsiang.top

Ruby: a, b = b, a
来源：http://xrv.uphjek.com

C#:   (a, b) = (b, a);
来源：http://iaw.xuanzx.com

[A20] 读取标准输入
来源：http://lqk.jlsjyb.cn

Py:   name = input("请输入：")
来源：http://hnl.svipenyu.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ews.yj20258.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://zvc.gzhubu.top

TS:   // Node.js：readline 模块
来源：http://hoz.jinqigfzy.top

Java: new Scanner(System.in).nextLine()
来源：http://krk.hcnkem.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://bal.tarul.cn

Ruby: gets.chomp
来源：http://txj.yonumen.top

C#:   Console.ReadLine();
来源：http://fpz.gaohongyu789.top

[A21] 保留指定小数位输出
来源：http://cll.nwbrower.top

Py:   f"{3.14159:.2f}"
来源：http://nzg.fzhhl.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://iyq.nwbrower.top

JS:   (3.14159).toFixed(2)
来源：http://reu.zhijiandao.cn

TS:   (3.14159).toFixed(2)
来源：http://sec.jinghuilouyu.cn

Java: String.format("%.2f", 3.14159)
来源：http://oyk.fzhhl.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gqk.hfpthk.cn

Ruby: format("%.2f", 3.14159)
来源：http://ejk.wangshuangyany.cn

C#:   3.14159.ToString("F2")
来源：http://ktm.jyoumei.cn

[A22] 获取字符串长度
来源：http://duk.aizwys.cn

Py:   len(s)
来源：http://pnl.shangyingyoupin.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://juc.bbcook.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://caq.vqdsnc.cn

TS:   s.length
来源：http://tfs.nanxuanxn.top

Java: s.length()
来源：http://rdg.hongshengwenyu.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fwl.hnxiangtu.top

Ruby: s.length
来源：http://ipm.gotoacloud.top

C#:   s.Length
来源：http://lji.hfpthk.cn

[A23] 大小写转换
来源：http://ljp.fzhhl.top

Py:   s.upper(); s.lower(); s.title()
来源：http://bpx.0kj1m.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lol.havefunace.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://loq.zhixingplan.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lay.ybcxt.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eey.zycfv.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hlv.chenlongwang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://qfa.hesvh.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lyu.ybcxt.top

[A24] 去除首尾空白
来源：http://ldz.jyoumei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vma.jiagoushi.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lco.redwolf501.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zmf.yfazqb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rpp.hysaishi.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://byr.ybcxt.top

Go:   strings.TrimSpace(s)
来源：http://jpi.vehdjk.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://agx.yueranfly.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vwe.redwolf501.top

[A25] 字符串比较
来源：http://wbc.zhoulong.xyz

Py:   s1 == s2; s1 != s2
来源：http://vex.gogol.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vzv.birdmap.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uma.nanxuanxn.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bqf.vqdsnc.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://dcq.xinyue.icu

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://imy.gogol.net.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://xqr.zhaomingkeji.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nov.jinqigufen.top

[A26] 类型转换总览
来源：http://chp.shuidangran.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://usz.daria6918.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cug.yonumen.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://oav.tian-w.cn

TS:   Number() String() Boolean() x as number
来源：http://qqs.shangyingyoupin.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fhk.xuanzx.com

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vqm.quarkkingdee.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rri.mhx1999.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pvx.xuetiantiany.cn

================================================================================
来源：http://ydj.hcnkem.com

B. 流程控制
来源：http://xbh.vqdsnc.cn

================================================================================
来源：http://jxn.fanxiaobao.xyz

[B01] 条件判断 if / else
来源：http://gbg.c1oappe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://dqe.pycfn.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mfq.yanxiufei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cgx.xuanzx.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hov.aizwys.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://wss.iojbl.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xnh.jinghuilouyu.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ppx.zhixingplan.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jay.mhx1999.top

[B02] 多分支 else if / elif
来源：http://xyi.jlsjyb.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://wld.jqgfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ivf.cqqwz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xpl.jinqigufen.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xks.birdmap.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aai.hfpthk.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zzf.hywenlv.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rns.ybcxt.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://plk.pycfn.com

[B03] switch / match / case
来源：http://xrs.quarkkingdee.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mpi.vqdsnc.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zcu.cqqwz.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://icw.xziqi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vdc.yueranfly.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zbr.cucudq.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://tne.shzxlz.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lpp.cqqwz.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ctw.kuanghao11.cn

[B04] for 计数循环
来源：http://chc.jyoumei.cn

Py:   for i in range(10): print(i)
来源：http://tpq.jyoumei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://jmz.dashuyun.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lfv.hnqzz.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bjg.ppjwa.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://omo.cashguo.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://cva.gzhubu.top

Ruby: 10.times { |i| puts i }
来源：http://nvg.zhongyouzk.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zju.xziqi.cn

[B05] 遍历数组 / 列表
来源：http://xzj.smart0.xyz

Py:   for item in arr: print(item)
来源：http://hsi.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lln.zhengqikj.top

JS:   for (const item of arr) { console.log(item); }
来源：http://ptz.jqgfzy.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zve.yueranfly.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://tiu.52xcode.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://czh.hnqzz.top

Ruby: arr.each { |item| puts item }
来源：http://xhw.nanxuanxn.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gpq.xingfuxueyuan.xyz

[B06] 遍历字典 / 对象
来源：http://rad.shuidangran.top

Py:   for k, v in d.items(): print(k, v)
来源：http://shw.hywenlv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vpj.hesvh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://yde.ydzc1.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zwu.zhongyouzk.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xty.shanyushiyangtech.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://eid.fktsv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qdm.ppjwa.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xqy.uphjek.com

[B07] while 循环
来源：http://qhs.xuetiantiany.cn

Py:   while i < 10: i += 1
来源：http://kel.yj20258.top

PHP:  while ($i < 10) { $i++; }
来源：http://mtc.0kj1m.cn

JS:   while (i < 10) { i++; }
来源：http://iyq.zdbjq.cn

TS:   while (i < 10) { i++; }
来源：http://rnt.hnxiangtu.top

Java: while (i < 10) { i++; }
来源：http://dav.hesvh.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://owr.jinyuanbaomall.cn

Ruby: while i < 10; i += 1; end
来源：http://vxo.jqgufenzy.top

C#:   while (i < 10) { i++; }
来源：http://kea.guannengcc.top

[B08] do-while（至少执行一次）
来源：http://zyu.316326.xyz

Py:   # 无 do-while：用 while True + break
来源：http://qkn.zhengqikj.top

PHP:  do { $i++; } while ($i < 10);
来源：http://aor.0kj1m.cn

JS:   do { i++; } while (i < 10);
来源：http://yfo.nwbrower.top

TS:   do { i++; } while (i < 10);
来源：http://qft.sweek.top

Java: do { i++; } while (i < 10);
来源：http://qem.xinyue.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://rrt.bbcook.cn

Ruby: begin; i += 1; end while i < 10
来源：http://cae.dianchejie.cn

C#:   do { i++; } while (i < 10);
来源：http://ynw.yuanzhike.top

[B09] break 与 continue
来源：http://uud.ydzc1.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xyh.wangshuangyany.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tjt.mhx1999.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bfq.sysykeji.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://box.jyoumei.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hbt.yonumen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ozm.sjlbkw.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://umo.smart0.xyz

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fzj.dashuyun.cn

[B10] 遍历同时拿索引
来源：http://yvo.daria6918.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bvt.gotoacloud.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yha.jqgufenzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ptv.fehbvm.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://izk.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://jtn.xinyue.icu

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bae.zhijiandao.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://eht.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wtl.ivvv.top

[B11] 生成数字序列 / 区间
来源：http://xba.jinyuanbaomall.cn

Py:   list(range(0, 10, 2))
来源：http://dxj.zdbjq.cn

PHP:  range(0, 10, 2);
来源：http://bup.cdnleiting.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://raf.yueranfly.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://coa.meibo888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://abk.shzxlz.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ygd.fzhhl.top

Ruby: (0...10).step(2).to_a
来源：http://tkf.andypj.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://kyz.52xcode.cn

[B12] 跳出多层循环
来源：http://lvl.zhijiandao.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wsv.iojbl.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tev.dashuyun.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lpx.yj202588.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rny.dashuyun.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wpj.ydjk.org.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gde.ppjwa.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://eqt.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blq.fktsv.cn

[B13] 判断是否为数字
来源：http://pti.yangfankeji.com

Py:   isinstance(x, (int, float))
来源：http://ikt.sufxvd.cn

PHP:  is_numeric($x)
来源：http://ihb.xylfe.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mwr.mhx1999.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://emz.dianchejie.cn

Java: x instanceof Number
来源：http://igd.ppjwa.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://avw.birdmap.top

Ruby: x.is_a?(Numeric)
来源：http://hki.guannengcc.top

C#:   x is int or double or decimal
来源：http://xyh.nanxuanxn.top

[B14] 判断值是否在集合内
来源：http://dsj.tarul.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://zew.epnwcf.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://equ.shangyingyoupin.top

JS:   [1, 2, 3].includes(x)
来源：http://sjt.zhiwuduotai.top

TS:   [1, 2, 3].includes(x)
来源：http://ifj.cucudq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://cfn.316326.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wdn.fzhhl.top

Ruby: [1, 2, 3].include?(x)
来源：http://jbn.gaohongyu789.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dbw.jinqigfzy.top

[B15] 布尔运算与取反
来源：http://nvi.xuanzx.com

Py:   a and b or not c
来源：http://zmj.meibo888.top

PHP:  $a && $b || !$c
来源：http://gxc.nwbrower.top

JS:   a && b || !c
来源：http://xuf.sysykeji.top

TS:   a && b || !c
来源：http://gql.zhijiandao.cn

Java: a && b || !c
来源：http://ggb.hesvh.cn

Go:   a && b || !c
来源：http://gdt.wangshuangyany.cn

Ruby: a && b || !c
来源：http://elz.chenlongwang.top

C#:   a && b || !c
来源：http://eqo.ywan-chungtsiang.top

[B16] 卫语句：不满足条件提前返回
来源：http://uyq.daria6918.cn

Py:   if not data: return
来源：http://tjh.yj202588.top

PHP:  if (!$data) { return; }
来源：http://tid.jianghu66.top

JS:   if (!data) return;
来源：http://iqw.sysykeji.top

TS:   if (!data) return;
来源：http://xmk.hnqzz.top

Java: if (data == null) return;
来源：http://swg.zdbjq.cn

Go:   if data == nil { return }
来源：http://gvv.redwolf501.top

Ruby: return if data.nil?
来源：http://qws.sweek.top

C#:   if (data == null) return;
来源：http://xis.jqgfzy.top

================================================================================
来源：http://kxo.aibaodan.cn

C. 函数与作用域
来源：http://hpa.tian-w.cn

================================================================================
来源：http://ljr.yj20258.top

[C01] 定义函数
来源：http://cah.aibaodan.cn

Py:   def add(a, b): return a + b
来源：http://tnd.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uhg.cqqwz.cn

JS:   function add(a, b) { return a + b; }
来源：http://qeo.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kkm.hongshengwenyu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://rzv.xylfe.cn

Go:   func add(a, b int) int { return a + b }
来源：http://jfx.dianchejie.cn

Ruby: def add(a, b); a + b; end
来源：http://cfw.shzxlz.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ylg.ywan-chungtsiang.top

[C02] 默认参数
来源：http://fca.dianchejie.cn

Py:   def greet(name="World"): return name
来源：http://uqa.yanxiufei.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://aip.jyoumei.cn

JS:   function greet(name = "World") { return name; }
来源：http://huv.fzhhl.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tqm.aibaodan.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://nru.haohaochexian.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ijp.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://sya.zhaomingkeji.xyz

C#:   string Greet(string name = "World") => name;
来源：http://jbt.ydzc1.top

[C03] 可变参数
来源：http://mjs.gogol.net.cn

Py:   def total(*args): return sum(args)
来源：http://gqa.zhiwuduotai.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://oiu.nwbrower.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lbj.aizwys.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yvx.yj202588.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://izj.ywan-chungtsiang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://qul.gzhubu.top

Ruby: def total(*nums); nums.sum; end
来源：http://ezz.birdmap.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ezc.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://war.gaohongyu789.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wec.gzhubu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kzq.sweek.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://eeg.jlsjyb.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pcg.zhaomingkeji.xyz

Java: // 无：用 Builder 模式或 record
来源：http://jow.tian-w.cn


<!-- 参考信息 -->