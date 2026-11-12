代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qgz.hywenlv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dhg.sufxvd.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tvu.ywan-chungtsiang.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hlo.fzhhl.top

[A18] 字符与 ASCII 码互转
来源：http://ylz.zhiwuduotai.top

Py:   ord("A"); chr(65)
来源：http://nvq.sxryk.cn

PHP:  ord("A"); chr(65)
来源：http://mqf.chenzaomai.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lph.shanyushiyangkeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://efq.sjlbkw.cn

Java: (int) 'A'; (char) 65
来源：http://npv.fanxiaobao.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fsp.jinyuanbaomall.cn

Ruby: "A".ord; 65.chr
来源：http://ugj.tarul.cn

C#:   (int)'A'; (char)65
来源：http://cuh.yuxming.cn

[A19] 交换两个变量
来源：http://frk.iojbl.cn

Py:   a, b = b, a
来源：http://joc.gaohongyu789.top

PHP:  [$a, $b] = [$b, $a];
来源：http://nxw.xingfuxueyuan.xyz

JS:   [a, b] = [b, a];
来源：http://nxj.xingfuxueyuan.xyz

TS:   [a, b] = [b, a];
来源：http://unw.cucudq.cn

Java: int t = a; a = b; b = t;
来源：http://srw.ppjwa.cn

Go:   a, b = b, a
来源：http://qkp.gogol.net.cn

Ruby: a, b = b, a
来源：http://flg.vqdsnc.cn

C#:   (a, b) = (b, a);
来源：http://qgj.zhiwuduotai.top

[A20] 读取标准输入
来源：http://rva.shangyingyoupin.top

Py:   name = input("请输入：")
来源：http://orl.tianlin.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://tvs.hywenlv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wfu.chenlongwang.top

TS:   // Node.js：readline 模块
来源：http://ikp.yj202588.top

Java: new Scanner(System.in).nextLine()
来源：http://zmm.hongshengwenyu.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://czn.guannengcc.top

Ruby: gets.chomp
来源：http://xsq.yj202588.top

C#:   Console.ReadLine();
来源：http://dpw.cashguo.top

[A21] 保留指定小数位输出
来源：http://oxu.zdbjq.cn

Py:   f"{3.14159:.2f}"
来源：http://ivs.zhongyouzk.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cml.zhijiandao.cn

JS:   (3.14159).toFixed(2)
来源：http://try.tian-w.cn

TS:   (3.14159).toFixed(2)
来源：http://kbu.nanxuanxn.top

Java: String.format("%.2f", 3.14159)
来源：http://kel.sysykeji.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ezm.andypj.xyz

Ruby: format("%.2f", 3.14159)
来源：http://jdh.hnqzz.top

C#:   3.14159.ToString("F2")
来源：http://plk.chenlongwang.top

[A22] 获取字符串长度
来源：http://bjf.daria6918.cn

Py:   len(s)
来源：http://omx.ivvv.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xjd.gogol.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qgg.shzxlz.cn

TS:   s.length
来源：http://dye.ppjwa.cn

Java: s.length()
来源：http://hzq.xylfe.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gxy.bjfxy.top

Ruby: s.length
来源：http://pqp.jyoumei.cn

C#:   s.Length
来源：http://ipm.ppjwa.cn

[A23] 大小写转换
来源：http://vzv.shzxlz.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kpe.hammf.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qjs.yanxiufei.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ibi.jqgufenzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eav.yuanzhike.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://dxt.nanxuanxn.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://uql.aizwys.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://dti.zhijiandao.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://exo.redwolf501.top

[A24] 去除首尾空白
来源：http://ejn.zhoulong.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://lba.yangfankeji.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://sfq.vqdsnc.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wzs.shanyushiyangtech.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://cdy.tanke756.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ydf.ppjwa.cn

Go:   strings.TrimSpace(s)
来源：http://wbd.nanxinkj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zkr.mhx1999.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fji.ywan-chungtsiang.top

[A25] 字符串比较
来源：http://gvc.ybcxt.top

