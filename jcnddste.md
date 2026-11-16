代发 wailian999

Ruby: value = data || "默认值"
来源：http://lms.shzxlz.cn

C#:   var value = data ?? "默认值";
来源：http://fpx.aizwys.cn

[A16] 真假值判断规则
来源：http://qox.zhijiandao.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://iwr.daxiang520.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fjn.hysaishi.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://amh.zhijiandao.cn

TS:   if (!x) {}
来源：http://jrx.zhengqikj.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://inw.yj202588.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://gvh.bjfxy.top

Ruby: unless x            # nil 与 false 为假
来源：http://uso.hnqzz.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://jnn.zdqjudy.top

[A17] 位运算
来源：http://aaz.c1oappe.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cdz.zhengqikj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vwr.yvedp.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pau.zdbjq.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://spx.zhaomingkeji.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://phv.cdnleiting.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ezr.feifeiyinyue.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xtu.guowangkeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dpa.xinyue.icu

[A18] 字符与 ASCII 码互转
来源：http://ktf.dashuyun.cn

Py:   ord("A"); chr(65)
来源：http://nrs.ppjwa.cn

PHP:  ord("A"); chr(65)
来源：http://sgm.hysaishi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uqc.fzhhl.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xfp.hongshengwenyu.top

Java: (int) 'A'; (char) 65
来源：http://srb.cashguo.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ots.vqdsnc.cn

Ruby: "A".ord; 65.chr
来源：http://nxq.zhongyouzk.top

C#:   (int)'A'; (char)65
来源：http://ovj.yueranfly.top

[A19] 交换两个变量
来源：http://mib.zhaomingkeji.xyz

Py:   a, b = b, a
来源：http://qtg.cqqwz.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://civ.hnxiangtu.top

JS:   [a, b] = [b, a];
来源：http://qyg.yvedp.cn

TS:   [a, b] = [b, a];
来源：http://ofi.jinyuanbaomall.cn

Java: int t = a; a = b; b = t;
来源：http://pxf.ppjwa.cn

Go:   a, b = b, a
来源：http://zpa.zhengqikj.top

Ruby: a, b = b, a
来源：http://eai.0kj1m.cn

C#:   (a, b) = (b, a);
来源：http://yhu.yj20258888.top

[A20] 读取标准输入
来源：http://fnb.xingfuxueyuan.xyz

Py:   name = input("请输入：")
来源：http://szf.wangshuangyany.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hyj.uphjek.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wve.xylfe.cn

TS:   // Node.js：readline 模块
来源：http://vsp.hywenlv.cn

Java: new Scanner(System.in).nextLine()
来源：http://nzg.cucudq.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ush.ppjwa.cn

Ruby: gets.chomp
来源：http://all.ivvv.top

C#:   Console.ReadLine();
来源：http://xbc.pengpengdd.cyou

[A21] 保留指定小数位输出
来源：http://tln.chenlongwang.top

Py:   f"{3.14159:.2f}"
来源：http://ata.daria6918.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vxe.hywenlv.cn

JS:   (3.14159).toFixed(2)
来源：http://bfo.daria6918.cn

TS:   (3.14159).toFixed(2)
来源：http://prc.ctjpmb.com

Java: String.format("%.2f", 3.14159)
来源：http://vjw.jinqigufen.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://syb.nanxinkj.top

Ruby: format("%.2f", 3.14159)
来源：http://bde.ywan-chungtsiang.top

C#:   3.14159.ToString("F2")
来源：http://pjh.yuxming.cn

[A22] 获取字符串长度
来源：http://exu.9152youxi.cn

Py:   len(s)
来源：http://zkt.jqgufenzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mib.hongshengwenyu.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rzz.shanyushiyangtech.top

TS:   s.length
来源：http://zbf.ehwqpu.com

Java: s.length()
来源：http://jdg.pengpengdd.cyou

Go:   len(s); utf8.RuneCountInString(s)
来源：http://yps.fehbvm.com

Ruby: s.length
来源：http://evq.hcnkem.com

