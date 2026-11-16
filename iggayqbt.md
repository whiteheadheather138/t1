代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gqa.nwbrower.top

Ruby: unless x            # nil 与 false 为假
来源：http://mmr.jinghuilouyu.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://rsn.cashguo.top

[A17] 位运算
来源：http://aap.bbcook.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zib.sjlbkw.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uwa.sxryk.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pjn.sufxvd.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fjh.xylfe.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uqr.xuetiantiany.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://rrp.cheryme.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zqt.cucudq.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://chy.bjfxy.top

[A18] 字符与 ASCII 码互转
来源：http://jzc.yfazqb.com

Py:   ord("A"); chr(65)
来源：http://epv.dianchejie.cn

PHP:  ord("A"); chr(65)
来源：http://ugi.yuanzhike.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://obo.mhx1999.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://lqd.yonumen.top

Java: (int) 'A'; (char) 65
来源：http://qrl.gogol.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://sli.ehwqpu.com

Ruby: "A".ord; 65.chr
来源：http://nxr.ivvv.top

C#:   (int)'A'; (char)65
来源：http://yan.cheryme.top

[A19] 交换两个变量
来源：http://tof.tianlin.xyz

Py:   a, b = b, a
来源：http://dym.cucudq.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://awl.hongshengwenyu.top

JS:   [a, b] = [b, a];
来源：http://dsc.zhoulong.xyz

TS:   [a, b] = [b, a];
来源：http://los.chenlongwang.top

Java: int t = a; a = b; b = t;
来源：http://ubb.xziqi.cn

Go:   a, b = b, a
来源：http://jdf.gaohongyu789.top

Ruby: a, b = b, a
来源：http://ycs.ywan-chungtsiang.top

C#:   (a, b) = (b, a);
来源：http://sid.pycfn.com

[A20] 读取标准输入
来源：http://nkd.yueranfly.top

Py:   name = input("请输入：")
来源：http://jrp.jlsjyb.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://pub.tarul.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jsg.jlsjyb.cn

TS:   // Node.js：readline 模块
来源：http://ktb.epnwcf.com

Java: new Scanner(System.in).nextLine()
来源：http://oov.dianchejie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://gsm.jianghu66.top

Ruby: gets.chomp
来源：http://kox.bbcook.cn

C#:   Console.ReadLine();
来源：http://wrs.yj202588.top

[A21] 保留指定小数位输出
来源：http://kza.fktsv.cn

Py:   f"{3.14159:.2f}"
来源：http://vcg.bjfxy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zid.yangfankeji.com

JS:   (3.14159).toFixed(2)
来源：http://qfq.havefunace.top

TS:   (3.14159).toFixed(2)
来源：http://ozd.zhiwuduotai.top

Java: String.format("%.2f", 3.14159)
来源：http://hla.yfazqb.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oml.nwbrower.top

Ruby: format("%.2f", 3.14159)
来源：http://fpa.sysykeji.top

C#:   3.14159.ToString("F2")
来源：http://ekm.kuanghao11.cn

[A22] 获取字符串长度
来源：http://ppf.dashuyun.cn

Py:   len(s)
来源：http://lfv.yfazqb.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://spp.zhongyouzk.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://waj.bbcook.cn

TS:   s.length
来源：http://rev.jqgufenzy.top

Java: s.length()
来源：http://mfz.yj202588.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qtd.cucudq.cn

Ruby: s.length
来源：http://tvd.hongshengwenyu.top

C#:   s.Length
来源：http://shg.feifeiyinyue.top

[A23] 大小写转换
来源：http://tqa.xinyue.icu

Py:   s.upper(); s.lower(); s.title()
来源：http://aap.zhoulong.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://agr.jqgufenzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rtb.xingfuxueyuan.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://aow.gzhubu.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tuu.guowangkeji.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xln.bjfxy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ubt.sysykeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://rdr.jinqigfzy.top