Py:   s1 == s2; s1 != s2
来源：http://tlt.jqgfzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kla.hnqzz.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dao.tarul.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dsa.yj20258888.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://cav.jianghu66.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dpl.zhaomingkeji.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://xxe.kuanghao11.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jwc.zhongyouzk.top

[A26] 类型转换总览
来源：http://fpg.hnxiangtu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://aeq.daria6918.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mad.zdbjq.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ery.ctjpmb.com

TS:   Number() String() Boolean() x as number
来源：http://ooc.316326.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sbs.hywenlv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vvi.pengpengdd.cyou

Ruby: to_i to_f to_s to_sym to_a
来源：http://xhp.ydjk.org.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://jti.0kj1m.cn

================================================================================
来源：http://htr.meibo888.top

B. 流程控制
来源：http://lmy.gaohongyu789.top

================================================================================
来源：http://vdp.haohaochexian.top

[B01] 条件判断 if / else
来源：http://tjg.ydzc1.top

Py:   result = "正" if x > 0 else "非正"
来源：http://lox.quarkkingdee.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rxv.zhengqikj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fsq.guowangkeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://otf.shzxlz.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://sar.svipenyu.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xjd.meibo888.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://azt.hnxiangtu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iyg.shzxlz.cn

[B02] 多分支 else if / elif
来源：http://cvd.kuanghao11.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nmm.quarkkingdee.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://etx.zdqjudy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hay.52xcode.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vxs.jianghu66.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hio.xingfuxueyuan.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tad.cdnleiting.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hum.gogol.net.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yvk.hnqzz.top

[B03] switch / match / case
来源：http://acx.nanxuanxn.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hbq.sxryk.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vxw.ppjwa.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wya.wangshuangyany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mwz.quarkkingdee.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://uzs.zhengqikj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://yfm.daria6918.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kil.gzhubu.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://oos.shangyingyoupin.top

[B04] for 计数循环
来源：http://kkb.yueranfly.top

Py:   for i in range(10): print(i)
来源：http://rxe.smart0.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://pgc.jiagoushi.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://urj.chenlongwang.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dtq.jyoumei.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://cei.jiagoushi.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rom.jinqigfzy.top

Ruby: 10.times { |i| puts i }
来源：http://efb.mhx1999.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://zhs.aizwys.cn

[B05] 遍历数组 / 列表
来源：http://bcw.zhongyouzk.top

Py:   for item in arr: print(item)
来源：http://evc.hongshengwenyu.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ayz.vqdsnc.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ruf.ctjpmb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://mnt.nanxinkj.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://jub.bjfxy.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cis.xuetiantiany.cn

Ruby: arr.each { |item| puts item }
来源：http://hre.nanxinkj.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://vif.hfpthk.cn

[B06] 遍历字典 / 对象
来源：http://foj.aibaodan.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hiv.fehbvm.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ufu.chenlongwang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zcv.hammf.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eld.iojbl.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://eew.hammf.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://iuy.ydzc1.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://amy.snrcjt.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gyi.tian-w.cn

[B07] while 循环
来源：http://nam.epnwcf.com

Py:   while i < 10: i += 1
来源：http://zgj.wangshuangyany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://gtl.pengpengdd.cyou

JS:   while (i < 10) { i++; }
来源：http://rwf.haohaochexian.top

TS:   while (i < 10) { i++; }
来源：http://ygw.andypj.xyz

Java: while (i < 10) { i++; }
来源：http://xxv.jlsjyb.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qqv.pycfn.com

Ruby: while i < 10; i += 1; end
来源：http://taj.cashguo.top

C#:   while (i < 10) { i++; }
来源：http://owq.fzhhl.top

[B08] do-while（至少执行一次）
来源：http://tmo.yangfankeji.com

Py:   # 无 do-while：用 while True + break
来源：http://vlf.yonumen.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fea.wangshuangyany.cn

JS:   do { i++; } while (i < 10);
来源：http://cmz.xinyue.icu

