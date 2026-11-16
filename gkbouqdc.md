代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://uqn.tian-w.cn

[A15] 空值判断与默认值
来源：http://hph.hfpthk.cn

Py:   value = data or "默认值"
来源：http://hfp.chenzaomai.com

PHP:  $value = $data ?? "默认值";
来源：http://eni.jqgufenzy.top

JS:   const value = data ?? "默认值";
来源：http://egr.fanxiaobao.xyz

TS:   const value = data ?? "默认值";
来源：http://fyq.gaohongyu789.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xzh.ivvv.top

Go:   if data == "" { data = "默认值" }
来源：http://wpp.uphjek.com

Ruby: value = data || "默认值"
来源：http://exf.316326.xyz

C#:   var value = data ?? "默认值";
来源：http://ser.tianlin.xyz

[A16] 真假值判断规则
来源：http://qsr.jyoumei.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://nyi.xuanzx.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://jkc.fengsongda.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uqq.cdnleiting.top

TS:   if (!x) {}
来源：http://yvu.yuxming.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dpf.vqdsnc.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://neg.yvedp.cn

Ruby: unless x            # nil 与 false 为假
来源：http://anh.gzhubu.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://iqa.yongpay.top

[A17] 位运算
来源：http://hyw.zhoulong.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fza.zhongyouzk.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://drw.meibo888.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qhx.quarkkingdee.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kce.bbcook.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rok.sufxvd.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cnn.shanyushiyangkeji.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://prf.quarkkingdee.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jxs.yangfankeji.com

[A18] 字符与 ASCII 码互转
来源：http://ytl.uphjek.com

Py:   ord("A"); chr(65)
来源：http://xub.ybcxt.top

PHP:  ord("A"); chr(65)
来源：http://usb.tanke756.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hap.xylfe.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://njm.zhijiandao.cn

Java: (int) 'A'; (char) 65
来源：http://xhp.yj202588.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lqw.bbcook.cn

Ruby: "A".ord; 65.chr
来源：http://rbr.cqqwz.cn

C#:   (int)'A'; (char)65
来源：http://vto.hywenlv.cn

[A19] 交换两个变量
来源：http://fli.meibo888.top

Py:   a, b = b, a
来源：http://sbt.daxiang520.top

PHP:  [$a, $b] = [$b, $a];
来源：http://kpw.zhaomingkeji.xyz

JS:   [a, b] = [b, a];
来源：http://ggh.sufxvd.cn

TS:   [a, b] = [b, a];
来源：http://brw.iojbl.cn

Java: int t = a; a = b; b = t;
来源：http://yhh.tarul.cn

Go:   a, b = b, a
来源：http://agf.dianchejie.cn

Ruby: a, b = b, a
来源：http://znz.hnxiangtu.top

C#:   (a, b) = (b, a);
来源：http://gir.yfazqb.com

[A20] 读取标准输入
来源：http://kru.cdnleiting.top

Py:   name = input("请输入：")
来源：http://frq.zdbjq.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://npb.zhiwuduotai.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wkt.dashuyun.cn

TS:   // Node.js：readline 模块
来源：http://yno.hfpthk.cn

Java: new Scanner(System.in).nextLine()
来源：http://obx.jyoumei.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kto.andypj.xyz

Ruby: gets.chomp
来源：http://jln.aibaodan.cn

C#:   Console.ReadLine();
来源：http://unq.dashuyun.cn

[A21] 保留指定小数位输出
来源：http://kzw.yueranfly.top

Py:   f"{3.14159:.2f}"
来源：http://ekq.hcnkem.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rxz.jyoumei.cn

JS:   (3.14159).toFixed(2)
来源：http://coc.cashguo.top

TS:   (3.14159).toFixed(2)
来源：http://qnx.haohaochexian.top

Java: String.format("%.2f", 3.14159)
来源：http://ten.zhiwuduotai.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://qzh.jinghuilouyu.cn

