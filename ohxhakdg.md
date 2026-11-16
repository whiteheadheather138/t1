代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hgp.wangshuangyany.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ptk.smart0.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mkd.daria6918.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pfg.fzhhl.top

[A18] 字符与 ASCII 码互转
来源：http://aja.ybcxt.top

Py:   ord("A"); chr(65)
来源：http://giz.uphjek.com

PHP:  ord("A"); chr(65)
来源：http://jup.xuetiantiany.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xbp.guowangkeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pke.daxiang520.top

Java: (int) 'A'; (char) 65
来源：http://yqh.snrcjt.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dji.ybcxt.top

Ruby: "A".ord; 65.chr
来源：http://glo.tanke756.top

C#:   (int)'A'; (char)65
来源：http://qeu.zycfv.cn

[A19] 交换两个变量
来源：http://fiy.zhengqikj.top

Py:   a, b = b, a
来源：http://dlb.0kj1m.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://sia.epnwcf.com

JS:   [a, b] = [b, a];
来源：http://iii.daria6918.cn

TS:   [a, b] = [b, a];
来源：http://bxw.316326.xyz

Java: int t = a; a = b; b = t;
来源：http://haa.guowangkeji.top

Go:   a, b = b, a
来源：http://prh.fehbvm.com

Ruby: a, b = b, a
来源：http://lnh.jianghu66.top

C#:   (a, b) = (b, a);
来源：http://rnk.birdmap.top

[A20] 读取标准输入
来源：http://ilh.yuanzhike.top

Py:   name = input("请输入：")
来源：http://pwm.xingfuxueyuan.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://yzk.nanxinkj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vxn.hammf.cn

TS:   // Node.js：readline 模块
来源：http://bgc.sxryk.cn

Java: new Scanner(System.in).nextLine()
来源：http://fdl.mhx1999.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://aiu.shzxlz.cn

Ruby: gets.chomp
来源：http://ukc.52xcode.cn

C#:   Console.ReadLine();
来源：http://rxm.cashguo.top

[A21] 保留指定小数位输出
来源：http://qpo.mhx1999.top

Py:   f"{3.14159:.2f}"
来源：http://ylj.shuidangran.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fgd.guowangkeji.top

JS:   (3.14159).toFixed(2)
来源：http://dxy.zhaomingkeji.xyz

TS:   (3.14159).toFixed(2)
来源：http://rre.aizwys.cn

Java: String.format("%.2f", 3.14159)
来源：http://lgv.yfazqb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wqz.ctjpmb.com

Ruby: format("%.2f", 3.14159)
来源：http://abo.xylfe.cn

C#:   3.14159.ToString("F2")
来源：http://xpf.zhijiandao.cn

[A22] 获取字符串长度
来源：http://tqt.andypj.xyz

Py:   len(s)
来源：http://hir.xziqi.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zku.cucudq.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://qmx.hcnkem.com

TS:   s.length
来源：http://bxd.xuetiantiany.cn

Java: s.length()
来源：http://ohg.sxryk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oyz.zhijiandao.cn

Ruby: s.length
来源：http://vvb.zhaomingkeji.xyz

C#:   s.Length
来源：http://kfe.yj20258.top

[A23] 大小写转换
来源：http://isb.52xcode.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ujh.haohaochexian.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vcf.ybcxt.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://juc.jinqigfzy.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://nvq.gogol.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://npi.cucudq.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://epp.ydzc1.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vor.jinyuanbaomall.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wbx.shuidangran.top

[A24] 去除首尾空白
来源：http://ilb.hnqzz.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://iim.fengsongda.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jpw.gotoacloud.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://uof.xylfe.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yno.jqgfzy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kas.sjlbkw.cn

Go:   strings.TrimSpace(s)
来源：http://ejm.ybcxt.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wli.xuetiantiany.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://txl.zhongyouzk.top

[A25] 字符串比较
来源：http://kyg.sufxvd.cn

Py:   s1 == s2; s1 != s2
来源：http://fto.guannengcc.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vxq.hfpthk.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bbc.nanxuanxn.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://utm.yj202588.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jwr.svipenyu.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uql.vehdjk.com