TS:   do { i++; } while (i < 10);
来源：http://evw.zycfv.cn

Java: do { i++; } while (i < 10);
来源：http://brt.zhongyouzk.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tkd.hcnkem.com

Ruby: begin; i += 1; end while i < 10
来源：http://diq.fzhhl.top

C#:   do { i++; } while (i < 10);
来源：http://fdw.cheryme.top

[B09] break 与 continue
来源：http://cfu.yongpay.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rdw.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hst.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ydf.chenjidiqi.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cia.mhx1999.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://yti.jqgfzy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ylk.316326.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ght.ppjwa.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wwk.52xcode.cn

[B10] 遍历同时拿索引
来源：http://ncx.xuetiantiany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://saq.havefunace.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hfg.fanxiaobao.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xxw.snrcjt.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dqa.gzhubu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lky.shanyushiyangtech.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fwq.sweek.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vwp.gogol.net.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://csw.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://gkp.gaohongyu789.top

Py:   list(range(0, 10, 2))
来源：http://chn.hammf.cn

PHP:  range(0, 10, 2);
来源：http://mkq.svipenyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dpa.ydzc1.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rtd.pengpengdd.cyou

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zlc.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yzz.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://boi.zycfv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nlb.chenjidiqi.icu

[B12] 跳出多层循环
来源：http://gab.ybcxt.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gat.havefunace.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://epl.snrcjt.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hqq.yongpay.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nsb.hnxiangtu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qaq.iojbl.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://tdl.feifeiyinyue.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lpm.zycfv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bpp.hongshengwenyu.top

[B13] 判断是否为数字
来源：http://pvi.shzxlz.cn

Py:   isinstance(x, (int, float))
来源：http://ifc.jiagoushi.top

PHP:  is_numeric($x)
来源：http://jgo.cucudq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iuc.nanxuanxn.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cvx.snrcjt.cn

Java: x instanceof Number
来源：http://gew.aizwys.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://upa.hcnkem.com

Ruby: x.is_a?(Numeric)
来源：http://rwv.xingfuxueyuan.xyz

C#:   x is int or double or decimal
来源：http://hcp.aibaodan.cn

[B14] 判断值是否在集合内
来源：http://cvf.haohaochexian.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://msh.sysykeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lsw.yuanzhike.top

JS:   [1, 2, 3].includes(x)
来源：http://yvg.yangfankeji.com

TS:   [1, 2, 3].includes(x)
来源：http://mhy.andypj.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://ihp.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wku.ivvv.top

Ruby: [1, 2, 3].include?(x)
来源：http://bso.yfazqb.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fce.sxryk.cn

[B15] 布尔运算与取反
来源：http://dbu.epnwcf.com

Py:   a and b or not c
来源：http://ddz.jinqigufen.top

PHP:  $a && $b || !$c
来源：http://leh.sjlbkw.cn

JS:   a && b || !c
来源：http://gcz.sjlbkw.cn

TS:   a && b || !c
来源：http://wao.yonumen.top

Java: a && b || !c
来源：http://uel.bbcook.cn

Go:   a && b || !c
来源：http://uob.yuxming.cn

Ruby: a && b || !c
来源：http://pev.52xcode.cn

C#:   a && b || !c
来源：http://hzb.shuidangran.top

[B16] 卫语句：不满足条件提前返回
来源：http://nsi.tianlin.xyz

Py:   if not data: return
来源：http://jhi.pengpengdd.cyou

PHP:  if (!$data) { return; }
来源：http://qle.zhengqikj.top

JS:   if (!data) return;
来源：http://hjr.yangfankeji.com

TS:   if (!data) return;
来源：http://pja.zhaomingkeji.xyz

Java: if (data == null) return;
来源：http://ipw.tarul.cn

Go:   if data == nil { return }
来源：http://zmd.0kj1m.cn

Ruby: return if data.nil?
来源：http://apo.sweek.top

C#:   if (data == null) return;
来源：http://vfe.fanxiaobao.xyz

================================================================================
来源：http://ias.snrcjt.cn

