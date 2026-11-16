代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://dia.shanyushiyangkeji.top

TS:   const value = data ?? "默认值";
来源：http://fmv.zhengqikj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://pgf.zycfv.cn

Go:   if data == "" { data = "默认值" }
来源：http://dat.daria6918.cn

Ruby: value = data || "默认值"
来源：http://pas.jyoumei.cn

C#:   var value = data ?? "默认值";
来源：http://yxd.andypj.xyz

[A16] 真假值判断规则
来源：http://rpw.ehwqpu.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wye.wangshuangyany.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://sgi.cdnleiting.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mzz.pycfn.com

TS:   if (!x) {}
来源：http://esm.0kj1m.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://zpa.jinqigufen.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dmy.hfpthk.cn

Ruby: unless x            # nil 与 false 为假
来源：http://cjz.xylfe.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gog.daxiang520.top

[A17] 位运算
来源：http://scp.tarul.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vjf.pycfn.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wrp.dashuyun.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oiq.hfpthk.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kof.daxiang520.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qwf.kuanghao11.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lyt.feifeiyinyue.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sah.sxryk.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://itg.xuanzx.com

[A18] 字符与 ASCII 码互转
来源：http://trx.pycfn.com

Py:   ord("A"); chr(65)
来源：http://qzb.quarkkingdee.top

PHP:  ord("A"); chr(65)
来源：http://rpb.fehbvm.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://njy.zhaomingkeji.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uhv.sweek.top

Java: (int) 'A'; (char) 65
来源：http://kce.316326.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://szh.mhx1999.top

Ruby: "A".ord; 65.chr
来源：http://wmo.ybcxt.top

C#:   (int)'A'; (char)65
来源：http://zkh.pengpengdd.cyou

[A19] 交换两个变量
来源：http://ili.daria6918.cn

Py:   a, b = b, a
来源：http://toe.chenlongwang.top

PHP:  [$a, $b] = [$b, $a];
来源：http://rva.wangdashe.top

JS:   [a, b] = [b, a];
来源：http://mse.ppjwa.cn

TS:   [a, b] = [b, a];
来源：http://cjc.cdnleiting.top

Java: int t = a; a = b; b = t;
来源：http://mtg.zycfv.cn

Go:   a, b = b, a
来源：http://fnf.nanxuanxn.top

Ruby: a, b = b, a
来源：http://hpw.sxryk.cn

C#:   (a, b) = (b, a);
来源：http://qrd.aibaodan.cn

[A20] 读取标准输入
来源：http://tkk.yangfankeji.com

Py:   name = input("请输入：")
来源：http://wpi.yangfankeji.com

PHP:  $name = trim(fgets(STDIN));
来源：http://hyu.hesvh.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://esz.bjfxy.top

TS:   // Node.js：readline 模块
来源：http://sxd.mhx1999.top

Java: new Scanner(System.in).nextLine()
来源：http://rdb.vqdsnc.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://uek.cheryme.top

Ruby: gets.chomp
来源：http://tef.zdqjudy.top

C#:   Console.ReadLine();
来源：http://vhq.aizwys.cn

[A21] 保留指定小数位输出
来源：http://owi.pycfn.com

Py:   f"{3.14159:.2f}"
来源：http://asu.cheryme.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://lof.mhx1999.top

JS:   (3.14159).toFixed(2)
来源：http://zob.52xcode.cn

TS:   (3.14159).toFixed(2)
来源：http://wae.nanxuanxn.top

Java: String.format("%.2f", 3.14159)
来源：http://acb.yueranfly.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vml.0kj1m.cn

Ruby: format("%.2f", 3.14159)
来源：http://mef.chenjidiqi.icu

C#:   3.14159.ToString("F2")
来源：http://ogm.vehdjk.com

[A22] 获取字符串长度
来源：http://vsf.gogol.net.cn

Py:   len(s)
来源：http://dkr.yj20258888.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://huk.xylfe.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zha.yj20258.top

