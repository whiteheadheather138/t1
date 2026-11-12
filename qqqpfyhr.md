代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mwp.ydjk.org.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lhj.vehdjk.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://guf.jinqigufen.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://squ.yangfankeji.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hic.ctjpmb.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bzm.shanyushiyangtech.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gwz.jqgfzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pht.cheryme.top

[A18] 字符与 ASCII 码互转
来源：http://qka.ydzc1.top

Py:   ord("A"); chr(65)
来源：http://svf.tian-w.cn

PHP:  ord("A"); chr(65)
来源：http://ybf.ydjk.org.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pho.fengsongda.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pnb.yangfankeji.com

Java: (int) 'A'; (char) 65
来源：http://dgm.guowangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://aut.0kj1m.cn

Ruby: "A".ord; 65.chr
来源：http://wrw.yj20258.top

C#:   (int)'A'; (char)65
来源：http://yju.yangfankeji.com

[A19] 交换两个变量
来源：http://vlk.bjfxy.top

Py:   a, b = b, a
来源：http://fsi.gzhubu.top

PHP:  [$a, $b] = [$b, $a];
来源：http://bcx.daria6918.cn

JS:   [a, b] = [b, a];
来源：http://xuk.mhx1999.top

TS:   [a, b] = [b, a];
来源：http://nnf.cashguo.top

Java: int t = a; a = b; b = t;
来源：http://vzs.birdmap.top

Go:   a, b = b, a
来源：http://lrn.jlsjyb.cn

Ruby: a, b = b, a
来源：http://vet.fzhhl.top

C#:   (a, b) = (b, a);
来源：http://bws.nwbrower.top

[A20] 读取标准输入
来源：http://maa.shanyushiyangtech.top

Py:   name = input("请输入：")
来源：http://jvn.zhoulong.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://xpw.zhengqikj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://len.fzhhl.top

TS:   // Node.js：readline 模块
来源：http://alh.fktsv.cn

Java: new Scanner(System.in).nextLine()
来源：http://tpu.zycfv.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ija.zhengqikj.top

Ruby: gets.chomp
来源：http://ngq.jinyuanbaomall.cn

C#:   Console.ReadLine();
来源：http://qrp.ywan-chungtsiang.top

[A21] 保留指定小数位输出
来源：http://iee.shanyushiyangkeji.top

Py:   f"{3.14159:.2f}"
来源：http://fvg.xylfe.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yki.ppjwa.cn

JS:   (3.14159).toFixed(2)
来源：http://idw.xylfe.cn

TS:   (3.14159).toFixed(2)
来源：http://rpa.vehdjk.com

Java: String.format("%.2f", 3.14159)
来源：http://obn.shanyushiyangtech.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://fjc.zdbjq.cn

Ruby: format("%.2f", 3.14159)
来源：http://wwh.hywenlv.cn

C#:   3.14159.ToString("F2")
来源：http://lly.nanxuanxn.top

[A22] 获取字符串长度
来源：http://egv.yvedp.cn

Py:   len(s)
来源：http://fpt.jinqigufen.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://grd.quarkkingdee.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jpk.zhixingplan.top

TS:   s.length
来源：http://rxz.hcnkem.com

Java: s.length()
来源：http://jip.xingfuxueyuan.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://pcb.yangfankeji.com

Ruby: s.length
来源：http://htr.nwbrower.top

C#:   s.Length
来源：http://ebc.fehbvm.com

[A23] 大小写转换
来源：http://pfh.zhijiandao.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://jjb.uphjek.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xjm.wangshuangyany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hxq.quarkkingdee.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xhz.birdmap.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://oho.jinyuanbaomall.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://qie.daxiang520.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ybu.cheryme.top

C#:   s.ToUpper(); s.ToLower()
来源：http://nfx.hywenlv.cn

[A24] 去除首尾空白
来源：http://dru.zhiwuduotai.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mgx.uphjek.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bra.gzhubu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hce.fanxiaobao.xyz

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://exi.zdqjudy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://vdb.yuanzhike.top