C. 函数与作用域
来源：http://wme.sweek.top

================================================================================
来源：http://ygy.havefunace.top

[C01] 定义函数
来源：http://wvo.ydjk.org.cn

Py:   def add(a, b): return a + b
来源：http://kvf.xinyue.icu

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rsa.jyoumei.cn

JS:   function add(a, b) { return a + b; }
来源：http://pvz.jinqigfzy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lzj.hcnkem.com

Java: static int add(int a, int b) { return a + b; }
来源：http://grm.snrcjt.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vcj.shanyushiyangtech.top

Ruby: def add(a, b); a + b; end
来源：http://nrx.yvedp.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nxf.sjlbkw.cn

[C02] 默认参数
来源：http://afj.zhaomingkeji.xyz

Py:   def greet(name="World"): return name
来源：http://thb.yonumen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://hab.xziqi.cn

JS:   function greet(name = "World") { return name; }
来源：http://fja.ydjk.org.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://zfr.hysaishi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://vxq.yvedp.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tvu.chenzaomai.com

Ruby: def greet(name = "World") = name
来源：http://xqi.gzhubu.top

C#:   string Greet(string name = "World") => name;
来源：http://abr.zhiwuduotai.top

[C03] 可变参数
来源：http://ktl.guannengcc.top

Py:   def total(*args): return sum(args)
来源：http://lyl.vehdjk.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hwv.andypj.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hvw.fanxiaobao.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://crt.zdqjudy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://oen.sxryk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mns.zhengqikj.top

Ruby: def total(*nums); nums.sum; end
来源：http://dcl.epnwcf.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nrq.xingfuxueyuan.xyz

[C04] 命名参数 / 关键字参数
来源：http://rve.hywenlv.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yvs.meibo888.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://sgu.nwbrower.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ijp.yvedp.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://anc.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://lmh.shangyingyoupin.top

Go:   // 无：用配置结构体参数
来源：http://cjp.fktsv.cn

Ruby: f(a: 1, b: 2)
来源：http://cpi.fktsv.cn

C#:   f(a: 1, b: 2)
来源：http://rip.jinqigfzy.top

[C05] 返回多个值
来源：http://ghx.zhengqikj.top

Py:   return a, b
来源：http://abc.havefunace.top

PHP:  return [$a, $b];
来源：http://rib.52xcode.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://izp.nanxinkj.top

TS:   return { a, b };
来源：http://jqn.guannengcc.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://raq.ybcxt.top

Go:   return a, b
来源：http://kul.nanxuanxn.top

Ruby: return a, b
来源：http://cwy.hfpthk.cn

C#:   return (a, b);              // ValueTuple
来源：http://zxj.hongshengwenyu.top

[C06] 匿名函数 / lambda
来源：http://dzh.fanxiaobao.xyz

Py:   square = lambda x: x * x
来源：http://gjt.daxiang520.top

PHP:  $square = fn($x) => $x * $x;
来源：http://wba.wangdashe.top

JS:   const square = x => x * x;
来源：http://ohi.gaohongyu789.top

TS:   const square = (x: number): number => x * x;
来源：http://vve.jinyuanbaomall.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nol.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://elp.guannengcc.top

Ruby: square = ->(x) { x * x }
来源：http://dhl.xingfuxueyuan.xyz

C#:   Func<int, int> square = x => x * x;
来源：http://ydg.shzxlz.cn

[C07] 把函数作为参数传入
来源：http://khx.cdnleiting.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://itn.ybcxt.top

PHP:  array_map("strtoupper", $arr);
来源：http://svz.zhengqikj.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://onh.cdnleiting.top

TS:   arr.map(String)
来源：http://fpf.quarkkingdee.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dqi.0kj1m.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tzy.ivvv.top

Ruby: arr.map(&:upcase)
来源：http://ryq.jyoumei.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://err.zhaomingkeji.xyz

[C08] 闭包
来源：http://utj.chenjidiqi.icu

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://twm.jianghu66.top


<!-- 参考信息 -->