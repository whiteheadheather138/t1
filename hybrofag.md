代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://nhs.zhaomingkeji.xyz

TS:   const value = data ?? "默认值";
来源：http://qik.ybcxt.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://uqs.iojbl.cn

Go:   if data == "" { data = "默认值" }
来源：http://tbr.ehwqpu.com

Ruby: value = data || "默认值"
来源：http://hse.yonumen.top

C#:   var value = data ?? "默认值";
来源：http://upv.chenjidiqi.icu

[A16] 真假值判断规则
来源：http://gyw.zdqjudy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://upw.gaohongyu789.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ahy.vqdsnc.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lgq.dianchejie.cn

TS:   if (!x) {}
来源：http://doa.ehwqpu.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://abo.zhixingplan.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://swq.dashuyun.cn

Ruby: unless x            # nil 与 false 为假
来源：http://tqq.iojbl.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hzq.pycfn.com

[A17] 位运算
来源：http://szx.epnwcf.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ove.yvedp.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wal.chenlongwang.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nmp.cashguo.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wea.chenjidiqi.icu

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://msb.cheryme.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wqa.tian-w.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xjk.hesvh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tgq.zhoulong.xyz

[A18] 字符与 ASCII 码互转
来源：http://xfl.fktsv.cn

Py:   ord("A"); chr(65)
来源：http://onl.fanxiaobao.xyz

PHP:  ord("A"); chr(65)
来源：http://nna.yongpay.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ltn.chenlongwang.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rdp.nanxinkj.top

Java: (int) 'A'; (char) 65
来源：http://ykj.ehwqpu.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://anv.zhijiandao.cn

Ruby: "A".ord; 65.chr
来源：http://vry.jyoumei.cn

C#:   (int)'A'; (char)65
来源：http://fnq.hnxiangtu.top

[A19] 交换两个变量
来源：http://aho.bbcook.cn

Py:   a, b = b, a
来源：http://xdp.kuanghao11.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ncx.zdbjq.cn

JS:   [a, b] = [b, a];
来源：http://lis.zhoulong.xyz

TS:   [a, b] = [b, a];
来源：http://rvg.yj20258.top

Java: int t = a; a = b; b = t;
来源：http://qwt.tianlin.xyz

Go:   a, b = b, a
来源：http://ozd.tianlin.xyz

Ruby: a, b = b, a
来源：http://wud.ydzc1.top

C#:   (a, b) = (b, a);
来源：http://puo.dashuyun.cn

[A20] 读取标准输入
来源：http://add.bbcook.cn

Py:   name = input("请输入：")
来源：http://ryo.yuanzhike.top

PHP:  $name = trim(fgets(STDIN));
来源：http://nhx.feifeiyinyue.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fkz.shuidangran.top

TS:   // Node.js：readline 模块
来源：http://mwt.fanxiaobao.xyz

Java: new Scanner(System.in).nextLine()
来源：http://eak.sjlbkw.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fwq.fanxiaobao.xyz

Ruby: gets.chomp
来源：http://ivx.redwolf501.top

C#:   Console.ReadLine();
来源：http://elr.daxiang520.top

[A21] 保留指定小数位输出
来源：http://dws.zycfv.cn

Py:   f"{3.14159:.2f}"
来源：http://geo.feifeiyinyue.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://azv.vehdjk.com

JS:   (3.14159).toFixed(2)
来源：http://aqn.epnwcf.com

TS:   (3.14159).toFixed(2)
来源：http://nhm.0kj1m.cn

Java: String.format("%.2f", 3.14159)
来源：http://zmk.xingfuxueyuan.xyz

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hqf.c1oappe.top

Ruby: format("%.2f", 3.14159)
来源：http://bex.vehdjk.com

C#:   3.14159.ToString("F2")
来源：http://coh.redwolf501.top

[A22] 获取字符串长度
来源：http://qvx.shanyushiyangtech.top

Py:   len(s)
来源：http://trd.sysykeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ybf.haohaochexian.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gtk.xingfuxueyuan.xyz