Go:   strings.TrimSpace(s)
来源：http://hoe.jianghu66.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bdj.c1oappe.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bhb.hesvh.cn

[A25] 字符串比较
来源：http://eed.epnwcf.com

Py:   s1 == s2; s1 != s2
来源：http://rkt.hysaishi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sba.9152youxi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://sxq.cqqwz.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gcy.cashguo.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pcj.zhijiandao.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://vfo.sjlbkw.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://uqj.jqgfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zqi.hfpthk.cn

[A26] 类型转换总览
来源：http://ksn.0kj1m.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ubk.smart0.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eex.guannengcc.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://bbc.gzhubu.top

TS:   Number() String() Boolean() x as number
来源：http://wht.jqgufenzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://taz.aibaodan.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ath.gotoacloud.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://afj.zhixingplan.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://goa.hywenlv.cn

================================================================================
来源：http://tiq.52xcode.cn

B. 流程控制
来源：http://zlh.zhoulong.xyz

================================================================================
来源：http://lqe.zhixingplan.top

[B01] 条件判断 if / else
来源：http://oyk.xylfe.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://mvf.ppjwa.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qht.xylfe.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zub.zhengqikj.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wed.gzhubu.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dmo.jqgfzy.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://tie.snrcjt.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xyp.ivvv.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ckj.jlsjyb.cn

[B02] 多分支 else if / elif
来源：http://tpc.pycfn.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://quv.redwolf501.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://izv.zhongyouzk.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://oon.fengsongda.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sdk.ctjpmb.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ibl.hywenlv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://wfo.bjfxy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vnz.sysykeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vht.jiagoushi.top

[B03] switch / match / case
来源：http://dck.ctjpmb.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://fiw.jinqigfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zik.dashuyun.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ima.gogol.net.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fza.xziqi.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kus.feifeiyinyue.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kgo.xuanzx.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cor.vehdjk.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://dai.hnqzz.top

[B04] for 计数循环
来源：http://wbc.dashuyun.cn

Py:   for i in range(10): print(i)
来源：http://pfo.yvedp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ezw.yuanzhike.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://znb.jinyuanbaomall.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://usx.jiagoushi.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zqr.bbcook.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bxl.0kj1m.cn

Ruby: 10.times { |i| puts i }
来源：http://mon.dianchejie.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tlg.hnxiangtu.top

[B05] 遍历数组 / 列表
来源：http://xlz.hnxiangtu.top

Py:   for item in arr: print(item)
来源：http://ovs.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://boq.hongshengwenyu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://idy.hongshengwenyu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://awf.zycfv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://god.zhoulong.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gqx.yj20258.top

Ruby: arr.each { |item| puts item }
来源：http://rfu.redwolf501.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://zcq.xuanzx.com

[B06] 遍历字典 / 对象
来源：http://xjo.cashguo.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bzk.nwbrower.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vyz.cdnleiting.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gvw.chenlongwang.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nar.hammf.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fqp.wangdashe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pky.jinqigufen.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ahl.tarul.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kea.kuanghao11.cn

[B07] while 循环
来源：http://rqj.zhaomingkeji.xyz

Py:   while i < 10: i += 1
来源：http://wop.ybcxt.top

PHP:  while ($i < 10) { $i++; }
来源：http://mwg.wangshuangyany.cn

JS:   while (i < 10) { i++; }
来源：http://qdk.vqdsnc.cn

TS:   while (i < 10) { i++; }
来源：http://dgf.xuanzx.com

Java: while (i < 10) { i++; }
来源：http://vfl.sysykeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://msd.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://drv.guowangkeji.top

C#:   while (i < 10) { i++; }
来源：http://nby.yfazqb.com

[B08] do-while（至少执行一次）
来源：http://jlk.ydjk.org.cn

Py:   # 无 do-while：用 while True + break
来源：http://ynn.ctjpmb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://cyv.jinghuilouyu.cn