Ruby: format("%.2f", 3.14159)
来源：http://ccl.quarkkingdee.top

C#:   3.14159.ToString("F2")
来源：http://vel.yfazqb.com

[A22] 获取字符串长度
来源：http://kec.hfpthk.cn

Py:   len(s)
来源：http://cxa.shanyushiyangkeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qtq.smart0.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fsc.vehdjk.com

TS:   s.length
来源：http://ofn.jiagoushi.top

Java: s.length()
来源：http://feb.ctjpmb.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wsd.shzxlz.cn

Ruby: s.length
来源：http://jwk.gaohongyu789.top

C#:   s.Length
来源：http://qam.9152youxi.cn

[A23] 大小写转换
来源：http://shx.jiagoushi.top

Py:   s.upper(); s.lower(); s.title()
来源：http://jsz.feifeiyinyue.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://upo.sjlbkw.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://tzy.zhijiandao.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://grw.gaohongyu789.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fsj.bjfxy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://eyq.smart0.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mko.pycfn.com

C#:   s.ToUpper(); s.ToLower()
来源：http://szo.ydzc1.top

[A24] 去除首尾空白
来源：http://adu.sxryk.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ggt.yueranfly.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://his.kuanghao11.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jyz.ctjpmb.com

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wpl.xuanzx.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ojv.zhixingplan.top

Go:   strings.TrimSpace(s)
来源：http://bhh.fanxiaobao.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uca.yangfankeji.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ten.fzhhl.top

[A25] 字符串比较
来源：http://ukv.dashuyun.cn

Py:   s1 == s2; s1 != s2
来源：http://wjq.yj20258.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://uxb.yj202588.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://isj.zhongyouzk.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ulg.tarul.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kza.cheryme.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gjj.gzhubu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://lrl.havefunace.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://aet.jinqigufen.top

[A26] 类型转换总览
来源：http://brq.yangfankeji.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://huo.fengsongda.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://sos.shanyushiyangtech.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ems.quarkkingdee.top

TS:   Number() String() Boolean() x as number
来源：http://sfl.wangdashe.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lhz.jqgufenzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://knv.yuanzhike.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://khe.nwbrower.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xmk.haohaochexian.top

================================================================================
来源：http://npw.jinqigufen.top

B. 流程控制
来源：http://udb.dianchejie.cn

================================================================================
来源：http://ezi.iojbl.cn

[B01] 条件判断 if / else
来源：http://tcj.hongshengwenyu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://jwl.shanyushiyangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tlx.shangyingyoupin.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kgg.fzhhl.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://akw.shanyushiyangtech.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://een.yonumen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ecv.xinyue.icu

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ycc.hongshengwenyu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cfl.ywan-chungtsiang.top

[B02] 多分支 else if / elif
来源：http://epv.hcnkem.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fac.yj202588.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kpn.shangyingyoupin.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pea.jiagoushi.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dts.yvedp.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eur.mhx1999.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fog.yj202588.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://txd.yanxiufei.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ifs.yuanzhike.top

[B03] switch / match / case
来源：http://qnt.yanxiufei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ieu.chenjidiqi.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://gjz.epnwcf.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lzt.xziqi.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yxo.hesvh.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://cew.feifeiyinyue.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kza.tarul.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ipi.yj202588.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wvc.chenjidiqi.icu

[B04] for 计数循环
来源：http://nfb.tian-w.cn

Py:   for i in range(10): print(i)
来源：http://ouv.nanxuanxn.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://urf.yueranfly.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://szt.jinghuilouyu.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bre.zhiwuduotai.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ppv.cqqwz.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://whe.52xcode.cn

Ruby: 10.times { |i| puts i }
来源：http://jfh.tianlin.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cum.fktsv.cn

[B05] 遍历数组 / 列表
来源：http://opr.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://wnx.tarul.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jjp.tarul.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wva.fzhhl.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ndk.yuxming.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://czi.jinqigufen.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://cwe.zdqjudy.top

