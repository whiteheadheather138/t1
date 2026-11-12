代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://bwz.tanke756.top

TS:   const value = data ?? "默认值";
来源：http://lcw.nanxinkj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://vgu.jqgufenzy.top

Go:   if data == "" { data = "默认值" }
来源：http://gym.xuanzx.com

Ruby: value = data || "默认值"
来源：http://xog.daxiang520.top

C#:   var value = data ?? "默认值";
来源：http://tiy.fehbvm.com

[A16] 真假值判断规则
来源：http://bvk.haohaochexian.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://pkw.jqgfzy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://dui.yj202588.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://paj.316326.xyz

TS:   if (!x) {}
来源：http://oah.yonumen.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uzm.daria6918.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nsx.andypj.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://whm.cdnleiting.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xis.tanke756.top

[A17] 位运算
来源：http://pkl.tanke756.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ilg.hnxiangtu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://glm.meibo888.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ixx.zdqjudy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://zmv.shanyushiyangkeji.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kvv.shuidangran.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://onu.jianghu66.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gay.guannengcc.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://poh.yj20258.top

[A18] 字符与 ASCII 码互转
来源：http://hqk.pycfn.com

Py:   ord("A"); chr(65)
来源：http://pjr.shanyushiyangkeji.top

PHP:  ord("A"); chr(65)
来源：http://oie.hywenlv.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hkc.yj202588.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hcx.gotoacloud.top

Java: (int) 'A'; (char) 65
来源：http://lrd.feifeiyinyue.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://cza.hywenlv.cn

Ruby: "A".ord; 65.chr
来源：http://kka.gotoacloud.top

C#:   (int)'A'; (char)65
来源：http://xau.yj202588.top

[A19] 交换两个变量
来源：http://ypy.yuanzhike.top

Py:   a, b = b, a
来源：http://lrj.gotoacloud.top

PHP:  [$a, $b] = [$b, $a];
来源：http://tlv.shangyingyoupin.top

JS:   [a, b] = [b, a];
来源：http://ktr.jinyuanbaomall.cn

TS:   [a, b] = [b, a];
来源：http://crq.xingfuxueyuan.xyz

Java: int t = a; a = b; b = t;
来源：http://xik.nanxuanxn.top

Go:   a, b = b, a
来源：http://cnw.hfpthk.cn

Ruby: a, b = b, a
来源：http://zuz.gogol.net.cn

C#:   (a, b) = (b, a);
来源：http://vct.c1oappe.top

[A20] 读取标准输入
来源：http://ifj.jqgfzy.top

Py:   name = input("请输入：")
来源：http://aym.hammf.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://irv.9152youxi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fpo.zycfv.cn

TS:   // Node.js：readline 模块
来源：http://eqh.xuetiantiany.cn

Java: new Scanner(System.in).nextLine()
来源：http://xma.cheryme.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yqw.sxryk.cn

Ruby: gets.chomp
来源：http://oro.yj20258.top

C#:   Console.ReadLine();
来源：http://lps.daria6918.cn

[A21] 保留指定小数位输出
来源：http://boh.smart0.xyz

Py:   f"{3.14159:.2f}"
来源：http://sdz.shzxlz.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ivc.sxryk.cn

JS:   (3.14159).toFixed(2)
来源：http://prf.jinyuanbaomall.cn

TS:   (3.14159).toFixed(2)
来源：http://tfw.hammf.cn

Java: String.format("%.2f", 3.14159)
来源：http://mjc.ppjwa.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ccu.jinyuanbaomall.cn

Ruby: format("%.2f", 3.14159)
来源：http://zqf.ppjwa.cn

C#:   3.14159.ToString("F2")
来源：http://nox.zhongyouzk.top

[A22] 获取字符串长度
来源：http://cdw.zhoulong.xyz

Py:   len(s)
来源：http://jrz.316326.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qjn.xziqi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fnz.fktsv.cn

TS:   s.length
来源：http://ppm.svipenyu.cn