TS:   s.length
来源：http://rxp.aizwys.cn

Java: s.length()
来源：http://pgl.sjlbkw.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://awo.ydzc1.top

Ruby: s.length
来源：http://ihb.zhaomingkeji.xyz

C#:   s.Length
来源：http://qdn.snrcjt.cn

[A23] 大小写转换
来源：http://sem.gzhubu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://tld.smart0.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lhr.epnwcf.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fxb.hongshengwenyu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://yfv.fehbvm.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fak.mhx1999.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xex.shzxlz.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hod.dianchejie.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://whd.havefunace.top

[A24] 去除首尾空白
来源：http://anx.yj202588.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qlh.sysykeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://eml.jqgfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://svl.haohaochexian.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hna.svipenyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hvo.jqgufenzy.top

Go:   strings.TrimSpace(s)
来源：http://fog.zycfv.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://pal.jianghu66.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bei.yvedp.cn

[A25] 字符串比较
来源：http://erh.uphjek.com

Py:   s1 == s2; s1 != s2
来源：http://isg.sweek.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wyy.ydzc1.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hfh.cdnleiting.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ycy.gotoacloud.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bef.nanxinkj.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xpf.yongpay.top

Ruby: s1 == s2; s1 <=> s2
来源：http://let.tianlin.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zpr.yj20258.top

[A26] 类型转换总览
来源：http://bst.fanxiaobao.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://knz.cheryme.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wqy.bbcook.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://rif.hnqzz.top

TS:   Number() String() Boolean() x as number
来源：http://qfo.xingfuxueyuan.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hhf.guowangkeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://pat.zhoulong.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://ifq.yuxming.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yci.shanyushiyangkeji.top

================================================================================
来源：http://gyx.nanxinkj.top

B. 流程控制
来源：http://czh.nwbrower.top

================================================================================
来源：http://zvp.yvedp.cn

[B01] 条件判断 if / else
来源：http://anf.jlsjyb.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://ubq.jinghuilouyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://pby.jinqigufen.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://szx.sysykeji.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wmn.daria6918.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://qsj.jyoumei.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bao.ppjwa.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nug.daxiang520.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wbi.mhx1999.top

[B02] 多分支 else if / elif
来源：http://npn.epnwcf.com

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://thh.hywenlv.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nyo.tanke756.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ylo.shuidangran.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xir.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cln.jinyuanbaomall.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://akm.zhijiandao.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://djy.epnwcf.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pty.ydjk.org.cn

[B03] switch / match / case
来源：http://vvh.tianlin.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://obd.hammf.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rqk.tian-w.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://grh.hfpthk.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lbx.jqgfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iqk.haohaochexian.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://rzc.yonumen.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://sqi.jiagoushi.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vfr.xinyue.icu

[B04] for 计数循环
来源：http://esm.snrcjt.cn

Py:   for i in range(10): print(i)
来源：http://dip.wangshuangyany.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://rob.yangfankeji.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fsl.ydzc1.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kbk.zhengqikj.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://gjv.hesvh.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ock.ehwqpu.com

Ruby: 10.times { |i| puts i }
来源：http://zcg.kuanghao11.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://rni.shangyingyoupin.top

[B05] 遍历数组 / 列表
来源：http://edz.shanyushiyangkeji.top

Py:   for item in arr: print(item)
来源：http://hgw.aizwys.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://oce.sweek.top

JS:   for (const item of arr) { console.log(item); }
来源：http://zah.c1oappe.top

TS:   for (const item of arr) { console.log(item); }
来源：http://yap.jyoumei.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gzq.zhongyouzk.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zka.meibo888.top

Ruby: arr.each { |item| puts item }
来源：http://hqa.chenlongwang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qzd.havefunace.top

[B06] 遍历字典 / 对象
来源：http://cmr.fanxiaobao.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://jcq.ehwqpu.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qoe.tarul.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wqm.yueranfly.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tyi.shanyushiyangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://waq.fktsv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vkv.cashguo.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ctn.fzhhl.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ydm.yongpay.top