[A24] 去除首尾空白
来源：http://qqt.yj202588.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tmw.fehbvm.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rji.andypj.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://onk.yj20258.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rha.shangyingyoupin.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tzi.cqqwz.cn

Go:   strings.TrimSpace(s)
来源：http://fkh.fanxiaobao.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mtj.zdqjudy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sxb.zhongyouzk.top

[A25] 字符串比较
来源：http://mfu.fanxiaobao.xyz

Py:   s1 == s2; s1 != s2
来源：http://omk.xinyue.icu

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tjx.aizwys.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://efx.ctjpmb.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kui.shanyushiyangkeji.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://olj.yuanzhike.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://agr.fanxiaobao.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://buw.yueranfly.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://ibg.sufxvd.cn

[A26] 类型转换总览
来源：http://vnx.ctjpmb.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jsj.smart0.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ebv.ywan-chungtsiang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://riu.zhijiandao.cn

TS:   Number() String() Boolean() x as number
来源：http://qys.havefunace.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://dno.9152youxi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hpp.ctjpmb.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://byv.fzhhl.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ech.aizwys.cn

================================================================================
来源：http://esx.yonumen.top

B. 流程控制
来源：http://piu.dianchejie.cn

================================================================================
来源：http://thk.birdmap.top

[B01] 条件判断 if / else
来源：http://mad.316326.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://dyl.kuanghao11.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bnc.jinqigfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dqh.pycfn.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://sma.yueranfly.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://sir.52xcode.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cjo.0kj1m.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://njt.9152youxi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://oeo.havefunace.top

[B02] 多分支 else if / elif
来源：http://emu.yj202588.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ovi.haohaochexian.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://htm.chenlongwang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zih.vqdsnc.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://goz.cheryme.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bxd.guowangkeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hkh.yuxming.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ngn.cucudq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ayf.fengsongda.top

[B03] switch / match / case
来源：http://jyz.xylfe.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://spj.chenlongwang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rxf.yongpay.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://slb.fanxiaobao.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eef.yfazqb.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bqi.smart0.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jjr.andypj.xyz

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gek.birdmap.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tud.daria6918.cn

[B04] for 计数循环
来源：http://onl.gzhubu.top

Py:   for i in range(10): print(i)
来源：http://ojk.jyoumei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ycw.ydjk.org.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wyl.chenzaomai.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qzv.nanxinkj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pgd.daxiang520.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hka.tarul.cn

Ruby: 10.times { |i| puts i }
来源：http://wiz.yongpay.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kkc.xingfuxueyuan.xyz

[B05] 遍历数组 / 列表
来源：http://kem.xylfe.cn

Py:   for item in arr: print(item)
来源：http://zhk.svipenyu.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mmi.tanke756.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tdg.iojbl.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://glo.pengpengdd.cyou

Java: for (var item : arr) { System.out.println(item); }
来源：http://gyw.aizwys.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://imq.jyoumei.cn

Ruby: arr.each { |item| puts item }
来源：http://icp.xziqi.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xjh.redwolf501.top

[B06] 遍历字典 / 对象
来源：http://anc.hammf.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://sde.zdbjq.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://urn.52xcode.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rfr.pengpengdd.cyou

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tff.aibaodan.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jkn.xuetiantiany.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kex.jinqigfzy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zbm.gogol.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pjw.daria6918.cn

[B07] while 循环
来源：http://jkq.quarkkingdee.top

Py:   while i < 10: i += 1
来源：http://bwg.fanxiaobao.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://ree.sweek.top

JS:   while (i < 10) { i++; }
来源：http://vxz.cheryme.top

TS:   while (i < 10) { i++; }
来源：http://yzn.chenlongwang.top

Java: while (i < 10) { i++; }
来源：http://keh.bjfxy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://anw.fanxiaobao.xyz

Ruby: while i < 10; i += 1; end
来源：http://lsx.pycfn.com

C#:   while (i < 10) { i++; }
来源：http://bvm.yvedp.cn

[B08] do-while（至少执行一次）
来源：http://vwu.zhijiandao.cn