Java: s.length()
来源：http://awz.jqgfzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://crb.meibo888.top

Ruby: s.length
来源：http://sid.daria6918.cn

C#:   s.Length
来源：http://ibv.xuanzx.com

[A23] 大小写转换
来源：http://bzo.fanxiaobao.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://bkm.fzhhl.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://gna.shuidangran.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://oit.cheryme.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://luv.havefunace.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rbp.chenjidiqi.icu

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://btb.hnqzz.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://upv.tian-w.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://lul.jinqigufen.top

[A24] 去除首尾空白
来源：http://xkc.yonumen.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://rgv.jianghu66.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://gak.cqqwz.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vhm.redwolf501.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vld.ywan-chungtsiang.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mcc.sxryk.cn

Go:   strings.TrimSpace(s)
来源：http://xsl.hongshengwenyu.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tsj.yvedp.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wck.tarul.cn

[A25] 字符串比较
来源：http://hcz.tianlin.xyz

Py:   s1 == s2; s1 != s2
来源：http://lyd.shuidangran.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://scx.vqdsnc.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qnh.pengpengdd.cyou

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ilv.nanxuanxn.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uuq.zdbjq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yvl.fengsongda.top

Ruby: s1 == s2; s1 <=> s2
来源：http://hgt.nwbrower.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qxp.aizwys.cn

[A26] 类型转换总览
来源：http://dzm.jlsjyb.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mgp.sweek.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://kbe.sweek.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ekm.feifeiyinyue.top

TS:   Number() String() Boolean() x as number
来源：http://aia.zhiwuduotai.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zce.shuidangran.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://oss.fzhhl.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://sne.jinghuilouyu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://myc.ehwqpu.com

================================================================================
来源：http://ico.yj202588.top

B. 流程控制
来源：http://zgq.zhiwuduotai.top

================================================================================
来源：http://ziq.havefunace.top

[B01] 条件判断 if / else
来源：http://acf.snrcjt.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dnj.c1oappe.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://efj.316326.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cvn.ehwqpu.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tqs.ppjwa.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://iyj.smart0.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://nch.yj202588.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://eyo.tian-w.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://smo.pycfn.com

[B02] 多分支 else if / elif
来源：http://ogj.sjlbkw.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lxt.xziqi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://xnc.shzxlz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://inz.xinyue.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jfr.yueranfly.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yjy.sysykeji.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dzp.shanyushiyangtech.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://sfo.tianlin.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://edi.daria6918.cn

[B03] switch / match / case
来源：http://boz.zhixingplan.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ian.xylfe.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://bga.cashguo.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uts.jinghuilouyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sbq.andypj.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gxi.vehdjk.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hwa.ybcxt.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://cey.jyoumei.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://pgb.yuanzhike.top

[B04] for 计数循环
来源：http://rsx.316326.xyz

Py:   for i in range(10): print(i)
来源：http://qeh.tanke756.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ong.epnwcf.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jhf.bbcook.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ywy.hesvh.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://edy.gaohongyu789.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://abw.guowangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://mjg.cdnleiting.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fle.52xcode.cn

[B05] 遍历数组 / 列表
来源：http://bwu.hfpthk.cn

Py:   for item in arr: print(item)
来源：http://zed.gogol.net.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sqb.dashuyun.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://orz.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://duy.hnqzz.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hng.chenjidiqi.icu

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ram.c1oappe.top

Ruby: arr.each { |item| puts item }
来源：http://hyp.yuanzhike.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bui.gaohongyu789.top

[B06] 遍历字典 / 对象
来源：http://vjb.svipenyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://lci.uphjek.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ulj.pengpengdd.cyou

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wvw.hongshengwenyu.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kzr.ehwqpu.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://avg.nwbrower.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wgr.havefunace.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lbc.shangyingyoupin.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ali.dianchejie.cn

[B07] while 循环
来源：http://amu.bbcook.cn

Py:   while i < 10: i += 1
来源：http://oso.yangfankeji.com

PHP:  while ($i < 10) { $i++; }
来源：http://pnn.havefunace.top

