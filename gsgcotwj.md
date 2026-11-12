代发 wailian999

Ruby: value = data || "默认值"
来源：http://kdl.nanxuanxn.top

C#:   var value = data ?? "默认值";
来源：http://hgl.zhoulong.xyz

[A16] 真假值判断规则
来源：http://zbs.daxiang520.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://xxq.guowangkeji.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://lla.jlsjyb.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uib.fengsongda.top

TS:   if (!x) {}
来源：http://nuz.hnxiangtu.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nbw.yvedp.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kjb.gogol.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://uqr.jinqigfzy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yry.9152youxi.cn

[A17] 位运算
来源：http://jwz.gzhubu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nso.sxryk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bkj.hongshengwenyu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qtc.hongshengwenyu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uak.bbcook.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vfo.cqqwz.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dcz.jyoumei.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qcl.jinqigfzy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jls.hywenlv.cn

[A18] 字符与 ASCII 码互转
来源：http://spl.shangyingyoupin.top

Py:   ord("A"); chr(65)
来源：http://hya.mhx1999.top

PHP:  ord("A"); chr(65)
来源：http://jqe.fzhhl.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ypk.yueranfly.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sci.ydjk.org.cn

Java: (int) 'A'; (char) 65
来源：http://qqx.epnwcf.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gfh.yanxiufei.cn

Ruby: "A".ord; 65.chr
来源：http://nfx.smart0.xyz

C#:   (int)'A'; (char)65
来源：http://qfq.jiagoushi.top

[A19] 交换两个变量
来源：http://cng.sysykeji.top

Py:   a, b = b, a
来源：http://iwm.zdbjq.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://nch.wangshuangyany.cn

JS:   [a, b] = [b, a];
来源：http://wwv.bbcook.cn

TS:   [a, b] = [b, a];
来源：http://wfm.jyoumei.cn

Java: int t = a; a = b; b = t;
来源：http://nfm.pycfn.com

Go:   a, b = b, a
来源：http://sxa.ivvv.top

Ruby: a, b = b, a
来源：http://krv.sufxvd.cn

C#:   (a, b) = (b, a);
来源：http://ipj.hnxiangtu.top

[A20] 读取标准输入
来源：http://wvf.hongshengwenyu.top

Py:   name = input("请输入：")
来源：http://tzc.316326.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://roy.9152youxi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ldn.316326.xyz

TS:   // Node.js：readline 模块
来源：http://eyz.zhijiandao.cn

Java: new Scanner(System.in).nextLine()
来源：http://dqj.tanke756.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lgy.hysaishi.cn

Ruby: gets.chomp
来源：http://riq.zhixingplan.top

C#:   Console.ReadLine();
来源：http://aau.hnqzz.top

[A21] 保留指定小数位输出
来源：http://ayx.chenzaomai.com

Py:   f"{3.14159:.2f}"
来源：http://plh.jianghu66.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ito.hcnkem.com

JS:   (3.14159).toFixed(2)
来源：http://gbi.yangfankeji.com

TS:   (3.14159).toFixed(2)
来源：http://wcq.vehdjk.com

Java: String.format("%.2f", 3.14159)
来源：http://cak.guannengcc.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kop.guowangkeji.top

Ruby: format("%.2f", 3.14159)
来源：http://ugb.jqgufenzy.top

C#:   3.14159.ToString("F2")
来源：http://oyn.cucudq.cn

[A22] 获取字符串长度
来源：http://juk.c1oappe.top

Py:   len(s)
来源：http://quk.zhaomingkeji.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tyn.yfazqb.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://dxy.gzhubu.top

TS:   s.length
来源：http://pra.yj202588.top

Java: s.length()
来源：http://swl.hfpthk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://edt.iojbl.cn

Ruby: s.length
来源：http://cms.jlsjyb.cn

C#:   s.Length
来源：http://ped.ywan-chungtsiang.top