TS:   s.length
来源：http://tou.9152youxi.cn

Java: s.length()
来源：http://pnd.tian-w.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bly.jqgfzy.top

Ruby: s.length
来源：http://wpc.zhongyouzk.top

C#:   s.Length
来源：http://knv.yueranfly.top

[A23] 大小写转换
来源：http://lyr.hysaishi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://mje.hywenlv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kfi.feifeiyinyue.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dro.zhijiandao.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bxp.ydzc1.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lhv.jiagoushi.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kne.gogol.net.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ike.jinqigfzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xeg.xuetiantiany.cn

[A24] 去除首尾空白
来源：http://wof.aizwys.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nly.yongpay.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://rvn.yj20258888.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lvc.havefunace.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ctj.xinyue.icu

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://urj.epnwcf.com

Go:   strings.TrimSpace(s)
来源：http://xdv.ehwqpu.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://npz.ydjk.org.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wni.yueranfly.top

[A25] 字符串比较
来源：http://fxn.hnqzz.top

Py:   s1 == s2; s1 != s2
来源：http://ocp.aizwys.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jcp.xylfe.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://dje.xuanzx.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kaf.yongpay.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://fck.c1oappe.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ryj.yueranfly.top

Ruby: s1 == s2; s1 <=> s2
来源：http://dbk.jinyuanbaomall.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yoz.zhixingplan.top

[A26] 类型转换总览
来源：http://iik.tarul.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://tzd.hesvh.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iur.dashuyun.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mna.guannengcc.top

TS:   Number() String() Boolean() x as number
来源：http://qbe.zhaomingkeji.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://jqn.hongshengwenyu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qib.pengpengdd.cyou

Ruby: to_i to_f to_s to_sym to_a
来源：http://swx.cqqwz.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qqr.nanxuanxn.top

================================================================================
来源：http://rvf.jlsjyb.cn

B. 流程控制
来源：http://snk.zhiwuduotai.top

================================================================================
来源：http://azd.feifeiyinyue.top

[B01] 条件判断 if / else
来源：http://rtf.sysykeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://rvm.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://aty.zycfv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jnw.daxiang520.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kxh.guannengcc.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://pal.hnqzz.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fht.ywan-chungtsiang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dyi.daria6918.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bdy.yongpay.top

[B02] 多分支 else if / elif
来源：http://drg.zhaomingkeji.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qlj.guannengcc.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kmz.fktsv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qda.bjfxy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ozd.jianghu66.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hvl.jianghu66.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bxx.daria6918.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ozf.jlsjyb.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jpt.cucudq.cn

[B03] switch / match / case
来源：http://xug.ybcxt.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kij.vehdjk.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oip.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nhk.nanxinkj.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cqe.hfpthk.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ndk.zhongyouzk.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://drf.bjfxy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dft.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://drj.svipenyu.cn

[B04] for 计数循环
来源：http://ruv.shangyingyoupin.top

Py:   for i in range(10): print(i)
来源：http://uef.hywenlv.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wcr.yfazqb.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://lhf.aizwys.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kic.jinghuilouyu.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wax.zhixingplan.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nnf.sjlbkw.cn

Ruby: 10.times { |i| puts i }
来源：http://fpl.gotoacloud.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lkz.fzhhl.top

[B05] 遍历数组 / 列表
来源：http://prp.yangfankeji.com

Py:   for item in arr: print(item)
来源：http://nkl.zhixingplan.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mls.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://lvz.ctjpmb.com

TS:   for (const item of arr) { console.log(item); }
来源：http://dxt.snrcjt.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://wsf.shanyushiyangkeji.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://sci.jianghu66.top

Ruby: arr.each { |item| puts item }
来源：http://uob.ehwqpu.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://nej.zhixingplan.top

[B06] 遍历字典 / 对象
来源：http://kee.jyoumei.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ofx.fktsv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fmz.havefunace.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mly.xingfuxueyuan.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qlo.ywan-chungtsiang.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sad.svipenyu.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://oyh.cashguo.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qnu.zhijiandao.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pxq.mhx1999.top