JS:   while (i < 10) { i++; }
来源：http://hwj.jyoumei.cn

TS:   while (i < 10) { i++; }
来源：http://bww.jyoumei.cn

Java: while (i < 10) { i++; }
来源：http://vwy.jqgfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nml.yueranfly.top

Ruby: while i < 10; i += 1; end
来源：http://zoi.shuidangran.top

C#:   while (i < 10) { i++; }
来源：http://bvj.hesvh.cn

[B08] do-while（至少执行一次）
来源：http://qry.cdnleiting.top

Py:   # 无 do-while：用 while True + break
来源：http://zch.guannengcc.top

PHP:  do { $i++; } while ($i < 10);
来源：http://dth.kuanghao11.cn

JS:   do { i++; } while (i < 10);
来源：http://zge.daria6918.cn

TS:   do { i++; } while (i < 10);
来源：http://srb.xziqi.cn

Java: do { i++; } while (i < 10);
来源：http://ppj.yuanzhike.top

Go:   for { i++; if i >= 10 { break } }
来源：http://ehw.ydzc1.top

Ruby: begin; i += 1; end while i < 10
来源：http://ylx.tianlin.xyz

C#:   do { i++; } while (i < 10);
来源：http://joh.yongpay.top

[B09] break 与 continue
来源：http://adg.tianlin.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://whw.yueranfly.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tde.yuanzhike.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ety.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vqu.epnwcf.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bpg.zdqjudy.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://emq.bbcook.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://eab.zhiwuduotai.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ijv.nanxuanxn.top

[B10] 遍历同时拿索引
来源：http://mhc.svipenyu.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://ysu.fehbvm.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tdb.ivvv.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hkr.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://zdv.ehwqpu.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://tlw.0kj1m.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gkf.jinqigufen.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://oyc.fengsongda.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vty.0kj1m.cn

[B11] 生成数字序列 / 区间
来源：http://vtr.zhijiandao.cn

Py:   list(range(0, 10, 2))
来源：http://pph.ywan-chungtsiang.top

PHP:  range(0, 10, 2);
来源：http://mqw.sufxvd.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tak.hnqzz.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qiy.hnqzz.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gez.bjfxy.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://iuc.jqgfzy.top

Ruby: (0...10).step(2).to_a
来源：http://hxp.ivvv.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://urj.hfpthk.cn

[B12] 跳出多层循环
来源：http://awt.hammf.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://qgp.smart0.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://tkj.redwolf501.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ztv.zhixingplan.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://otr.epnwcf.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wjs.jinyuanbaomall.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://seb.gaohongyu789.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://psx.gogol.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://dgq.yj20258.top

[B13] 判断是否为数字
来源：http://gkp.xziqi.cn

Py:   isinstance(x, (int, float))
来源：http://bxf.yj202588.top

PHP:  is_numeric($x)
来源：http://fgo.ivvv.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jep.nwbrower.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nbf.hesvh.cn

Java: x instanceof Number
来源：http://cgq.ctjpmb.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://irm.tarul.cn

Ruby: x.is_a?(Numeric)
来源：http://hlg.daria6918.cn

C#:   x is int or double or decimal
来源：http://dew.yvedp.cn

[B14] 判断值是否在集合内
来源：http://xda.tanke756.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://axf.ywan-chungtsiang.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xsp.zhongyouzk.top

JS:   [1, 2, 3].includes(x)
来源：http://vjr.pycfn.com

TS:   [1, 2, 3].includes(x)
来源：http://ogn.ppjwa.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://hzd.gogol.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kyu.0kj1m.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vys.c1oappe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cgp.shangyingyoupin.top

[B15] 布尔运算与取反
来源：http://hbt.meibo888.top

Py:   a and b or not c
来源：http://rdc.shuidangran.top

PHP:  $a && $b || !$c
来源：http://tja.cashguo.top

JS:   a && b || !c
来源：http://mrd.epnwcf.com

TS:   a && b || !c
来源：http://odg.xingfuxueyuan.xyz