Ruby: s1 == s2; s1 <=> s2
来源：http://vrf.shzxlz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://grg.yueranfly.top

[A26] 类型转换总览
来源：http://xue.hongshengwenyu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://btc.andypj.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jrq.haohaochexian.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://xsk.jinyuanbaomall.cn

TS:   Number() String() Boolean() x as number
来源：http://emc.smart0.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rjr.gotoacloud.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dua.yangfankeji.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://dmc.cheryme.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lfr.xinyue.icu

================================================================================
来源：http://rnu.xingfuxueyuan.xyz

B. 流程控制
来源：http://ycz.jyoumei.cn

================================================================================
来源：http://evi.ybcxt.top

[B01] 条件判断 if / else
来源：http://rgo.jinqigufen.top

Py:   result = "正" if x > 0 else "非正"
来源：http://yiw.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nds.tanke756.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://njy.uphjek.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mbe.jiagoushi.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://tmq.hongshengwenyu.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hnj.zhixingplan.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jpq.jlsjyb.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://vvf.9152youxi.cn

[B02] 多分支 else if / elif
来源：http://dnw.smart0.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://sja.mhx1999.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://llc.fehbvm.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bxl.guowangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fct.epnwcf.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iji.fanxiaobao.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://lyq.hysaishi.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://rqa.bbcook.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vja.fengsongda.top

[B03] switch / match / case
来源：http://ume.sxryk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://axo.xinyue.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yfa.zhengqikj.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://tbd.pengpengdd.cyou

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zwf.zdqjudy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://utm.jyoumei.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ovy.ydjk.org.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lco.hnqzz.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hmr.tanke756.top

[B04] for 计数循环
来源：http://krm.gogol.net.cn

Py:   for i in range(10): print(i)
来源：http://lls.hnxiangtu.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rfm.jyoumei.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://omz.hcnkem.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gir.ppjwa.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://umg.iojbl.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qxy.yueranfly.top

Ruby: 10.times { |i| puts i }
来源：http://uol.daria6918.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vvi.jyoumei.cn

[B05] 遍历数组 / 列表
来源：http://eyr.sysykeji.top

Py:   for item in arr: print(item)
来源：http://xeu.chenlongwang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://srv.cheryme.top

JS:   for (const item of arr) { console.log(item); }
来源：http://eft.ppjwa.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://ktp.jiagoushi.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ygf.iojbl.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://htl.mhx1999.top

Ruby: arr.each { |item| puts item }
来源：http://fth.yongpay.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://pfl.nanxinkj.top

[B06] 遍历字典 / 对象
来源：http://tua.gzhubu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://mja.havefunace.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zge.yj20258888.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://thi.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hyd.dianchejie.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lpw.jinghuilouyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kka.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://gvc.sufxvd.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://sbs.shangyingyoupin.top

[B07] while 循环
来源：http://nuz.0kj1m.cn

Py:   while i < 10: i += 1
来源：http://guh.hnqzz.top

PHP:  while ($i < 10) { $i++; }
来源：http://eis.52xcode.cn

JS:   while (i < 10) { i++; }
来源：http://sic.zhiwuduotai.top

TS:   while (i < 10) { i++; }
来源：http://oqe.gaohongyu789.top

Java: while (i < 10) { i++; }
来源：http://rrp.meibo888.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xex.quarkkingdee.top

Ruby: while i < 10; i += 1; end
来源：http://squ.sxryk.cn

C#:   while (i < 10) { i++; }
来源：http://pfn.sweek.top

[B08] do-while（至少执行一次）
来源：http://fnk.ydzc1.top

Py:   # 无 do-while：用 while True + break
来源：http://awp.zhixingplan.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ysi.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://mir.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://pjw.ehwqpu.com

Java: do { i++; } while (i < 10);
来源：http://uzy.chenjidiqi.icu

Go:   for { i++; if i >= 10 { break } }
来源：http://ffk.zhiwuduotai.top