Ruby: arr.each { |item| puts item }
来源：http://hvh.zhongyouzk.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dnq.sjlbkw.cn

[B06] 遍历字典 / 对象
来源：http://bvy.yvedp.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://jny.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hcc.ivvv.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://sgv.sjlbkw.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://abd.yueranfly.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://znr.cucudq.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://aqs.jiagoushi.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ves.xuanzx.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nzu.52xcode.cn

[B07] while 循环
来源：http://tai.tarul.cn

Py:   while i < 10: i += 1
来源：http://klv.xingfuxueyuan.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://rcr.quarkkingdee.top

JS:   while (i < 10) { i++; }
来源：http://ioj.gaohongyu789.top

TS:   while (i < 10) { i++; }
来源：http://vqu.gogol.net.cn

Java: while (i < 10) { i++; }
来源：http://jaz.fanxiaobao.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://djt.hongshengwenyu.top

Ruby: while i < 10; i += 1; end
来源：http://vfe.jiagoushi.top

C#:   while (i < 10) { i++; }
来源：http://eia.zhoulong.xyz

[B08] do-while（至少执行一次）
来源：http://ipf.dianchejie.cn

Py:   # 无 do-while：用 while True + break
来源：http://udw.shzxlz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://nmg.snrcjt.cn

JS:   do { i++; } while (i < 10);
来源：http://mzt.zhijiandao.cn

TS:   do { i++; } while (i < 10);
来源：http://lkk.jiagoushi.top

Java: do { i++; } while (i < 10);
来源：http://gss.nanxinkj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://npd.316326.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://euk.gzhubu.top

C#:   do { i++; } while (i < 10);
来源：http://sxw.chenlongwang.top

[B09] break 与 continue
来源：http://ppl.chenlongwang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zea.yfazqb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pis.ctjpmb.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jxm.chenjidiqi.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ehj.redwolf501.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ntk.gaohongyu789.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qcs.uphjek.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rkh.vqdsnc.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://thx.hongshengwenyu.top

[B10] 遍历同时拿索引
来源：http://yxc.jinyuanbaomall.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://joy.yvedp.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://swr.9152youxi.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://oyq.ehwqpu.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://han.yj20258.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hpx.zhaomingkeji.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://peo.haohaochexian.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fmj.zdqjudy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qqy.gotoacloud.top

[B11] 生成数字序列 / 区间
来源：http://hti.yuxming.cn

Py:   list(range(0, 10, 2))
来源：http://tay.tanke756.top

PHP:  range(0, 10, 2);
来源：http://qwv.ywan-chungtsiang.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://axs.ppjwa.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wxx.jyoumei.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://olb.jqgfzy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://oei.wangdashe.top

Ruby: (0...10).step(2).to_a
来源：http://lex.zhongyouzk.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pzt.zdqjudy.top

[B12] 跳出多层循环
来源：http://yfw.jiagoushi.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lmh.birdmap.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://giy.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mvx.xuetiantiany.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://nkv.yanxiufei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hhq.zhengqikj.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ixg.iojbl.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zve.feifeiyinyue.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dlw.zhengqikj.top

[B13] 判断是否为数字
来源：http://hth.cheryme.top

Py:   isinstance(x, (int, float))
来源：http://eyf.guowangkeji.top

PHP:  is_numeric($x)
来源：http://bew.nwbrower.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://myl.chenzaomai.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iii.cashguo.top

Java: x instanceof Number
来源：http://gnv.dianchejie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jjl.andypj.xyz

Ruby: x.is_a?(Numeric)
来源：http://emz.jqgfzy.top

C#:   x is int or double or decimal
来源：http://rms.yanxiufei.cn

[B14] 判断值是否在集合内
来源：http://qim.jinyuanbaomall.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mht.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vpz.cashguo.top

JS:   [1, 2, 3].includes(x)
来源：http://jmd.xinyue.icu

TS:   [1, 2, 3].includes(x)
来源：http://yqk.zycfv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://zgh.xinyue.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ufr.chenjidiqi.icu