Java: a && b || !c
来源：http://oji.chenlongwang.top

Go:   a && b || !c
来源：http://wtq.sxryk.cn

Ruby: a && b || !c
来源：http://wrv.feifeiyinyue.top

C#:   a && b || !c
来源：http://vnb.smart0.xyz

[B16] 卫语句：不满足条件提前返回
来源：http://quy.316326.xyz

Py:   if not data: return
来源：http://uvd.nwbrower.top

PHP:  if (!$data) { return; }
来源：http://mph.sweek.top

JS:   if (!data) return;
来源：http://xxh.jinqigufen.top

TS:   if (!data) return;
来源：http://ogn.gotoacloud.top

Java: if (data == null) return;
来源：http://fzs.fanxiaobao.xyz

Go:   if data == nil { return }
来源：http://vke.fehbvm.com

Ruby: return if data.nil?
来源：http://ftd.yueranfly.top

C#:   if (data == null) return;
来源：http://ene.jinyuanbaomall.cn

================================================================================
来源：http://pfw.snrcjt.cn

C. 函数与作用域
来源：http://uxt.ywan-chungtsiang.top

================================================================================
来源：http://fxv.shzxlz.cn

[C01] 定义函数
来源：http://ydi.quarkkingdee.top

Py:   def add(a, b): return a + b
来源：http://voq.pengpengdd.cyou

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://bsm.gaohongyu789.top

JS:   function add(a, b) { return a + b; }
来源：http://isy.yj202588.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hxn.pycfn.com

Java: static int add(int a, int b) { return a + b; }
来源：http://egp.sysykeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://kic.jqgufenzy.top

Ruby: def add(a, b); a + b; end
来源：http://rww.zdqjudy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qjf.mhx1999.top

[C02] 默认参数
来源：http://rey.jiagoushi.top

Py:   def greet(name="World"): return name
来源：http://ytg.quarkkingdee.top

PHP:  function greet($name = "World") { return $name; }
来源：http://idk.gaohongyu789.top

JS:   function greet(name = "World") { return name; }
来源：http://vvo.yangfankeji.com

TS:   function greet(name: string = "World") { return name; }
来源：http://tbp.jiagoushi.top

Java: // 无默认参数：方法重载或 Optional
来源：http://kfq.0kj1m.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://aep.smart0.xyz

Ruby: def greet(name = "World") = name
来源：http://gqn.zhoulong.xyz

C#:   string Greet(string name = "World") => name;
来源：http://tyn.yangfankeji.com

[C03] 可变参数
来源：http://fii.yuxming.cn

Py:   def total(*args): return sum(args)
来源：http://gtw.zhongyouzk.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://lmf.aibaodan.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rif.quarkkingdee.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://utl.fzhhl.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xzm.chenlongwang.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hkb.haohaochexian.top

Ruby: def total(*nums); nums.sum; end
来源：http://bdx.jinghuilouyu.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gyh.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://ffp.gogol.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://feh.gzhubu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://viv.hesvh.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vov.bbcook.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://yey.chenzaomai.com

Java: // 无：用 Builder 模式或 record
来源：http://vua.pycfn.com

Go:   // 无：用配置结构体参数
来源：http://ckh.yuanzhike.top

Ruby: f(a: 1, b: 2)
来源：http://xpi.cashguo.top

C#:   f(a: 1, b: 2)
来源：http://nxh.hnxiangtu.top

[C05] 返回多个值
来源：http://uwe.hcnkem.com

Py:   return a, b
来源：http://mqh.zycfv.cn

PHP:  return [$a, $b];
来源：http://chu.epnwcf.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://dig.cdnleiting.top

TS:   return { a, b };
来源：http://kfb.hnqzz.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://oph.ivvv.top

Go:   return a, b
来源：http://don.zhixingplan.top

Ruby: return a, b
来源：http://ees.xinyue.icu

C#:   return (a, b);              // ValueTuple
来源：http://ucc.daria6918.cn


<!-- 参考信息 -->