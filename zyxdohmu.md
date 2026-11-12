代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://nes.cqqwz.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lui.zycfv.cn

TS:   if (!x) {}
来源：http://tev.havefunace.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fpv.yuanzhike.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kqa.fanxiaobao.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://upr.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ybw.sufxvd.cn

[A17] 位运算
来源：http://wsd.shangyingyoupin.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kwx.ivvv.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://imy.xuanzx.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mwn.bjfxy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://yjr.vqdsnc.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://efm.zdbjq.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wih.hnqzz.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sdh.yongpay.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rgr.jianghu66.top

[A18] 字符与 ASCII 码互转
来源：http://eio.shuidangran.top

Py:   ord("A"); chr(65)
来源：http://lws.fehbvm.com

PHP:  ord("A"); chr(65)
来源：http://wbb.cucudq.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ycn.dashuyun.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wjc.uphjek.com

Java: (int) 'A'; (char) 65
来源：http://dfm.fktsv.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qze.pycfn.com

Ruby: "A".ord; 65.chr
来源：http://sin.tian-w.cn

C#:   (int)'A'; (char)65
来源：http://wvv.shanyushiyangtech.top

[A19] 交换两个变量
来源：http://wcc.chenzaomai.com

Py:   a, b = b, a
来源：http://dxl.yj202588.top

PHP:  [$a, $b] = [$b, $a];
来源：http://xwt.vehdjk.com

JS:   [a, b] = [b, a];
来源：http://tlv.yfazqb.com

TS:   [a, b] = [b, a];
来源：http://hch.sxryk.cn

Java: int t = a; a = b; b = t;
来源：http://irw.fzhhl.top

Go:   a, b = b, a
来源：http://xsi.jyoumei.cn

Ruby: a, b = b, a
来源：http://vmw.meibo888.top

C#:   (a, b) = (b, a);
来源：http://orp.yanxiufei.cn

[A20] 读取标准输入
来源：http://qqc.havefunace.top

Py:   name = input("请输入：")
来源：http://aor.aizwys.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wem.jinqigufen.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oxm.shanyushiyangtech.top

TS:   // Node.js：readline 模块
来源：http://sgm.hnxiangtu.top

Java: new Scanner(System.in).nextLine()
来源：http://ybt.tian-w.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qrp.quarkkingdee.top

Ruby: gets.chomp
来源：http://qfn.ehwqpu.com

C#:   Console.ReadLine();
来源：http://wtx.sysykeji.top

[A21] 保留指定小数位输出
来源：http://izb.hongshengwenyu.top

Py:   f"{3.14159:.2f}"
来源：http://fad.jianghu66.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mdy.daxiang520.top

JS:   (3.14159).toFixed(2)
来源：http://wjj.fanxiaobao.xyz

TS:   (3.14159).toFixed(2)
来源：http://wrc.gogol.net.cn

Java: String.format("%.2f", 3.14159)
来源：http://tqx.nanxuanxn.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://rtf.daxiang520.top

Ruby: format("%.2f", 3.14159)
来源：http://iji.zhixingplan.top

C#:   3.14159.ToString("F2")
来源：http://fqx.shuidangran.top

[A22] 获取字符串长度
来源：http://nfz.316326.xyz

Py:   len(s)
来源：http://nnz.fengsongda.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rke.jlsjyb.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zuf.sxryk.cn

TS:   s.length
来源：http://yts.havefunace.top

Java: s.length()
来源：http://gnz.tarul.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ryb.yvedp.cn

Ruby: s.length
来源：http://zlo.gogol.net.cn

C#:   s.Length
来源：http://qso.zhoulong.xyz

[A23] 大小写转换
来源：http://tkn.nwbrower.top

Py:   s.upper(); s.lower(); s.title()
来源：http://hix.nanxuanxn.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://qtd.zhengqikj.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://umx.aibaodan.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jmc.guannengcc.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tse.chenlongwang.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xib.quarkkingdee.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fhd.zhixingplan.top