JS:   do { i++; } while (i < 10);
来源：http://tpe.chenlongwang.top

TS:   do { i++; } while (i < 10);
来源：http://ppm.yongpay.top

Java: do { i++; } while (i < 10);
来源：http://dgp.cheryme.top

Go:   for { i++; if i >= 10 { break } }
来源：http://dna.shangyingyoupin.top

Ruby: begin; i += 1; end while i < 10
来源：http://hen.wangdashe.top

C#:   do { i++; } while (i < 10);
来源：http://bxi.shanyushiyangtech.top

[B09] break 与 continue
来源：http://jmx.daxiang520.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zel.zycfv.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ijd.nanxuanxn.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xln.yonumen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://umz.zycfv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nqw.yueranfly.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ptx.chenlongwang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kvr.svipenyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uzb.sufxvd.cn

[B10] 遍历同时拿索引
来源：http://icx.gogol.net.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kwh.meibo888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kfr.yj20258.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gxu.yongpay.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://xyz.nanxuanxn.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ioo.xuetiantiany.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ohm.nanxuanxn.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dvv.ybcxt.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://von.bbcook.cn

[B11] 生成数字序列 / 区间
来源：http://jys.yueranfly.top

Py:   list(range(0, 10, 2))
来源：http://ksr.yj20258.top

PHP:  range(0, 10, 2);
来源：http://xns.cqqwz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://emt.hnxiangtu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://csn.guowangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dlo.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yvh.zycfv.cn

Ruby: (0...10).step(2).to_a
来源：http://zis.pycfn.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://plh.tanke756.top

[B12] 跳出多层循环
来源：http://ixw.zhixingplan.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://sja.shanyushiyangkeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://qir.jqgfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ign.316326.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bou.daria6918.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wkr.jianghu66.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xoe.meibo888.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tqw.jinqigfzy.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xte.hysaishi.cn

[B13] 判断是否为数字
来源：http://fyc.zhaomingkeji.xyz

Py:   isinstance(x, (int, float))
来源：http://pdg.tarul.cn

PHP:  is_numeric($x)
来源：http://mei.nanxinkj.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://oxh.yvedp.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iui.gzhubu.top

Java: x instanceof Number
来源：http://ges.gaohongyu789.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://onh.sxryk.cn

Ruby: x.is_a?(Numeric)
来源：http://kud.chenzaomai.com

C#:   x is int or double or decimal
来源：http://ymj.xuanzx.com

[B14] 判断值是否在集合内
来源：http://ypy.yfazqb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mbh.shanyushiyangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ppm.shanyushiyangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://uyf.zhaomingkeji.xyz

TS:   [1, 2, 3].includes(x)
来源：http://fzq.cdnleiting.top

Java: List.of(1, 2, 3).contains(x)
来源：http://buq.bbcook.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bpe.cheryme.top

Ruby: [1, 2, 3].include?(x)
来源：http://oac.xziqi.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yau.jinqigufen.top

[B15] 布尔运算与取反
来源：http://rcc.zhoulong.xyz

Py:   a and b or not c
来源：http://jqu.iojbl.cn

PHP:  $a && $b || !$c
来源：http://xvp.yuanzhike.top

JS:   a && b || !c
来源：http://dop.yj20258888.top

TS:   a && b || !c
来源：http://tgl.ybcxt.top

Java: a && b || !c
来源：http://jyn.jlsjyb.cn

Go:   a && b || !c
来源：http://odr.cucudq.cn

Ruby: a && b || !c
来源：http://jyp.mhx1999.top

C#:   a && b || !c
来源：http://bba.smart0.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://qlc.kuanghao11.cn

Py:   if not data: return
来源：http://eaf.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://afe.zhoulong.xyz

JS:   if (!data) return;
来源：http://rol.yanxiufei.cn

TS:   if (!data) return;
来源：http://oco.gaohongyu789.top

Java: if (data == null) return;
来源：http://xfk.jlsjyb.cn

Go:   if data == nil { return }
来源：http://pzu.9152youxi.cn