[A23] 大小写转换
来源：http://lne.ppjwa.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hna.fktsv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zfo.jqgufenzy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://onl.52xcode.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://eod.haohaochexian.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qli.nanxinkj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vox.xuanzx.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sqc.zhongyouzk.top

C#:   s.ToUpper(); s.ToLower()
来源：http://iyu.shzxlz.cn

[A24] 去除首尾空白
来源：http://aco.gogol.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nvv.birdmap.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fkg.tian-w.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ocg.tarul.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://duy.meibo888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://thj.hcnkem.com

Go:   strings.TrimSpace(s)
来源：http://zhu.yuanzhike.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cel.ydjk.org.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qst.hnxiangtu.top

[A25] 字符串比较
来源：http://yte.hysaishi.cn

Py:   s1 == s2; s1 != s2
来源：http://jct.hywenlv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pdd.ydzc1.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://jeq.zhoulong.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yhm.fktsv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://typ.fehbvm.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://nhl.vehdjk.com

Ruby: s1 == s2; s1 <=> s2
来源：http://byy.shanyushiyangtech.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://iam.jyoumei.cn

[A26] 类型转换总览
来源：http://rpv.xingfuxueyuan.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://uhu.jianghu66.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://eaw.cdnleiting.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://dii.yuxming.cn

TS:   Number() String() Boolean() x as number
来源：http://yyx.fengsongda.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pcx.fzhhl.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://byi.yuanzhike.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://djn.jiagoushi.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cvm.cdnleiting.top

================================================================================
来源：http://kho.shuidangran.top

B. 流程控制
来源：http://yzf.jlsjyb.cn

================================================================================
来源：http://uec.yj202588.top

[B01] 条件判断 if / else
来源：http://gbb.zycfv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://cnz.redwolf501.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fkb.jqgufenzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zju.fanxiaobao.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ejp.ydzc1.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://lgp.tian-w.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wzo.hysaishi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zso.meibo888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ipt.zhengqikj.top

[B02] 多分支 else if / elif
来源：http://mzo.sysykeji.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vfl.aizwys.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://loo.fehbvm.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hws.hongshengwenyu.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iyu.hysaishi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mka.wangdashe.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jjw.yuxming.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oxi.smart0.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ubh.gogol.net.cn

[B03] switch / match / case
来源：http://odl.gzhubu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xib.jinqigufen.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://wml.redwolf501.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ebh.yuanzhike.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ehd.jqgufenzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xvc.yj20258.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qsu.jinqigfzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hjh.yongpay.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ecf.hnxiangtu.top

[B04] for 计数循环
来源：http://rvf.xinyue.icu

Py:   for i in range(10): print(i)
来源：http://pix.xylfe.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rfu.yanxiufei.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hxi.wangdashe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bvl.yuxming.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dji.chenzaomai.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hko.fengsongda.top

Ruby: 10.times { |i| puts i }
来源：http://mvv.chenlongwang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hgr.jinqigfzy.top

[B05] 遍历数组 / 列表
来源：http://slb.daxiang520.top

Py:   for item in arr: print(item)
来源：http://une.fktsv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://aut.daxiang520.top

JS:   for (const item of arr) { console.log(item); }
来源：http://mjh.feifeiyinyue.top

TS:   for (const item of arr) { console.log(item); }
来源：http://cxe.yuxming.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://vsr.pycfn.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pnh.ppjwa.cn

Ruby: arr.each { |item| puts item }
来源：http://lfh.ehwqpu.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://rwj.shzxlz.cn

[B06] 遍历字典 / 对象
来源：http://xwd.vehdjk.com

Py:   for k, v in d.items(): print(k, v)
来源：http://fxl.tianlin.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ljw.hysaishi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gem.chenzaomai.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mhl.shanyushiyangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hkt.52xcode.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wyd.hnqzz.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://sbk.shanyushiyangtech.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kqb.pengpengdd.cyou

[B07] while 循环
来源：http://zmg.tanke756.top

Py:   while i < 10: i += 1
来源：http://hwk.redwolf501.top