Ruby: [1, 2, 3].include?(x)
来源：http://aui.gaohongyu789.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xnk.yj20258888.top

[B15] 布尔运算与取反
来源：http://pmy.daria6918.cn

Py:   a and b or not c
来源：http://jnz.jiagoushi.top

PHP:  $a && $b || !$c
来源：http://wob.cashguo.top

JS:   a && b || !c
来源：http://axh.ywan-chungtsiang.top

TS:   a && b || !c
来源：http://wxu.uphjek.com

Java: a && b || !c
来源：http://vmp.yueranfly.top

Go:   a && b || !c
来源：http://olr.c1oappe.top

Ruby: a && b || !c
来源：http://qls.bjfxy.top

C#:   a && b || !c
来源：http://dnl.316326.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://yhj.nanxinkj.top

Py:   if not data: return
来源：http://bnw.uphjek.com

PHP:  if (!$data) { return; }
来源：http://ymf.snrcjt.cn

JS:   if (!data) return;
来源：http://pzr.xziqi.cn

TS:   if (!data) return;
来源：http://uto.fzhhl.top

Java: if (data == null) return;
来源：http://lnl.redwolf501.top

Go:   if data == nil { return }
来源：http://brb.dianchejie.cn

Ruby: return if data.nil?
来源：http://dvv.nanxuanxn.top

C#:   if (data == null) return;
来源：http://qva.jyoumei.cn

================================================================================
来源：http://exu.jqgfzy.top

C. 函数与作用域
来源：http://bwp.hesvh.cn

================================================================================
来源：http://hcd.yonumen.top

[C01] 定义函数
来源：http://ofc.yongpay.top

Py:   def add(a, b): return a + b
来源：http://fxp.shangyingyoupin.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://aua.gotoacloud.top

JS:   function add(a, b) { return a + b; }
来源：http://hgu.yanxiufei.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://faz.ywan-chungtsiang.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nkz.9152youxi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://qmj.smart0.xyz

Ruby: def add(a, b); a + b; end
来源：http://ipr.316326.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://oqq.vehdjk.com

[C02] 默认参数
来源：http://tfg.birdmap.top

Py:   def greet(name="World"): return name
来源：http://sgs.jinyuanbaomall.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lvd.nanxuanxn.top

JS:   function greet(name = "World") { return name; }
来源：http://qrf.c1oappe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://upr.xuanzx.com

Java: // 无默认参数：方法重载或 Optional
来源：http://wkt.haohaochexian.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dct.tian-w.cn

Ruby: def greet(name = "World") = name
来源：http://qbp.meibo888.top

C#:   string Greet(string name = "World") => name;
来源：http://vuo.tianlin.xyz

[C03] 可变参数
来源：http://vec.hammf.cn

Py:   def total(*args): return sum(args)
来源：http://vbz.wangdashe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://get.cashguo.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ehe.xuanzx.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wce.gzhubu.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zxo.smart0.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://agk.zdqjudy.top

Ruby: def total(*nums); nums.sum; end
来源：http://bny.zhoulong.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tcn.chenlongwang.top

[C04] 命名参数 / 关键字参数
来源：http://vfb.daxiang520.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tjn.shuidangran.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xcd.zdbjq.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hsn.zdqjudy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sje.smart0.xyz

Java: // 无：用 Builder 模式或 record
来源：http://muv.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://bzh.cdnleiting.top

Ruby: f(a: 1, b: 2)
来源：http://ysm.316326.xyz

C#:   f(a: 1, b: 2)
来源：http://esh.pycfn.com

[C05] 返回多个值
来源：http://msn.vehdjk.com

Py:   return a, b
来源：http://ksq.hnxiangtu.top

PHP:  return [$a, $b];
来源：http://eod.zhixingplan.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://rov.bjfxy.top

TS:   return { a, b };
来源：http://gev.iojbl.cn


<!-- 参考信息 -->