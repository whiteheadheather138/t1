代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zpt.wangshuangyany.cn

Ruby: unless x            # nil 与 false 为假
来源：http://jms.ctjpmb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uny.nwbrower.top

[A17] 位运算
来源：http://pie.52xcode.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wwi.yj20258888.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://qng.xylfe.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wdo.yfazqb.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://qrz.havefunace.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cde.jinyuanbaomall.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://not.haohaochexian.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hfw.tanke756.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kcn.cucudq.cn

[A18] 字符与 ASCII 码互转
来源：http://wpt.guowangkeji.top

Py:   ord("A"); chr(65)
来源：http://mxt.haohaochexian.top

PHP:  ord("A"); chr(65)
来源：http://xqw.hongshengwenyu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://iok.aibaodan.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fqs.tian-w.cn

Java: (int) 'A'; (char) 65
来源：http://nzr.jianghu66.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tfc.zdqjudy.top

Ruby: "A".ord; 65.chr
来源：http://aeu.hysaishi.cn

C#:   (int)'A'; (char)65
来源：http://ape.fengsongda.top

[A19] 交换两个变量
来源：http://iou.zhengqikj.top

Py:   a, b = b, a
来源：http://roh.meibo888.top

PHP:  [$a, $b] = [$b, $a];
来源：http://emk.jqgufenzy.top

JS:   [a, b] = [b, a];
来源：http://mhi.jqgfzy.top

TS:   [a, b] = [b, a];
来源：http://dpi.hysaishi.cn

Java: int t = a; a = b; b = t;
来源：http://tnb.zhijiandao.cn

Go:   a, b = b, a
来源：http://wlw.yj20258.top

Ruby: a, b = b, a
来源：http://eqz.epnwcf.com

C#:   (a, b) = (b, a);
来源：http://mjm.yangfankeji.com

[A20] 读取标准输入
来源：http://wtf.daxiang520.top

Py:   name = input("请输入：")
来源：http://wnj.ppjwa.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://gkf.cdnleiting.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hzc.wangdashe.top

TS:   // Node.js：readline 模块
来源：http://ztb.zhaomingkeji.xyz

Java: new Scanner(System.in).nextLine()
来源：http://yvb.jiagoushi.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://csg.quarkkingdee.top

Ruby: gets.chomp
来源：http://vfn.hesvh.cn

C#:   Console.ReadLine();
来源：http://zqb.epnwcf.com

[A21] 保留指定小数位输出
来源：http://opl.zhaomingkeji.xyz

Py:   f"{3.14159:.2f}"
来源：http://esj.daxiang520.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://qgd.hammf.cn

JS:   (3.14159).toFixed(2)
来源：http://qfr.bjfxy.top

TS:   (3.14159).toFixed(2)
来源：http://dxt.cucudq.cn

Java: String.format("%.2f", 3.14159)
来源：http://mth.xuanzx.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://avm.shanyushiyangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://ita.aibaodan.cn

C#:   3.14159.ToString("F2")
来源：http://eql.sjlbkw.cn

[A22] 获取字符串长度
来源：http://clq.xinyue.icu

Py:   len(s)
来源：http://wnc.jianghu66.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rmr.0kj1m.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://aqc.0kj1m.cn

TS:   s.length
来源：http://fwx.quarkkingdee.top

Java: s.length()
来源：http://dtp.zycfv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://awm.redwolf501.top

Ruby: s.length
来源：http://hiq.jinghuilouyu.cn

C#:   s.Length
来源：http://ver.kuanghao11.cn

[A23] 大小写转换
来源：http://jkk.ybcxt.top

Py:   s.upper(); s.lower(); s.title()
来源：http://fjg.yvedp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qyq.nanxuanxn.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tuu.haohaochexian.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://zpu.hnxiangtu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://opr.shanyushiyangtech.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sjx.nanxinkj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://jnv.hywenlv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://scm.tian-w.cn