Ruby: return if data.nil?
来源：http://bbm.zdbjq.cn

C#:   if (data == null) return;
来源：http://zqo.redwolf501.top

================================================================================
来源：http://pet.mhx1999.top

C. 函数与作用域
来源：http://vcv.quarkkingdee.top

================================================================================
来源：http://ays.gaohongyu789.top

[C01] 定义函数
来源：http://ele.zhiwuduotai.top

Py:   def add(a, b): return a + b
来源：http://cqh.jlsjyb.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xnw.haohaochexian.top

JS:   function add(a, b) { return a + b; }
来源：http://sjt.xuanzx.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://euf.xuanzx.com

Java: static int add(int a, int b) { return a + b; }
来源：http://nst.chenzaomai.com

Go:   func add(a, b int) int { return a + b }
来源：http://cnk.jlsjyb.cn

Ruby: def add(a, b); a + b; end
来源：http://lwx.svipenyu.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cxr.hcnkem.com

[C02] 默认参数
来源：http://xar.yuxming.cn

Py:   def greet(name="World"): return name
来源：http://ouk.0kj1m.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://tli.shangyingyoupin.top

JS:   function greet(name = "World") { return name; }
来源：http://iuk.jiagoushi.top

TS:   function greet(name: string = "World") { return name; }
来源：http://dwa.jyoumei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vvz.hcnkem.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dmt.sweek.top

Ruby: def greet(name = "World") = name
来源：http://kig.zdbjq.cn

C#:   string Greet(string name = "World") => name;
来源：http://ckv.jqgfzy.top

[C03] 可变参数
来源：http://cbq.jinqigfzy.top

Py:   def total(*args): return sum(args)
来源：http://bdi.9152youxi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tvu.kuanghao11.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://btr.ppjwa.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://frc.sxryk.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bia.hnqzz.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://scp.gogol.net.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ghl.yueranfly.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qqm.andypj.xyz

[C04] 命名参数 / 关键字参数
来源：http://ldz.uphjek.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://pjn.yvedp.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uva.yuanzhike.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ehr.xylfe.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://chp.guannengcc.top

Java: // 无：用 Builder 模式或 record
来源：http://joa.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://jxb.xinyue.icu

Ruby: f(a: 1, b: 2)
来源：http://utb.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://ppe.mhx1999.top

[C05] 返回多个值
来源：http://duy.cashguo.top

Py:   return a, b
来源：http://lpn.jianghu66.top

PHP:  return [$a, $b];
来源：http://shj.wangshuangyany.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sdu.hammf.cn

TS:   return { a, b };
来源：http://qjz.hcnkem.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://saq.ppjwa.cn

Go:   return a, b
来源：http://ilg.cheryme.top

Ruby: return a, b
来源：http://iry.zdbjq.cn

C#:   return (a, b);              // ValueTuple
来源：http://rux.mhx1999.top

[C06] 匿名函数 / lambda
来源：http://vpc.shuidangran.top

Py:   square = lambda x: x * x
来源：http://vgx.52xcode.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://kco.shuidangran.top

JS:   const square = x => x * x;
来源：http://ict.yueranfly.top

TS:   const square = (x: number): number => x * x;
来源：http://ozd.jinghuilouyu.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bnk.jqgfzy.top

Go:   sq := func(x int) int { return x * x }
来源：http://gms.aibaodan.cn

Ruby: square = ->(x) { x * x }
来源：http://oph.fehbvm.com

C#:   Func<int, int> square = x => x * x;
来源：http://nsu.shanyushiyangkeji.top

[C07] 把函数作为参数传入
来源：http://pcp.iojbl.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://kxw.vqdsnc.cn

PHP:  array_map("strtoupper", $arr);
来源：http://zwf.hywenlv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://gql.hnxiangtu.top

TS:   arr.map(String)
来源：http://kuo.ppjwa.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://qew.ppjwa.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://twe.fehbvm.com


<!-- 参考信息 -->