[B07] while 循环
来源：http://adl.gzhubu.top

Py:   while i < 10: i += 1
来源：http://nab.yvedp.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ksa.zdbjq.cn

JS:   while (i < 10) { i++; }
来源：http://moo.guannengcc.top

TS:   while (i < 10) { i++; }
来源：http://zfs.guannengcc.top

Java: while (i < 10) { i++; }
来源：http://ywl.ywan-chungtsiang.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rym.xuanzx.com

Ruby: while i < 10; i += 1; end
来源：http://teu.pycfn.com

C#:   while (i < 10) { i++; }
来源：http://ton.yj20258.top

[B08] do-while（至少执行一次）
来源：http://cfc.redwolf501.top

Py:   # 无 do-while：用 while True + break
来源：http://smy.316326.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://ota.yanxiufei.cn

JS:   do { i++; } while (i < 10);
来源：http://ify.epnwcf.com

TS:   do { i++; } while (i < 10);
来源：http://owe.c1oappe.top

Java: do { i++; } while (i < 10);
来源：http://hsq.shanyushiyangkeji.top

Go:   for { i++; if i >= 10 { break } }
来源：http://vai.tianlin.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://ubc.ivvv.top

C#:   do { i++; } while (i < 10);
来源：http://hlf.sysykeji.top

[B09] break 与 continue
来源：http://snd.vehdjk.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wqp.jqgfzy.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ert.cdnleiting.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://llo.jianghu66.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jxm.sysykeji.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://slb.jlsjyb.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wli.chenzaomai.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dnl.dashuyun.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jgl.bbcook.cn

[B10] 遍历同时拿索引
来源：http://rgh.yj20258.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pze.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bew.jlsjyb.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://xzp.jinqigufen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pba.guannengcc.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yhx.gogol.net.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://wrq.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pms.cqqwz.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://afe.kuanghao11.cn

[B11] 生成数字序列 / 区间
来源：http://sxy.ydzc1.top

Py:   list(range(0, 10, 2))
来源：http://mla.ybcxt.top

PHP:  range(0, 10, 2);
来源：http://wez.svipenyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://usv.shanyushiyangtech.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://izk.cucudq.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lfm.xylfe.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hgx.jlsjyb.cn

Ruby: (0...10).step(2).to_a
来源：http://agy.cdnleiting.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jcm.jyoumei.cn

[B12] 跳出多层循环
来源：http://rci.yuxming.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wmm.nwbrower.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://uxw.uphjek.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jjc.ydzc1.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://vvs.xuetiantiany.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://efi.kuanghao11.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hfs.sweek.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://afq.vehdjk.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://lhy.yvedp.cn

[B13] 判断是否为数字
来源：http://nhv.ppjwa.cn

Py:   isinstance(x, (int, float))
来源：http://ssa.ydzc1.top

PHP:  is_numeric($x)
来源：http://vjx.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tij.fengsongda.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://csm.yongpay.top

Java: x instanceof Number
来源：http://dsa.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://enm.cucudq.cn

Ruby: x.is_a?(Numeric)
来源：http://dfe.sxryk.cn

C#:   x is int or double or decimal
来源：http://lyo.tarul.cn

[B14] 判断值是否在集合内
来源：http://klb.hywenlv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lfe.fengsongda.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jbt.cucudq.cn

JS:   [1, 2, 3].includes(x)
来源：http://wwh.chenlongwang.top

TS:   [1, 2, 3].includes(x)
来源：http://mjs.52xcode.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ggp.uphjek.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jcu.nanxinkj.top

Ruby: [1, 2, 3].include?(x)
来源：http://tdp.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yur.daxiang520.top

[B15] 布尔运算与取反
来源：http://emk.bbcook.cn

Py:   a and b or not c
来源：http://zht.9152youxi.cn

PHP:  $a && $b || !$c
来源：http://xqw.hfpthk.cn