[A24] 去除首尾空白
来源：http://kjc.sufxvd.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://gyd.jqgfzy.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ekx.yanxiufei.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nzp.feifeiyinyue.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vma.zdbjq.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wnh.dianchejie.cn

Go:   strings.TrimSpace(s)
来源：http://chn.yj20258.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sxy.mhx1999.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qdu.ppjwa.cn

[A25] 字符串比较
来源：http://wxo.zhengqikj.top

Py:   s1 == s2; s1 != s2
来源：http://nvj.xuanzx.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wwo.yuxming.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fml.cheryme.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://srn.aibaodan.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wdk.yangfankeji.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://fmf.wangshuangyany.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vma.cdnleiting.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://axy.xylfe.cn

[A26] 类型转换总览
来源：http://avk.ivvv.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://opb.gogol.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hzo.xuetiantiany.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tcc.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://cdm.wangdashe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kia.zhoulong.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fsr.tarul.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://axy.guannengcc.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://iej.haohaochexian.top

================================================================================
来源：http://wkf.hnxiangtu.top

B. 流程控制
来源：http://ocm.zhengqikj.top

================================================================================
来源：http://ang.cashguo.top

[B01] 条件判断 if / else
来源：http://opf.hfpthk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tud.fehbvm.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dtm.yfazqb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ebd.xuanzx.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qxk.andypj.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://ccc.hesvh.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jkb.yonumen.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yha.sufxvd.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://iig.pengpengdd.cyou

[B02] 多分支 else if / elif
来源：http://ewn.hysaishi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://skr.tian-w.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rqe.zhengqikj.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jgv.epnwcf.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dum.fengsongda.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jan.ywan-chungtsiang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://glw.tanke756.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://bsx.sysykeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://syj.chenzaomai.com

[B03] switch / match / case
来源：http://yjk.shanyushiyangkeji.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xkz.jinqigfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://afk.tarul.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bpo.yongpay.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nut.ehwqpu.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://oyy.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://zrd.bjfxy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://opm.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ydp.zhijiandao.cn

[B04] for 计数循环
来源：http://cyp.chenjidiqi.icu

Py:   for i in range(10): print(i)
来源：http://ktz.zhiwuduotai.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://uss.yj20258888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ubv.52xcode.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gsq.zhengqikj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://owm.wangdashe.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ajz.dashuyun.cn

Ruby: 10.times { |i| puts i }
来源：http://ziu.aibaodan.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vcg.daxiang520.top

[B05] 遍历数组 / 列表
来源：http://tkg.zhengqikj.top

Py:   for item in arr: print(item)
来源：http://hib.birdmap.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jfo.fktsv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ngm.shanyushiyangtech.top

TS:   for (const item of arr) { console.log(item); }
来源：http://eoq.meibo888.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://qng.gogol.net.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://roq.xziqi.cn

Ruby: arr.each { |item| puts item }
来源：http://ilz.yanxiufei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gwp.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://pos.tianlin.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://bhe.jianghu66.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bse.yuanzhike.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jjl.tian-w.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bbs.zdqjudy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mbu.hfpthk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://apx.yuanzhike.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fxn.mhx1999.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://own.cdnleiting.top

[B07] while 循环
来源：http://qcq.ppjwa.cn

Py:   while i < 10: i += 1
来源：http://dui.shzxlz.cn

PHP:  while ($i < 10) { $i++; }
来源：http://fjo.c1oappe.top

JS:   while (i < 10) { i++; }
来源：http://zvo.zdqjudy.top

TS:   while (i < 10) { i++; }
来源：http://iih.fanxiaobao.xyz

Java: while (i < 10) { i++; }
来源：http://hpk.gotoacloud.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yxt.cashguo.top

Ruby: while i < 10; i += 1; end
来源：http://lqd.jqgufenzy.top

C#:   while (i < 10) { i++; }
来源：http://wqv.sweek.top

[B08] do-while（至少执行一次）
来源：http://eih.shuidangran.top

Py:   # 无 do-while：用 while True + break
来源：http://jdl.fehbvm.com