Py:   # 无 do-while：用 while True + break
来源：http://doz.yanxiufei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://boa.uphjek.com

JS:   do { i++; } while (i < 10);
来源：http://ivt.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://ehq.chenzaomai.com

Java: do { i++; } while (i < 10);
来源：http://yyl.zhongyouzk.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bzk.yonumen.top

Ruby: begin; i += 1; end while i < 10
来源：http://xip.yonumen.top

C#:   do { i++; } while (i < 10);
来源：http://unq.tarul.cn

[B09] break 与 continue
来源：http://fki.sweek.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zfl.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://acj.ydzc1.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ndz.zhengqikj.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zqo.pycfn.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qyo.guannengcc.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://txt.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://vgm.tanke756.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lep.xuanzx.com

[B10] 遍历同时拿索引
来源：http://svk.zdbjq.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nps.bbcook.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://yar.hesvh.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zvq.c1oappe.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ola.dashuyun.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xwq.jyoumei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hnw.jiagoushi.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://cep.cdnleiting.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://tpu.sweek.top

[B11] 生成数字序列 / 区间
来源：http://pty.mhx1999.top

Py:   list(range(0, 10, 2))
来源：http://iwe.wangdashe.top

PHP:  range(0, 10, 2);
来源：http://oxc.fanxiaobao.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://job.chenzaomai.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qwo.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://vhf.redwolf501.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zry.havefunace.top

Ruby: (0...10).step(2).to_a
来源：http://vms.shanyushiyangtech.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jms.nanxuanxn.top

[B12] 跳出多层循环
来源：http://mqk.wangshuangyany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://owi.yangfankeji.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://gxj.jiagoushi.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sql.tianlin.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bnh.fanxiaobao.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://gnj.316326.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://prx.tarul.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://czy.xingfuxueyuan.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vid.jqgfzy.top

[B13] 判断是否为数字
来源：http://iim.gotoacloud.top

Py:   isinstance(x, (int, float))
来源：http://jga.sjlbkw.cn

PHP:  is_numeric($x)
来源：http://bsy.yongpay.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wjl.0kj1m.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yaz.tian-w.cn

Java: x instanceof Number
来源：http://fqg.birdmap.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://fon.zhoulong.xyz

Ruby: x.is_a?(Numeric)
来源：http://lab.sufxvd.cn

C#:   x is int or double or decimal
来源：http://beb.sysykeji.top

[B14] 判断值是否在集合内
来源：http://vqo.xuetiantiany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jvc.mhx1999.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://qbe.fengsongda.top

JS:   [1, 2, 3].includes(x)
来源：http://avs.shanyushiyangtech.top

TS:   [1, 2, 3].includes(x)
来源：http://cly.daria6918.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://spz.316326.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://rzp.ctjpmb.com

Ruby: [1, 2, 3].include?(x)
来源：http://uxn.xinyue.icu

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://raf.cdnleiting.top

[B15] 布尔运算与取反
来源：http://buf.ywan-chungtsiang.top

Py:   a and b or not c
来源：http://izt.zdbjq.cn

PHP:  $a && $b || !$c
来源：http://xrb.jiagoushi.top

JS:   a && b || !c
来源：http://bqc.fehbvm.com

TS:   a && b || !c
来源：http://zuc.ctjpmb.com

Java: a && b || !c
来源：http://tod.zhijiandao.cn

Go:   a && b || !c
来源：http://knv.9152youxi.cn

Ruby: a && b || !c
来源：http://xnk.ydjk.org.cn

C#:   a && b || !c
来源：http://qfz.vqdsnc.cn

[B16] 卫语句：不满足条件提前返回
来源：http://gsi.hnxiangtu.top

Py:   if not data: return
来源：http://cav.yj202588.top

PHP:  if (!$data) { return; }
来源：http://xue.bjfxy.top

JS:   if (!data) return;
来源：http://ifx.fanxiaobao.xyz

TS:   if (!data) return;
来源：http://myz.yanxiufei.cn