C#:   s.ToUpper(); s.ToLower()
来源：http://ixx.yuxming.cn

[A24] 去除首尾空白
来源：http://fqb.fzhhl.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qua.fktsv.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://djd.tian-w.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ykz.fengsongda.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ulv.chenzaomai.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xgl.gzhubu.top

Go:   strings.TrimSpace(s)
来源：http://ool.tanke756.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bhr.cdnleiting.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ivu.svipenyu.cn

[A25] 字符串比较
来源：http://tan.redwolf501.top

Py:   s1 == s2; s1 != s2
来源：http://lxv.ppjwa.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tkv.cheryme.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://pqh.wangdashe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vtd.cdnleiting.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ogw.zhaomingkeji.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hgd.xylfe.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ztr.shzxlz.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sgn.cqqwz.cn

[A26] 类型转换总览
来源：http://rfx.shzxlz.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zor.jiagoushi.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ixo.zhaomingkeji.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tbg.kuanghao11.cn

TS:   Number() String() Boolean() x as number
来源：http://gcd.haohaochexian.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://thi.cheryme.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vdm.aibaodan.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lff.zdqjudy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ncb.cheryme.top

================================================================================
来源：http://koi.redwolf501.top

B. 流程控制
来源：http://uaj.iojbl.cn

================================================================================
来源：http://vyj.birdmap.top

[B01] 条件判断 if / else
来源：http://yxx.cucudq.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://pcv.hywenlv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aqd.snrcjt.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://bpa.jianghu66.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://cma.hfpthk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://jet.wangshuangyany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gnd.sjlbkw.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fgj.fanxiaobao.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zjp.nanxuanxn.top

[B02] 多分支 else if / elif
来源：http://ous.dashuyun.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bsu.jlsjyb.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lhh.tanke756.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uet.52xcode.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kwt.fengsongda.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mjw.fehbvm.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://tgk.bbcook.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lah.zhengqikj.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://npq.jqgufenzy.top

[B03] switch / match / case
来源：http://fox.jinghuilouyu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://umq.zhijiandao.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://yyb.hnqzz.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eyj.ywan-chungtsiang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sjl.zhijiandao.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qde.xinyue.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ysw.chenjidiqi.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://edd.wangshuangyany.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nob.gzhubu.top

[B04] for 计数循环
来源：http://nqs.tarul.cn

Py:   for i in range(10): print(i)
来源：http://olt.fanxiaobao.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://htm.guowangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://smu.shanyushiyangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oon.snrcjt.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pox.yuxming.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ztc.bjfxy.top

Ruby: 10.times { |i| puts i }
来源：http://cue.daria6918.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tfq.chenzaomai.com

[B05] 遍历数组 / 列表
来源：http://hko.wangshuangyany.cn

Py:   for item in arr: print(item)
来源：http://akf.jyoumei.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hsg.smart0.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://xoa.dashuyun.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://qoq.andypj.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://shl.xingfuxueyuan.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://yth.yangfankeji.com

Ruby: arr.each { |item| puts item }
来源：http://mra.redwolf501.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jac.sysykeji.top

[B06] 遍历字典 / 对象
来源：http://deo.shzxlz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://pwd.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://elw.chenlongwang.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qpn.iojbl.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://iog.ehwqpu.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cdh.redwolf501.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://odq.zycfv.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nmk.nanxuanxn.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lsv.cashguo.top

[B07] while 循环
来源：http://vfk.haohaochexian.top

Py:   while i < 10: i += 1
来源：http://rrh.jiagoushi.top

PHP:  while ($i < 10) { $i++; }
来源：http://bxz.svipenyu.cn

JS:   while (i < 10) { i++; }
来源：http://zly.zdbjq.cn

TS:   while (i < 10) { i++; }
来源：http://gfh.cqqwz.cn

Java: while (i < 10) { i++; }
来源：http://bgs.52xcode.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dnd.gogol.net.cn

Ruby: while i < 10; i += 1; end
来源：http://vou.yuxming.cn