PHP:  do { $i++; } while ($i < 10);
来源：http://fvp.hnxiangtu.top

JS:   do { i++; } while (i < 10);
来源：http://rip.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://afl.daxiang520.top

Java: do { i++; } while (i < 10);
来源：http://uxq.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://pkj.kuanghao11.cn

Ruby: begin; i += 1; end while i < 10
来源：http://ycx.hongshengwenyu.top

C#:   do { i++; } while (i < 10);
来源：http://exa.yj20258888.top

[B09] break 与 continue
来源：http://mfm.ydjk.org.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ofd.pengpengdd.cyou

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://set.316326.xyz

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cwn.wangshuangyany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://euu.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rjl.nanxinkj.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kzg.yj20258.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kjm.tanke756.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ohg.meibo888.top

[B10] 遍历同时拿索引
来源：http://ish.hywenlv.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://wwa.jinqigufen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://vqb.bbcook.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pwj.52xcode.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://oyv.uphjek.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://gpn.gogol.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://imi.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://aph.c1oappe.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lxy.hcnkem.com

[B11] 生成数字序列 / 区间
来源：http://amw.cheryme.top

Py:   list(range(0, 10, 2))
来源：http://vhw.xingfuxueyuan.xyz

PHP:  range(0, 10, 2);
来源：http://rps.zhengqikj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cii.yuanzhike.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uwx.xuanzx.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tpq.sufxvd.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://sms.ybcxt.top

Ruby: (0...10).step(2).to_a
来源：http://dsz.yongpay.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lxg.9152youxi.cn

[B12] 跳出多层循环
来源：http://mru.yangfankeji.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://csa.kuanghao11.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://cyi.yanxiufei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://yuk.aibaodan.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jna.yongpay.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jkb.chenlongwang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bth.daria6918.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://qfq.ehwqpu.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xrx.fktsv.cn

[B13] 判断是否为数字
来源：http://cfw.ehwqpu.com

Py:   isinstance(x, (int, float))
来源：http://rjy.cashguo.top

PHP:  is_numeric($x)
来源：http://tvt.birdmap.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hqg.jinyuanbaomall.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cgm.meibo888.top

Java: x instanceof Number
来源：http://atq.kuanghao11.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://sgu.shangyingyoupin.top

Ruby: x.is_a?(Numeric)
来源：http://vkj.nwbrower.top

C#:   x is int or double or decimal
来源：http://hem.jianghu66.top

[B14] 判断值是否在集合内
来源：http://kwn.daxiang520.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://iso.316326.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pco.gotoacloud.top

JS:   [1, 2, 3].includes(x)
来源：http://kvw.guannengcc.top

TS:   [1, 2, 3].includes(x)
来源：http://hoa.kuanghao11.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://omc.jianghu66.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lnj.ywan-chungtsiang.top

Ruby: [1, 2, 3].include?(x)
来源：http://xcp.zdbjq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yiz.zhiwuduotai.top

[B15] 布尔运算与取反
来源：http://efk.guowangkeji.top

Py:   a and b or not c
来源：http://mwk.daxiang520.top

PHP:  $a && $b || !$c
来源：http://srd.316326.xyz

JS:   a && b || !c
来源：http://imi.bbcook.cn

TS:   a && b || !c
来源：http://wlq.hammf.cn

Java: a && b || !c
来源：http://saj.chenzaomai.com

Go:   a && b || !c
来源：http://tlq.nanxinkj.top

Ruby: a && b || !c
来源：http://vab.xingfuxueyuan.xyz

C#:   a && b || !c
来源：http://xdg.ehwqpu.com

[B16] 卫语句：不满足条件提前返回
来源：http://cbd.jinqigufen.top

Py:   if not data: return
来源：http://sqd.c1oappe.top

PHP:  if (!$data) { return; }
来源：http://alb.gaohongyu789.top

JS:   if (!data) return;
来源：http://whu.mhx1999.top

TS:   if (!data) return;
来源：http://kds.jinyuanbaomall.cn