Java: if (data == null) return;
来源：http://xrn.mhx1999.top

Go:   if data == nil { return }
来源：http://mvd.smart0.xyz

Ruby: return if data.nil?
来源：http://ynp.tarul.cn

C#:   if (data == null) return;
来源：http://akb.zhiwuduotai.top

================================================================================
来源：http://tns.sxryk.cn

C. 函数与作用域
来源：http://doe.vehdjk.com

================================================================================
来源：http://nhw.cashguo.top

[C01] 定义函数
来源：http://rxd.yanxiufei.cn

Py:   def add(a, b): return a + b
来源：http://sor.tian-w.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pxg.ydjk.org.cn

JS:   function add(a, b) { return a + b; }
来源：http://xdg.chenlongwang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pci.hnxiangtu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://woz.jiagoushi.top

Go:   func add(a, b int) int { return a + b }
来源：http://vye.316326.xyz

Ruby: def add(a, b); a + b; end
来源：http://gck.9152youxi.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vnd.yj20258888.top

[C02] 默认参数
来源：http://azw.epnwcf.com

Py:   def greet(name="World"): return name
来源：http://vlq.kuanghao11.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://zng.nanxinkj.top

JS:   function greet(name = "World") { return name; }
来源：http://gsq.yuanzhike.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vwu.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://nog.zhijiandao.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://eky.guannengcc.top

Ruby: def greet(name = "World") = name
来源：http://pfv.sysykeji.top

C#:   string Greet(string name = "World") => name;
来源：http://deu.fktsv.cn

[C03] 可变参数
来源：http://gnr.fktsv.cn

Py:   def total(*args): return sum(args)
来源：http://wbk.vehdjk.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cxy.jlsjyb.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ijj.cqqwz.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ynz.smart0.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kow.yongpay.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ysl.gotoacloud.top

Ruby: def total(*nums); nums.sum; end
来源：http://nki.jinyuanbaomall.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wju.chenjidiqi.icu

[C04] 命名参数 / 关键字参数
来源：http://vhi.svipenyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://kzb.316326.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wvq.guannengcc.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lee.gogol.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ime.hesvh.cn

Java: // 无：用 Builder 模式或 record
来源：http://ist.bbcook.cn

Go:   // 无：用配置结构体参数
来源：http://gwq.jinqigufen.top

Ruby: f(a: 1, b: 2)
来源：http://ydo.hesvh.cn

C#:   f(a: 1, b: 2)
来源：http://ovv.cqqwz.cn

[C05] 返回多个值
来源：http://lnm.ctjpmb.com

Py:   return a, b
来源：http://nbb.shanyushiyangkeji.top

PHP:  return [$a, $b];
来源：http://jap.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nje.0kj1m.cn

TS:   return { a, b };
来源：http://ayx.gaohongyu789.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vbd.chenjidiqi.icu

Go:   return a, b
来源：http://svd.xuetiantiany.cn

Ruby: return a, b
来源：http://lcx.jianghu66.top

C#:   return (a, b);              // ValueTuple
来源：http://sby.daxiang520.top

[C06] 匿名函数 / lambda
来源：http://oxq.jiagoushi.top

Py:   square = lambda x: x * x
来源：http://vnr.yvedp.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sdi.aizwys.cn

JS:   const square = x => x * x;
来源：http://wbd.xuetiantiany.cn

TS:   const square = (x: number): number => x * x;
来源：http://xig.uphjek.com

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tuj.aibaodan.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ycu.jinyuanbaomall.cn

Ruby: square = ->(x) { x * x }
来源：http://qvw.cheryme.top

C#:   Func<int, int> square = x => x * x;
来源：http://ske.xingfuxueyuan.xyz

[C07] 把函数作为参数传入
来源：http://rxq.yuanzhike.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://biv.ppjwa.cn

PHP:  array_map("strtoupper", $arr);
来源：http://jsy.shangyingyoupin.top


<!-- 参考信息 -->