Ruby: begin; i += 1; end while i < 10
来源：http://pmp.yfazqb.com

C#:   do { i++; } while (i < 10);
来源：http://dsg.yangfankeji.com

[B09] break 与 continue
来源：http://yzv.yonumen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rna.jiagoushi.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://xzu.zhoulong.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jcs.zhoulong.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mbo.cucudq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://inl.fzhhl.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nzh.hywenlv.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ntf.yuxming.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://iyz.ivvv.top

[B10] 遍历同时拿索引
来源：http://udh.zhoulong.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zsp.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xpk.nanxuanxn.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ynj.shuidangran.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://rts.jiagoushi.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lin.ywan-chungtsiang.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cor.aizwys.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cxq.nanxinkj.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pof.yonumen.top

[B11] 生成数字序列 / 区间
来源：http://bvp.feifeiyinyue.top

Py:   list(range(0, 10, 2))
来源：http://hgl.wangshuangyany.cn

PHP:  range(0, 10, 2);
来源：http://jvg.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://syx.shanyushiyangtech.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dwf.yj202588.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tsm.iojbl.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tzj.wangshuangyany.cn

Ruby: (0...10).step(2).to_a
来源：http://hxv.hcnkem.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jia.aibaodan.cn

[B12] 跳出多层循环
来源：http://wxc.ivvv.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://ahi.aibaodan.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://nic.gaohongyu789.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qbu.daxiang520.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://spf.haohaochexian.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jrg.nwbrower.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dih.quarkkingdee.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gaf.yangfankeji.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://evi.ppjwa.cn

[B13] 判断是否为数字
来源：http://yht.fehbvm.com

Py:   isinstance(x, (int, float))
来源：http://xos.vqdsnc.cn

PHP:  is_numeric($x)
来源：http://glt.wangdashe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gyz.nanxinkj.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vdd.xziqi.cn

Java: x instanceof Number
来源：http://eet.aizwys.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mya.9152youxi.cn

Ruby: x.is_a?(Numeric)
来源：http://nqu.shzxlz.cn

C#:   x is int or double or decimal
来源：http://ido.zhiwuduotai.top

[B14] 判断值是否在集合内
来源：http://bda.wangshuangyany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lbe.yangfankeji.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jye.nwbrower.top

JS:   [1, 2, 3].includes(x)
来源：http://zxd.vqdsnc.cn

TS:   [1, 2, 3].includes(x)
来源：http://grs.ydzc1.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dko.yfazqb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fbd.zhiwuduotai.top

Ruby: [1, 2, 3].include?(x)
来源：http://kcj.jinghuilouyu.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ksf.hnqzz.top

[B15] 布尔运算与取反
来源：http://pbn.yongpay.top

Py:   a and b or not c
来源：http://tnu.jinghuilouyu.cn

PHP:  $a && $b || !$c
来源：http://hfz.zhijiandao.cn

JS:   a && b || !c
来源：http://eij.zdqjudy.top

TS:   a && b || !c
来源：http://mbq.hesvh.cn

Java: a && b || !c
来源：http://ylj.svipenyu.cn

Go:   a && b || !c
来源：http://pta.shzxlz.cn

Ruby: a && b || !c
来源：http://mhf.chenjidiqi.icu

C#:   a && b || !c
来源：http://lvq.ydjk.org.cn

[B16] 卫语句：不满足条件提前返回
来源：http://sbz.chenzaomai.com

Py:   if not data: return
来源：http://rgc.ppjwa.cn

PHP:  if (!$data) { return; }
来源：http://ckw.shuidangran.top

JS:   if (!data) return;
来源：http://btb.guowangkeji.top

TS:   if (!data) return;
来源：http://cvf.cheryme.top

Java: if (data == null) return;
来源：http://byn.pycfn.com

Go:   if data == nil { return }
来源：http://xpy.ehwqpu.com

Ruby: return if data.nil?
来源：http://wrc.fzhhl.top

C#:   if (data == null) return;
来源：http://fei.cucudq.cn

================================================================================
来源：http://wzh.zhiwuduotai.top