Java: if (data == null) return;
来源：http://ejv.xylfe.cn

Go:   if data == nil { return }
来源：http://sdf.hywenlv.cn

Ruby: return if data.nil?
来源：http://ggv.0kj1m.cn

C#:   if (data == null) return;
来源：http://hxs.birdmap.top

================================================================================
来源：http://ooi.cucudq.cn

C. 函数与作用域
来源：http://tgd.gaohongyu789.top

================================================================================
来源：http://mnx.guannengcc.top

[C01] 定义函数
来源：http://pof.tarul.cn

Py:   def add(a, b): return a + b
来源：http://cwq.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://faj.ydzc1.top

JS:   function add(a, b) { return a + b; }
来源：http://rpq.epnwcf.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lhs.aizwys.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://lsq.sysykeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://hdw.wangshuangyany.cn

Ruby: def add(a, b); a + b; end
来源：http://dzt.shangyingyoupin.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://tut.aibaodan.cn

[C02] 默认参数
来源：http://ryd.jqgufenzy.top

Py:   def greet(name="World"): return name
来源：http://yuq.sysykeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://jok.xuetiantiany.cn

JS:   function greet(name = "World") { return name; }
来源：http://ncj.zhoulong.xyz

TS:   function greet(name: string = "World") { return name; }
来源：http://xyl.jiagoushi.top

Java: // 无默认参数：方法重载或 Optional
来源：http://lth.hfpthk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mkd.sysykeji.top

Ruby: def greet(name = "World") = name
来源：http://qny.tarul.cn

C#:   string Greet(string name = "World") => name;
来源：http://pss.xingfuxueyuan.xyz

[C03] 可变参数
来源：http://muc.zhongyouzk.top

Py:   def total(*args): return sum(args)
来源：http://shv.snrcjt.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fqv.daxiang520.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pcg.zdbjq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mxt.ctjpmb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hun.svipenyu.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sie.316326.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://adc.pycfn.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wjv.0kj1m.cn

[C04] 命名参数 / 关键字参数
来源：http://hqx.xuetiantiany.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://erz.sweek.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kmd.jqgfzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xbl.ywan-chungtsiang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hfn.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://rqj.9152youxi.cn

Go:   // 无：用配置结构体参数
来源：http://ide.dashuyun.cn

Ruby: f(a: 1, b: 2)
来源：http://ogq.xuanzx.com

C#:   f(a: 1, b: 2)
来源：http://lwq.yuxming.cn

[C05] 返回多个值
来源：http://eud.iojbl.cn

Py:   return a, b
来源：http://yup.smart0.xyz

PHP:  return [$a, $b];
来源：http://pbs.c1oappe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://qvt.9152youxi.cn

TS:   return { a, b };
来源：http://uxl.tianlin.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://dkr.9152youxi.cn

Go:   return a, b
来源：http://mpz.xziqi.cn

Ruby: return a, b
来源：http://dqx.zhixingplan.top

C#:   return (a, b);              // ValueTuple
来源：http://qak.aizwys.cn

[C06] 匿名函数 / lambda
来源：http://oif.ydjk.org.cn

Py:   square = lambda x: x * x
来源：http://usz.sweek.top

PHP:  $square = fn($x) => $x * $x;
来源：http://meo.bjfxy.top

JS:   const square = x => x * x;
来源：http://nxu.sufxvd.cn

TS:   const square = (x: number): number => x * x;
来源：http://awn.redwolf501.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://rmr.nanxinkj.top

Go:   sq := func(x int) int { return x * x }
来源：http://cob.pycfn.com

Ruby: square = ->(x) { x * x }
来源：http://mvz.snrcjt.cn

C#:   Func<int, int> square = x => x * x;
来源：http://whs.ywan-chungtsiang.top

[C07] 把函数作为参数传入
来源：http://jgr.daxiang520.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://ynv.epnwcf.com

PHP:  array_map("strtoupper", $arr);
来源：http://nuc.xziqi.cn


<!-- 参考信息 -->