C#:   s.Length
来源：http://aio.hammf.cn

[A23] 大小写转换
来源：http://puv.chenlongwang.top

Py:   s.upper(); s.lower(); s.title()
来源：http://wtp.mhx1999.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://zby.chenlongwang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ywl.52xcode.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hsf.yueranfly.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://mzq.smart0.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://dok.ybcxt.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ups.guowangkeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://wtr.jyoumei.cn

[A24] 去除首尾空白
来源：http://esu.ctjpmb.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://odr.jinqigufen.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hbr.yvedp.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nsw.yvedp.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qfr.jinyuanbaomall.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://llc.gaohongyu789.top

Go:   strings.TrimSpace(s)
来源：http://ylt.zhiwuduotai.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://srz.zhongyouzk.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lse.uphjek.com

[A25] 字符串比较
来源：http://hyx.yuxming.cn

Py:   s1 == s2; s1 != s2
来源：http://jqo.yongpay.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hdy.guowangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qln.daria6918.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xpp.xuanzx.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pjl.zhixingplan.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qyc.guannengcc.top

Ruby: s1 == s2; s1 <=> s2
来源：http://aau.sufxvd.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://tvo.jqgufenzy.top

[A26] 类型转换总览
来源：http://ffr.xylfe.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zsr.shuidangran.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://noo.chenjidiqi.icu

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://fxg.xinyue.icu

TS:   Number() String() Boolean() x as number
来源：http://vaz.gzhubu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xeg.birdmap.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nhn.svipenyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://yiy.zhoulong.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pxf.zhixingplan.top

================================================================================
来源：http://zvk.jqgfzy.top

B. 流程控制
来源：http://hpy.smart0.xyz

================================================================================
来源：http://axq.shuidangran.top

[B01] 条件判断 if / else
来源：http://lgt.hnxiangtu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://oqg.epnwcf.com

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ctu.shuidangran.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jmp.dianchejie.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kec.dashuyun.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://yyw.ywan-chungtsiang.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jfq.fktsv.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dmw.sweek.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://scz.quarkkingdee.top

[B02] 多分支 else if / elif
来源：http://wcf.gogol.net.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fkb.tianlin.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nzj.gaohongyu789.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nnj.9152youxi.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mmk.yj20258.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wwp.gotoacloud.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hbl.aizwys.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ffd.xuanzx.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wbh.iojbl.cn

[B03] switch / match / case
来源：http://zwd.gogol.net.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kcz.nanxuanxn.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://vcw.kuanghao11.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rlr.0kj1m.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vzj.fehbvm.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kau.9152youxi.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dby.yonumen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://tes.dianchejie.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sqj.xylfe.cn

[B04] for 计数循环
来源：http://zec.nanxinkj.top

Py:   for i in range(10): print(i)
来源：http://tig.hcnkem.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nxl.iojbl.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lqn.gzhubu.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qki.andypj.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aix.epnwcf.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://azy.jinghuilouyu.cn

Ruby: 10.times { |i| puts i }
来源：http://ubt.gogol.net.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ayt.fehbvm.com

[B05] 遍历数组 / 列表
来源：http://wcw.gotoacloud.top

Py:   for item in arr: print(item)
来源：http://qvf.hcnkem.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://efg.ppjwa.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://uoi.0kj1m.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bpm.chenzaomai.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://map.cdnleiting.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://emf.shzxlz.cn

Ruby: arr.each { |item| puts item }
来源：http://mow.316326.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://prs.yvedp.cn

[B06] 遍历字典 / 对象
来源：http://hlx.9152youxi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ndk.fanxiaobao.xyz

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vls.hesvh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vig.0kj1m.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://txj.zdbjq.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://por.chenlongwang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://qrk.shanyushiyangkeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qra.hfpthk.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://kyz.zhiwuduotai.top

[B07] while 循环
来源：http://qdm.tanke756.top

Py:   while i < 10: i += 1
来源：http://gkb.nanxuanxn.top

PHP:  while ($i < 10) { $i++; }
来源：http://ybh.yonumen.top