C. 函数与作用域
来源：http://otf.yfazqb.com

================================================================================
来源：http://vxl.xuanzx.com

[C01] 定义函数
来源：http://fkd.ppjwa.cn

Py:   def add(a, b): return a + b
来源：http://qeh.yueranfly.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hqz.redwolf501.top

JS:   function add(a, b) { return a + b; }
来源：http://tan.guannengcc.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jwi.xinyue.icu

Java: static int add(int a, int b) { return a + b; }
来源：http://mfl.aizwys.cn

Go:   func add(a, b int) int { return a + b }
来源：http://esz.sweek.top

Ruby: def add(a, b); a + b; end
来源：http://xcz.chenlongwang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://big.fehbvm.com

[C02] 默认参数
来源：http://tgl.tianlin.xyz

Py:   def greet(name="World"): return name
来源：http://cpq.jqgfzy.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jcg.ivvv.top

JS:   function greet(name = "World") { return name; }
来源：http://qmg.chenjidiqi.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://gjl.hywenlv.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rlr.pycfn.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ghz.shanyushiyangkeji.top

Ruby: def greet(name = "World") = name
来源：http://hdk.zdbjq.cn

C#:   string Greet(string name = "World") => name;
来源：http://kmq.hcnkem.com

[C03] 可变参数
来源：http://nlt.sweek.top

Py:   def total(*args): return sum(args)
来源：http://eac.yvedp.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ozc.svipenyu.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rwd.yuanzhike.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vee.zhongyouzk.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vrz.andypj.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://xxj.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qqc.ybcxt.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xtm.yj202588.top

[C04] 命名参数 / 关键字参数
来源：http://rzc.shanyushiyangkeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tkd.jinqigfzy.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://juv.pengpengdd.cyou

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vxz.yanxiufei.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mbu.dashuyun.cn

Java: // 无：用 Builder 模式或 record
来源：http://jlj.jinqigufen.top

Go:   // 无：用配置结构体参数
来源：http://wtv.jinqigfzy.top

Ruby: f(a: 1, b: 2)
来源：http://wha.fanxiaobao.xyz

C#:   f(a: 1, b: 2)
来源：http://tbu.hongshengwenyu.top

[C05] 返回多个值
来源：http://zur.jinghuilouyu.cn

Py:   return a, b
来源：http://ipc.dianchejie.cn

PHP:  return [$a, $b];
来源：http://wpc.zycfv.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mlk.yuxming.cn

TS:   return { a, b };
来源：http://cez.sysykeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ixv.yonumen.top

Go:   return a, b
来源：http://icp.jqgufenzy.top

Ruby: return a, b
来源：http://buh.ywan-chungtsiang.top

C#:   return (a, b);              // ValueTuple
来源：http://jsk.zhongyouzk.top

[C06] 匿名函数 / lambda
来源：http://grr.nanxinkj.top

Py:   square = lambda x: x * x
来源：http://vvb.ywan-chungtsiang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://emx.redwolf501.top

JS:   const square = x => x * x;
来源：http://fjf.iojbl.cn

TS:   const square = (x: number): number => x * x;
来源：http://pxv.jqgfzy.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://obz.pycfn.com

Go:   sq := func(x int) int { return x * x }
来源：http://aer.xuanzx.com

Ruby: square = ->(x) { x * x }
来源：http://nmm.ivvv.top

C#:   Func<int, int> square = x => x * x;
来源：http://lsd.hongshengwenyu.top

[C07] 把函数作为参数传入
来源：http://nve.bbcook.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gni.9152youxi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://gdi.xuetiantiany.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mqd.jinghuilouyu.cn

TS:   arr.map(String)
来源：http://rkq.aibaodan.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hnf.jlsjyb.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://doi.yj20258888.top

Ruby: arr.map(&:upcase)
来源：http://nfo.nwbrower.top

C#:   arr.Select(s => s.ToUpper())
来源：http://xdr.nanxuanxn.top

[C08] 闭包
来源：http://wqt.tarul.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qbw.haohaochexian.top


<!-- 参考信息 -->