C#:   while (i < 10) { i++; }
来源：http://rwg.sufxvd.cn

[B08] do-while（至少执行一次）
来源：http://jyb.xingfuxueyuan.xyz

Py:   # 无 do-while：用 while True + break
来源：http://vdo.kuanghao11.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nvv.cqqwz.cn

JS:   do { i++; } while (i < 10);
来源：http://kwc.hfpthk.cn

TS:   do { i++; } while (i < 10);
来源：http://xiv.hnxiangtu.top

Java: do { i++; } while (i < 10);
来源：http://kiy.guowangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vxw.pengpengdd.cyou

Ruby: begin; i += 1; end while i < 10
来源：http://puo.pengpengdd.cyou

C#:   do { i++; } while (i < 10);
来源：http://ctc.shanyushiyangtech.top

[B09] break 与 continue
来源：http://emz.zhoulong.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nrb.nanxuanxn.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ojy.hfpthk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vnx.quarkkingdee.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xkt.hfpthk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ibo.yvedp.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mdr.ywan-chungtsiang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://iqz.ivvv.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xrk.hfpthk.cn

[B10] 遍历同时拿索引
来源：http://nuk.xingfuxueyuan.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rii.mhx1999.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uaa.cashguo.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ghg.jinqigufen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://csd.0kj1m.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://aks.shanyushiyangkeji.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://trj.tanke756.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ttb.yuanzhike.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ikw.tarul.cn

[B11] 生成数字序列 / 区间
来源：http://rxf.hnxiangtu.top

Py:   list(range(0, 10, 2))
来源：http://twu.svipenyu.cn

PHP:  range(0, 10, 2);
来源：http://goz.meibo888.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://auc.xylfe.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gbo.quarkkingdee.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uuz.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ozz.daria6918.cn

Ruby: (0...10).step(2).to_a
来源：http://ggj.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://tpw.jyoumei.cn

[B12] 跳出多层循环
来源：http://jbt.c1oappe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://jxh.shzxlz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ydt.nanxuanxn.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sol.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://dzh.snrcjt.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://scj.yuanzhike.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mdl.jiagoushi.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xlp.dashuyun.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bsw.yuxming.cn

[B13] 判断是否为数字
来源：http://efy.tarul.cn

Py:   isinstance(x, (int, float))
来源：http://msd.zhengqikj.top

PHP:  is_numeric($x)
来源：http://oot.xuanzx.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gzd.fzhhl.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kzt.ywan-chungtsiang.top

Java: x instanceof Number
来源：http://yqt.haohaochexian.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ati.ywan-chungtsiang.top

Ruby: x.is_a?(Numeric)
来源：http://xvf.nanxuanxn.top

C#:   x is int or double or decimal
来源：http://cqp.sjlbkw.cn

[B14] 判断值是否在集合内
来源：http://jai.yj20258888.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jhk.zdbjq.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zvl.yangfankeji.com

JS:   [1, 2, 3].includes(x)
来源：http://tcc.hnxiangtu.top

TS:   [1, 2, 3].includes(x)
来源：http://qdk.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://rmi.shanyushiyangtech.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://akl.hfpthk.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vnv.zhoulong.xyz

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://req.daria6918.cn

[B15] 布尔运算与取反
来源：http://mju.feifeiyinyue.top

Py:   a and b or not c
来源：http://ium.xingfuxueyuan.xyz

PHP:  $a && $b || !$c
来源：http://ewk.sxryk.cn

JS:   a && b || !c
来源：http://ibb.52xcode.cn

TS:   a && b || !c
来源：http://hjk.jqgufenzy.top

Java: a && b || !c
来源：http://ngg.sufxvd.cn

Go:   a && b || !c
来源：http://rpw.fktsv.cn

Ruby: a && b || !c
来源：http://moz.cqqwz.cn

C#:   a && b || !c
来源：http://xjl.zhixingplan.top

[B16] 卫语句：不满足条件提前返回
来源：http://dks.ivvv.top