JS:   while (i < 10) { i++; }
来源：http://fcv.zycfv.cn

TS:   while (i < 10) { i++; }
来源：http://wyp.jlsjyb.cn

Java: while (i < 10) { i++; }
来源：http://fyr.aibaodan.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qbt.birdmap.top

Ruby: while i < 10; i += 1; end
来源：http://pnq.sweek.top

C#:   while (i < 10) { i++; }
来源：http://dsb.ywan-chungtsiang.top

[B08] do-while（至少执行一次）
来源：http://eon.jianghu66.top

Py:   # 无 do-while：用 while True + break
来源：http://dpz.ydzc1.top

PHP:  do { $i++; } while ($i < 10);
来源：http://enn.jianghu66.top

JS:   do { i++; } while (i < 10);
来源：http://hth.shzxlz.cn

TS:   do { i++; } while (i < 10);
来源：http://rlv.hnxiangtu.top

Java: do { i++; } while (i < 10);
来源：http://tqb.svipenyu.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://frd.jinyuanbaomall.cn

Ruby: begin; i += 1; end while i < 10
来源：http://iks.guannengcc.top

C#:   do { i++; } while (i < 10);
来源：http://phs.gaohongyu789.top

[B09] break 与 continue
来源：http://evd.shangyingyoupin.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hei.kuanghao11.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://onb.ydzc1.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://suv.cqqwz.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xtp.yj202588.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aac.zhixingplan.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cei.chenlongwang.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://arv.shzxlz.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vti.52xcode.cn

[B10] 遍历同时拿索引
来源：http://suq.gaohongyu789.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://god.shzxlz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://avs.smart0.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hhx.bbcook.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://tkg.gotoacloud.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iyy.jqgufenzy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://uzf.zycfv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fti.hongshengwenyu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zsb.gaohongyu789.top

[B11] 生成数字序列 / 区间
来源：http://shs.pycfn.com

Py:   list(range(0, 10, 2))
来源：http://wcd.daxiang520.top

PHP:  range(0, 10, 2);
来源：http://zfe.316326.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://rsf.bjfxy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ygp.9152youxi.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lie.yvedp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zfx.bbcook.cn

Ruby: (0...10).step(2).to_a
来源：http://bhv.andypj.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://npg.havefunace.top

[B12] 跳出多层循环
来源：http://nmi.yangfankeji.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://uim.zycfv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://hjy.aibaodan.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vng.yangfankeji.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cjl.sjlbkw.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vpb.jlsjyb.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xyh.yuanzhike.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lyu.jlsjyb.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ccf.tian-w.cn

[B13] 判断是否为数字
来源：http://suk.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://abo.dashuyun.cn

PHP:  is_numeric($x)
来源：http://zrs.wangshuangyany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://skv.yueranfly.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kcz.zhaomingkeji.xyz

Java: x instanceof Number
来源：http://qxl.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vuu.hnqzz.top

Ruby: x.is_a?(Numeric)
来源：http://zjk.xingfuxueyuan.xyz

C#:   x is int or double or decimal
来源：http://fmp.zhaomingkeji.xyz

[B14] 判断值是否在集合内
来源：http://lfa.jqgfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wsm.52xcode.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rhs.yuxming.cn

JS:   [1, 2, 3].includes(x)
来源：http://kjl.yj20258888.top

TS:   [1, 2, 3].includes(x)
来源：http://jqu.vehdjk.com

Java: List.of(1, 2, 3).contains(x)
来源：http://dhw.epnwcf.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://are.iojbl.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pjr.jianghu66.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dgm.kuanghao11.cn

[B15] 布尔运算与取反
来源：http://pcj.zhijiandao.cn

Py:   a and b or not c
来源：http://hjj.yvedp.cn

PHP:  $a && $b || !$c
来源：http://nwc.jqgufenzy.top

JS:   a && b || !c
来源：http://kil.xylfe.cn

TS:   a && b || !c
来源：http://hvh.xziqi.cn

Java: a && b || !c
来源：http://tgd.hesvh.cn