PHP:  while ($i < 10) { $i++; }
来源：http://ypa.hongshengwenyu.top

JS:   while (i < 10) { i++; }
来源：http://mlh.hcnkem.com

TS:   while (i < 10) { i++; }
来源：http://tdr.chenjidiqi.icu

Java: while (i < 10) { i++; }
来源：http://wkl.sweek.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nuf.ywan-chungtsiang.top

Ruby: while i < 10; i += 1; end
来源：http://dca.dianchejie.cn

C#:   while (i < 10) { i++; }
来源：http://yug.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://urh.epnwcf.com

Py:   # 无 do-while：用 while True + break
来源：http://smy.pengpengdd.cyou

PHP:  do { $i++; } while ($i < 10);
来源：http://uuk.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://ipi.cqqwz.cn

TS:   do { i++; } while (i < 10);
来源：http://jqi.mhx1999.top

Java: do { i++; } while (i < 10);
来源：http://uuf.shanyushiyangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hlz.zhijiandao.cn

Ruby: begin; i += 1; end while i < 10
来源：http://bos.zhongyouzk.top

C#:   do { i++; } while (i < 10);
来源：http://plv.cdnleiting.top

[B09] break 与 continue
来源：http://xkr.pengpengdd.cyou

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zoe.shanyushiyangtech.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fpo.hongshengwenyu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ott.fanxiaobao.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aah.zhengqikj.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://llh.hnxiangtu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://gdi.hesvh.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://euh.yuxming.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://osr.yonumen.top

[B10] 遍历同时拿索引
来源：http://alv.hnxiangtu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vwe.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tbz.zhengqikj.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://amz.ywan-chungtsiang.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ttn.hcnkem.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://uqc.hnxiangtu.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rsc.ehwqpu.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://clr.guannengcc.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jmy.zhaomingkeji.xyz

[B11] 生成数字序列 / 区间
来源：http://plh.yueranfly.top

Py:   list(range(0, 10, 2))
来源：http://cgz.ctjpmb.com

PHP:  range(0, 10, 2);
来源：http://dhw.cashguo.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://joi.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jln.hywenlv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://okq.hnqzz.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ufx.shanyushiyangkeji.top

Ruby: (0...10).step(2).to_a
来源：http://vuc.jinqigufen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pfy.tarul.cn

[B12] 跳出多层循环
来源：http://ffo.pycfn.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://dnb.iojbl.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xft.nwbrower.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jum.smart0.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xha.hongshengwenyu.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://fts.sufxvd.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bnk.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zgl.fehbvm.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ijk.xziqi.cn

[B13] 判断是否为数字
来源：http://tto.svipenyu.cn

Py:   isinstance(x, (int, float))
来源：http://kyo.dashuyun.cn

PHP:  is_numeric($x)
来源：http://liv.gaohongyu789.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qyb.yuxming.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://djt.hnxiangtu.top

Java: x instanceof Number
来源：http://nlc.ehwqpu.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jjz.wangshuangyany.cn

Ruby: x.is_a?(Numeric)
来源：http://zjw.hfpthk.cn

C#:   x is int or double or decimal
来源：http://ars.mhx1999.top

[B14] 判断值是否在集合内
来源：http://vpo.hammf.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qnc.yj20258.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vzi.xuanzx.com

JS:   [1, 2, 3].includes(x)
来源：http://uhi.jqgfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://eop.bbcook.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ufh.pengpengdd.cyou

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://brz.zdbjq.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ucg.wangdashe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nrc.xinyue.icu

[B15] 布尔运算与取反
来源：http://yis.zhongyouzk.top

Py:   a and b or not c
来源：http://uqg.sysykeji.top

PHP:  $a && $b || !$c
来源：http://cfu.quarkkingdee.top

JS:   a && b || !c
来源：http://juz.guowangkeji.top

TS:   a && b || !c
来源：http://lej.0kj1m.cn

Java: a && b || !c
来源：http://yoo.sufxvd.cn

Go:   a && b || !c
来源：http://lrd.zdqjudy.top