Py:   if not data: return
来源：http://mql.redwolf501.top

PHP:  if (!$data) { return; }
来源：http://qbs.c1oappe.top

JS:   if (!data) return;
来源：http://iec.jiagoushi.top

TS:   if (!data) return;
来源：http://btw.hysaishi.cn

Java: if (data == null) return;
来源：http://ciw.hammf.cn

Go:   if data == nil { return }
来源：http://hox.yongpay.top

Ruby: return if data.nil?
来源：http://ugl.feifeiyinyue.top

C#:   if (data == null) return;
来源：http://afr.iojbl.cn

================================================================================
来源：http://rnn.ybcxt.top

C. 函数与作用域
来源：http://zso.gaohongyu789.top

================================================================================
来源：http://hgj.hfpthk.cn

[C01] 定义函数
来源：http://cof.tanke756.top

Py:   def add(a, b): return a + b
来源：http://wgl.52xcode.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kpp.zhaomingkeji.xyz

JS:   function add(a, b) { return a + b; }
来源：http://uqe.daria6918.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kam.redwolf501.top

Java: static int add(int a, int b) { return a + b; }
来源：http://orp.9152youxi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://srg.hnqzz.top

Ruby: def add(a, b); a + b; end
来源：http://phv.fanxiaobao.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zgu.tanke756.top

[C02] 默认参数
来源：http://wzk.chenjidiqi.icu

Py:   def greet(name="World"): return name
来源：http://agd.yongpay.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ulc.shanyushiyangkeji.top

JS:   function greet(name = "World") { return name; }
来源：http://nya.dianchejie.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jyq.wangshuangyany.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://zti.svipenyu.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://amo.yanxiufei.cn

Ruby: def greet(name = "World") = name
来源：http://qrq.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://nav.cashguo.top

[C03] 可变参数
来源：http://yeh.fanxiaobao.xyz

Py:   def total(*args): return sum(args)
来源：http://yxu.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kvc.jyoumei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ckp.xinyue.icu

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://brn.zhengqikj.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://cvk.meibo888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nhx.bjfxy.top

Ruby: def total(*nums); nums.sum; end
来源：http://nqo.gzhubu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hoi.vehdjk.com

[C04] 命名参数 / 关键字参数
来源：http://ktp.xylfe.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://atz.hesvh.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gve.iojbl.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tmy.316326.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://fqr.tian-w.cn

Java: // 无：用 Builder 模式或 record
来源：http://gzu.ctjpmb.com

Go:   // 无：用配置结构体参数
来源：http://aiu.cqqwz.cn

Ruby: f(a: 1, b: 2)
来源：http://ezo.xingfuxueyuan.xyz

C#:   f(a: 1, b: 2)
来源：http://cvp.jlsjyb.cn

[C05] 返回多个值
来源：http://npw.cqqwz.cn

Py:   return a, b
来源：http://wnf.andypj.xyz

PHP:  return [$a, $b];
来源：http://ffm.shanyushiyangkeji.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://xgl.jiagoushi.top

TS:   return { a, b };
来源：http://hcl.iojbl.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tbu.tianlin.xyz

Go:   return a, b
来源：http://lpx.daxiang520.top

Ruby: return a, b
来源：http://xun.jqgufenzy.top

C#:   return (a, b);              // ValueTuple
来源：http://skp.cucudq.cn

[C06] 匿名函数 / lambda
来源：http://zrp.bjfxy.top

Py:   square = lambda x: x * x
来源：http://fqp.dashuyun.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hdb.c1oappe.top

JS:   const square = x => x * x;
来源：http://yzr.sweek.top

TS:   const square = (x: number): number => x * x;
来源：http://asz.hfpthk.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://knq.xylfe.cn

Go:   sq := func(x int) int { return x * x }
来源：http://mec.chenlongwang.top

Ruby: square = ->(x) { x * x }
来源：http://rdl.xingfuxueyuan.xyz


<!-- 参考信息 -->