JS:   a && b || !c
来源：http://pgi.tarul.cn

TS:   a && b || !c
来源：http://qal.gzhubu.top

Java: a && b || !c
来源：http://fth.zhengqikj.top

Go:   a && b || !c
来源：http://dwf.iojbl.cn

Ruby: a && b || !c
来源：http://utm.yuanzhike.top

C#:   a && b || !c
来源：http://ehk.hywenlv.cn

[B16] 卫语句：不满足条件提前返回
来源：http://she.52xcode.cn

Py:   if not data: return
来源：http://gxh.ctjpmb.com

PHP:  if (!$data) { return; }
来源：http://liq.jlsjyb.cn

JS:   if (!data) return;
来源：http://pga.ybcxt.top

TS:   if (!data) return;
来源：http://gsc.sweek.top

Java: if (data == null) return;
来源：http://xad.yanxiufei.cn

Go:   if data == nil { return }
来源：http://wow.tanke756.top

Ruby: return if data.nil?
来源：http://rlj.zhixingplan.top

C#:   if (data == null) return;
来源：http://tfu.hysaishi.cn

================================================================================
来源：http://ugj.yfazqb.com

C. 函数与作用域
来源：http://sbi.kuanghao11.cn

================================================================================
来源：http://vcg.316326.xyz

[C01] 定义函数
来源：http://ybd.hesvh.cn

Py:   def add(a, b): return a + b
来源：http://gef.yj20258.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zmh.0kj1m.cn

JS:   function add(a, b) { return a + b; }
来源：http://mcr.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bja.fengsongda.top

Java: static int add(int a, int b) { return a + b; }
来源：http://yss.quarkkingdee.top

Go:   func add(a, b int) int { return a + b }
来源：http://czn.hammf.cn

Ruby: def add(a, b); a + b; end
来源：http://bia.ydjk.org.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ucm.zhixingplan.top

[C02] 默认参数
来源：http://cll.ybcxt.top

Py:   def greet(name="World"): return name
来源：http://wej.ywan-chungtsiang.top

PHP:  function greet($name = "World") { return $name; }
来源：http://ell.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://zct.9152youxi.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://mqo.chenlongwang.top

Java: // 无默认参数：方法重载或 Optional
来源：http://pci.gogol.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://arn.zdbjq.cn

Ruby: def greet(name = "World") = name
来源：http://vok.cheryme.top

C#:   string Greet(string name = "World") => name;
来源：http://his.zdbjq.cn

[C03] 可变参数
来源：http://bok.sjlbkw.cn

Py:   def total(*args): return sum(args)
来源：http://xmm.sjlbkw.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kce.nanxinkj.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ccg.daria6918.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://qlf.sweek.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nuc.meibo888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gmx.sufxvd.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ezm.chenlongwang.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jbf.dashuyun.cn

[C04] 命名参数 / 关键字参数
来源：http://mvy.zdbjq.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rnm.andypj.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xyo.jqgufenzy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://agw.chenzaomai.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://zuw.dianchejie.cn

Java: // 无：用 Builder 模式或 record
来源：http://gvk.yj202588.top

Go:   // 无：用配置结构体参数
来源：http://ywy.tarul.cn

Ruby: f(a: 1, b: 2)
来源：http://tcd.shanyushiyangtech.top

C#:   f(a: 1, b: 2)
来源：http://dwp.chenlongwang.top

[C05] 返回多个值
来源：http://boy.dianchejie.cn

Py:   return a, b
来源：http://jns.fehbvm.com

PHP:  return [$a, $b];
来源：http://qzk.shangyingyoupin.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://bxm.yongpay.top

TS:   return { a, b };
来源：http://yfa.yfazqb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://joq.cucudq.cn

Go:   return a, b
来源：http://ars.chenjidiqi.icu

Ruby: return a, b
来源：http://whk.haohaochexian.top

C#:   return (a, b);              // ValueTuple
来源：http://nhd.yangfankeji.com


<!-- 参考信息 -->