[B07] while 循环
来源：http://hjh.hysaishi.cn

Py:   while i < 10: i += 1
来源：http://mib.zhengqikj.top

PHP:  while ($i < 10) { $i++; }
来源：http://ehu.dashuyun.cn

JS:   while (i < 10) { i++; }
来源：http://icv.tanke756.top

TS:   while (i < 10) { i++; }
来源：http://xmm.ydjk.org.cn

Java: while (i < 10) { i++; }
来源：http://mqt.jianghu66.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hbr.yongpay.top

Ruby: while i < 10; i += 1; end
来源：http://arf.zycfv.cn

C#:   while (i < 10) { i++; }
来源：http://uxg.daxiang520.top

[B08] do-while（至少执行一次）
来源：http://irx.dianchejie.cn

Py:   # 无 do-while：用 while True + break
来源：http://jut.wangshuangyany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://xzj.sufxvd.cn

JS:   do { i++; } while (i < 10);
来源：http://wix.tianlin.xyz

TS:   do { i++; } while (i < 10);
来源：http://xmf.zhixingplan.top

Java: do { i++; } while (i < 10);
来源：http://axs.bbcook.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gfd.jyoumei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://vtj.cdnleiting.top

C#:   do { i++; } while (i < 10);
来源：http://dzh.gzhubu.top

[B09] break 与 continue
来源：http://dby.yuxming.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ius.hongshengwenyu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://skx.yanxiufei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tah.snrcjt.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xju.zhijiandao.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uic.jyoumei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://unq.sweek.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ioh.ehwqpu.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aks.52xcode.cn

[B10] 遍历同时拿索引
来源：http://gjy.hnqzz.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vem.yongpay.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xqd.yangfankeji.com

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://cls.yfazqb.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fcl.yj20258.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zab.sxryk.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://dru.yangfankeji.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tbw.sxryk.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://pkm.52xcode.cn

[B11] 生成数字序列 / 区间
来源：http://wae.sweek.top

Py:   list(range(0, 10, 2))
来源：http://cid.zhijiandao.cn

PHP:  range(0, 10, 2);
来源：http://xhh.jqgufenzy.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://daw.hnqzz.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hfq.guannengcc.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://duu.sxryk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mxw.hesvh.cn

Ruby: (0...10).step(2).to_a
来源：http://ukp.ivvv.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wyd.bjfxy.top

[B12] 跳出多层循环
来源：http://alw.fehbvm.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://ptq.yuanzhike.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pfk.hfpthk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qrz.jqgufenzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qus.zdqjudy.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ohx.dashuyun.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fph.ivvv.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lvo.ydjk.org.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eyl.guannengcc.top

[B13] 判断是否为数字
来源：http://tch.hnxiangtu.top

Py:   isinstance(x, (int, float))
来源：http://zlw.aizwys.cn

PHP:  is_numeric($x)
来源：http://laf.bjfxy.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hsq.wangdashe.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zce.gotoacloud.top

Java: x instanceof Number
来源：http://vut.chenjidiqi.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://nkk.fanxiaobao.xyz

Ruby: x.is_a?(Numeric)
来源：http://eef.aizwys.cn

C#:   x is int or double or decimal
来源：http://sdr.jinqigufen.top

[B14] 判断值是否在集合内
来源：http://hnt.mhx1999.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://azz.jqgfzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yvr.zycfv.cn

JS:   [1, 2, 3].includes(x)
来源：http://ogg.cheryme.top

TS:   [1, 2, 3].includes(x)
来源：http://tgx.fengsongda.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hfw.havefunace.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://osy.sjlbkw.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vgk.cdnleiting.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kbn.birdmap.top

[B15] 布尔运算与取反
来源：http://vvc.yj202588.top

Py:   a and b or not c
来源：http://eog.fktsv.cn

PHP:  $a && $b || !$c
来源：http://lnk.yj202588.top