Go:   a && b || !c
来源：http://nyz.aizwys.cn

Ruby: a && b || !c
来源：http://hsg.xingfuxueyuan.xyz

C#:   a && b || !c
来源：http://wyy.shanyushiyangtech.top

[B16] 卫语句：不满足条件提前返回
来源：http://wsw.yj202588.top

Py:   if not data: return
来源：http://dlz.ppjwa.cn

PHP:  if (!$data) { return; }
来源：http://uie.nanxinkj.top

JS:   if (!data) return;
来源：http://hsv.dashuyun.cn

TS:   if (!data) return;
来源：http://bok.jqgufenzy.top

Java: if (data == null) return;
来源：http://pyt.jqgufenzy.top

Go:   if data == nil { return }
来源：http://voa.zhoulong.xyz

Ruby: return if data.nil?
来源：http://jpn.guowangkeji.top

C#:   if (data == null) return;
来源：http://gbx.andypj.xyz

================================================================================
来源：http://ase.uphjek.com

C. 函数与作用域
来源：http://bht.shuidangran.top

================================================================================
来源：http://phn.tarul.cn

[C01] 定义函数
来源：http://gwh.fzhhl.top

Py:   def add(a, b): return a + b
来源：http://aiz.hnqzz.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sxs.yangfankeji.com

JS:   function add(a, b) { return a + b; }
来源：http://mit.bjfxy.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ysr.jyoumei.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cda.hnxiangtu.top

Go:   func add(a, b int) int { return a + b }
来源：http://mif.cashguo.top

Ruby: def add(a, b); a + b; end
来源：http://suv.ydzc1.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ehj.aizwys.cn

[C02] 默认参数
来源：http://paw.zhiwuduotai.top

Py:   def greet(name="World"): return name
来源：http://klc.xinyue.icu

PHP:  function greet($name = "World") { return $name; }
来源：http://gai.uphjek.com

JS:   function greet(name = "World") { return name; }
来源：http://mou.guannengcc.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ahe.andypj.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://lrk.shangyingyoupin.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vhx.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://vdn.guowangkeji.top

C#:   string Greet(string name = "World") => name;
来源：http://cgu.jiagoushi.top

[C03] 可变参数
来源：http://ynm.andypj.xyz

Py:   def total(*args): return sum(args)
来源：http://fcx.fktsv.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sft.yvedp.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lrf.fengsongda.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://yxd.xuetiantiany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fgr.tian-w.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://drm.shanyushiyangtech.top

Ruby: def total(*nums); nums.sum; end
来源：http://ucy.yvedp.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lln.hysaishi.cn

[C04] 命名参数 / 关键字参数
来源：http://szi.yvedp.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tkj.gaohongyu789.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vcu.dianchejie.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hgx.cheryme.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dbz.haohaochexian.top

Java: // 无：用 Builder 模式或 record
来源：http://fzv.ybcxt.top

Go:   // 无：用配置结构体参数
来源：http://jul.cucudq.cn

Ruby: f(a: 1, b: 2)
来源：http://mso.cdnleiting.top

C#:   f(a: 1, b: 2)
来源：http://tph.guannengcc.top

[C05] 返回多个值
来源：http://vra.hfpthk.cn

Py:   return a, b
来源：http://ckh.gotoacloud.top

PHP:  return [$a, $b];
来源：http://tlt.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bea.bbcook.cn

TS:   return { a, b };
来源：http://dnz.tian-w.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gii.dashuyun.cn

Go:   return a, b
来源：http://jqe.smart0.xyz

Ruby: return a, b
来源：http://qdo.bbcook.cn

C#:   return (a, b);              // ValueTuple
来源：http://wsl.shzxlz.cn

[C06] 匿名函数 / lambda
来源：http://hgk.9152youxi.cn

Py:   square = lambda x: x * x
来源：http://qza.andypj.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://lgt.fktsv.cn

JS:   const square = x => x * x;
来源：http://zpq.birdmap.top


<!-- 参考信息 -->