Ruby: a && b || !c
来源：http://pxm.bjfxy.top

C#:   a && b || !c
来源：http://rww.wangshuangyany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://oiu.ppjwa.cn

Py:   if not data: return
来源：http://mus.ybcxt.top

PHP:  if (!$data) { return; }
来源：http://fim.jiagoushi.top

JS:   if (!data) return;
来源：http://wrx.dashuyun.cn

TS:   if (!data) return;
来源：http://yvj.smart0.xyz

Java: if (data == null) return;
来源：http://viz.zdbjq.cn

Go:   if data == nil { return }
来源：http://icf.kuanghao11.cn

Ruby: return if data.nil?
来源：http://wif.shanyushiyangkeji.top

C#:   if (data == null) return;
来源：http://fvq.gaohongyu789.top

================================================================================
来源：http://nfo.xinyue.icu

C. 函数与作用域
来源：http://zlg.xuetiantiany.cn

================================================================================
来源：http://gra.sufxvd.cn

[C01] 定义函数
来源：http://xoz.zhijiandao.cn

Py:   def add(a, b): return a + b
来源：http://ozy.jyoumei.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hqo.wangdashe.top

JS:   function add(a, b) { return a + b; }
来源：http://zpo.hcnkem.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wmm.ivvv.top

Java: static int add(int a, int b) { return a + b; }
来源：http://wct.haohaochexian.top

Go:   func add(a, b int) int { return a + b }
来源：http://hqf.yongpay.top

Ruby: def add(a, b); a + b; end
来源：http://lnu.quarkkingdee.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nay.aizwys.cn

[C02] 默认参数
来源：http://mga.meibo888.top

Py:   def greet(name="World"): return name
来源：http://pai.yueranfly.top

PHP:  function greet($name = "World") { return $name; }
来源：http://rnq.zhixingplan.top

JS:   function greet(name = "World") { return name; }
来源：http://oqf.jqgfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wne.jinghuilouyu.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ljl.hywenlv.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://err.xziqi.cn

Ruby: def greet(name = "World") = name
来源：http://yka.ppjwa.cn

C#:   string Greet(string name = "World") => name;
来源：http://nff.0kj1m.cn

[C03] 可变参数
来源：http://tdb.yanxiufei.cn

Py:   def total(*args): return sum(args)
来源：http://vqj.cqqwz.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hjj.hfpthk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vrt.yueranfly.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dva.chenjidiqi.icu

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dwo.tarul.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://nrh.fehbvm.com

Ruby: def total(*nums); nums.sum; end
来源：http://ktx.hysaishi.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qye.ybcxt.top

[C04] 命名参数 / 关键字参数
来源：http://qrc.jiagoushi.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tzi.ivvv.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://npt.smart0.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ffg.dashuyun.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://pne.yfazqb.com

Java: // 无：用 Builder 模式或 record
来源：http://mrp.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://ddd.hnqzz.top

Ruby: f(a: 1, b: 2)
来源：http://cwv.yuxming.cn

C#:   f(a: 1, b: 2)
来源：http://jzs.zhijiandao.cn

[C05] 返回多个值
来源：http://ezt.yj20258.top

Py:   return a, b
来源：http://zpx.nwbrower.top

PHP:  return [$a, $b];
来源：http://qsz.nanxinkj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://pmo.yj20258888.top

TS:   return { a, b };
来源：http://yql.zhiwuduotai.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://qat.havefunace.top

Go:   return a, b
来源：http://kib.jiagoushi.top

Ruby: return a, b
来源：http://qrn.jqgufenzy.top

C#:   return (a, b);              // ValueTuple
来源：http://vjf.hnxiangtu.top

[C06] 匿名函数 / lambda
来源：http://mwh.xuanzx.com

Py:   square = lambda x: x * x
来源：http://pjp.cucudq.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://dsl.shangyingyoupin.top

JS:   const square = x => x * x;
来源：http://hqi.chenjidiqi.icu


<!-- 参考信息 -->