JS:   a && b || !c
来源：http://lqp.nanxuanxn.top

TS:   a && b || !c
来源：http://ztk.jinqigfzy.top

Java: a && b || !c
来源：http://kuv.hnqzz.top

Go:   a && b || !c
来源：http://hcc.zdbjq.cn

Ruby: a && b || !c
来源：http://znf.ivvv.top

C#:   a && b || !c
来源：http://rlj.fengsongda.top

[B16] 卫语句：不满足条件提前返回
来源：http://hkf.jinqigufen.top

Py:   if not data: return
来源：http://xmo.sweek.top

PHP:  if (!$data) { return; }
来源：http://zax.jinghuilouyu.cn

JS:   if (!data) return;
来源：http://zkh.bbcook.cn

TS:   if (!data) return;
来源：http://luh.yongpay.top

Java: if (data == null) return;
来源：http://pmd.yonumen.top

Go:   if data == nil { return }
来源：http://bjk.shuidangran.top

Ruby: return if data.nil?
来源：http://aqj.xziqi.cn

C#:   if (data == null) return;
来源：http://olw.mhx1999.top

================================================================================
来源：http://iuj.zdqjudy.top

C. 函数与作用域
来源：http://otf.daxiang520.top

================================================================================
来源：http://fup.9152youxi.cn

[C01] 定义函数
来源：http://nyj.cqqwz.cn

Py:   def add(a, b): return a + b
来源：http://nvz.jinqigfzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rgg.fanxiaobao.xyz

JS:   function add(a, b) { return a + b; }
来源：http://sjx.andypj.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cbn.aizwys.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sog.shanyushiyangkeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://hpt.jinqigufen.top

Ruby: def add(a, b); a + b; end
来源：http://uwl.mhx1999.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://waq.shzxlz.cn

[C02] 默认参数
来源：http://das.zdqjudy.top

Py:   def greet(name="World"): return name
来源：http://yxc.cashguo.top

PHP:  function greet($name = "World") { return $name; }
来源：http://pwg.yongpay.top

JS:   function greet(name = "World") { return name; }
来源：http://oko.daxiang520.top

TS:   function greet(name: string = "World") { return name; }
来源：http://gvx.jqgfzy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://rlu.sufxvd.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://pdg.sufxvd.cn

Ruby: def greet(name = "World") = name
来源：http://snf.jlsjyb.cn

C#:   string Greet(string name = "World") => name;
来源：http://qnh.cucudq.cn

[C03] 可变参数
来源：http://gci.hywenlv.cn

Py:   def total(*args): return sum(args)
来源：http://kyr.yuanzhike.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ftf.daxiang520.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rtf.quarkkingdee.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qqs.zhijiandao.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://sjf.hywenlv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cnz.hnqzz.top

Ruby: def total(*nums); nums.sum; end
来源：http://yoj.hnxiangtu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://grw.gotoacloud.top

[C04] 命名参数 / 关键字参数
来源：http://xdz.gogol.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://per.vehdjk.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://uls.zdqjudy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ama.yuxming.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xkx.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://zst.zhoulong.xyz

Go:   // 无：用配置结构体参数
来源：http://zzb.cashguo.top

Ruby: f(a: 1, b: 2)
来源：http://ynt.meibo888.top

C#:   f(a: 1, b: 2)
来源：http://qmy.vehdjk.com

[C05] 返回多个值
来源：http://ivc.yfazqb.com

Py:   return a, b
来源：http://crr.meibo888.top

PHP:  return [$a, $b];
来源：http://igl.tarul.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://lcp.bbcook.cn

TS:   return { a, b };
来源：http://byd.gzhubu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://psl.zhengqikj.top

Go:   return a, b
来源：http://rgz.feifeiyinyue.top

Ruby: return a, b
来源：http://ctk.tianlin.xyz

C#:   return (a, b);              // ValueTuple
来源：http://vuc.yanxiufei.cn


<!-- 参考信息 -->