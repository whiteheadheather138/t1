代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://prh.aibaodan.cn

Ruby: unless x            # nil 与 false 为假
来源：http://quq.fengsongda.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://gyz.bbcook.cn

[A17] 位运算
来源：http://cym.xinyue.icu

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cvh.gzhubu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://fxp.xinyue.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fki.uphjek.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ksj.zdqjudy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ptg.zycfv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fkk.tianlin.xyz

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ljn.zhaomingkeji.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zht.yj20258.top

[A18] 字符与 ASCII 码互转
来源：http://tez.ybcxt.top

Py:   ord("A"); chr(65)
来源：http://mwt.xziqi.cn

PHP:  ord("A"); chr(65)
来源：http://fxr.ydjk.org.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ydn.sxryk.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fou.aizwys.cn

Java: (int) 'A'; (char) 65
来源：http://uzp.guowangkeji.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tus.yuxming.cn

Ruby: "A".ord; 65.chr
来源：http://tdx.yangfankeji.com

C#:   (int)'A'; (char)65
来源：http://ncr.epnwcf.com

[A19] 交换两个变量
来源：http://lta.gaohongyu789.top

Py:   a, b = b, a
来源：http://jpp.gaohongyu789.top

PHP:  [$a, $b] = [$b, $a];
来源：http://ktx.dashuyun.cn

JS:   [a, b] = [b, a];
来源：http://esg.jqgufenzy.top

TS:   [a, b] = [b, a];
来源：http://ecp.haohaochexian.top

Java: int t = a; a = b; b = t;
来源：http://txz.vehdjk.com

Go:   a, b = b, a
来源：http://tmh.gotoacloud.top

Ruby: a, b = b, a
来源：http://bra.dashuyun.cn

C#:   (a, b) = (b, a);
来源：http://hyy.yanxiufei.cn

[A20] 读取标准输入
来源：http://veb.jianghu66.top

Py:   name = input("请输入：")
来源：http://zgs.ybcxt.top

PHP:  $name = trim(fgets(STDIN));
来源：http://pic.daria6918.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dkz.sufxvd.cn

TS:   // Node.js：readline 模块
来源：http://roa.fzhhl.top

Java: new Scanner(System.in).nextLine()
来源：http://uiy.ehwqpu.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fdr.dashuyun.cn

Ruby: gets.chomp
来源：http://pfm.nanxinkj.top

C#:   Console.ReadLine();
来源：http://iyv.jinqigfzy.top

[A21] 保留指定小数位输出
来源：http://yvt.jlsjyb.cn

Py:   f"{3.14159:.2f}"
来源：http://vem.feifeiyinyue.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tkt.tianlin.xyz

JS:   (3.14159).toFixed(2)
来源：http://dki.zhongyouzk.top

TS:   (3.14159).toFixed(2)
来源：http://ngg.jinqigfzy.top

Java: String.format("%.2f", 3.14159)
来源：http://pzz.fehbvm.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vrs.sysykeji.top

Ruby: format("%.2f", 3.14159)
来源：http://ibm.cdnleiting.top

C#:   3.14159.ToString("F2")
来源：http://ktl.sweek.top

[A22] 获取字符串长度
来源：http://rzq.jinqigufen.top

Py:   len(s)
来源：http://ivz.meibo888.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nml.ydzc1.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://lsc.ctjpmb.com

TS:   s.length
来源：http://hgi.aizwys.cn

Java: s.length()
来源：http://gjb.ybcxt.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zxf.yuxming.cn

Ruby: s.length
来源：http://hgn.pengpengdd.cyou

C#:   s.Length
来源：http://kar.nanxuanxn.top

[A23] 大小写转换
来源：http://rzt.yuxming.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://oyy.zdbjq.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xxu.xuetiantiany.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hno.kuanghao11.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hht.cashguo.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zqz.tarul.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jmi.guowangkeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://abk.jqgfzy.top

C#:   s.ToUpper(); s.ToLower()
来源：http://sdj.316326.xyz

[A24] 去除首尾空白
来源：http://yuu.chenzaomai.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ocs.ydjk.org.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://crt.zdqjudy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://knp.jyoumei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jpe.yj20258888.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dap.mhx1999.top

Go:   strings.TrimSpace(s)
来源：http://olj.zdbjq.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rqt.tarul.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://aqw.bbcook.cn

[A25] 字符串比较
来源：http://bik.fengsongda.top

Py:   s1 == s2; s1 != s2
来源：http://yos.gogol.net.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://btc.vehdjk.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://etx.nanxinkj.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wdu.fengsongda.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://czd.jinqigfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ala.shanyushiyangkeji.top

Ruby: s1 == s2; s1 <=> s2
来源：http://uze.mhx1999.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jue.ehwqpu.com

[A26] 类型转换总览
来源：http://agn.tanke756.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xgz.fanxiaobao.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lpj.zhijiandao.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://pmi.hammf.cn

TS:   Number() String() Boolean() x as number
来源：http://bua.andypj.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xfr.shangyingyoupin.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://dwf.yj20258888.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://ypj.hnxiangtu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://czf.zhongyouzk.top

================================================================================
来源：http://eqx.nanxuanxn.top

B. 流程控制
来源：http://gsu.jinqigufen.top

================================================================================
来源：http://xss.hfpthk.cn

[B01] 条件判断 if / else
来源：http://atf.mhx1999.top

Py:   result = "正" if x > 0 else "非正"
来源：http://azq.hywenlv.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uno.tarul.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://igh.ehwqpu.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://xny.shanyushiyangtech.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://gvw.daxiang520.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kmv.gzhubu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ddu.hnxiangtu.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://pwm.hcnkem.com

[B02] 多分支 else if / elif
来源：http://skq.daria6918.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yln.fehbvm.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zlc.hnxiangtu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jdn.sweek.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qwj.yonumen.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ney.fengsongda.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hha.yueranfly.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cvl.hongshengwenyu.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dto.aibaodan.cn

[B03] switch / match / case
来源：http://oss.0kj1m.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://njn.cdnleiting.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://rns.yj20258.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nqe.tian-w.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mcq.ctjpmb.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ijl.yuxming.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://quj.yfazqb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://udi.fehbvm.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://bjy.shanyushiyangkeji.top

[B04] for 计数循环
来源：http://ulb.jinqigfzy.top

Py:   for i in range(10): print(i)
来源：http://kum.shanyushiyangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dlt.jyoumei.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iuf.iojbl.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jno.sjlbkw.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ehb.haohaochexian.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://msu.chenjidiqi.icu

Ruby: 10.times { |i| puts i }
来源：http://mdl.yfazqb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qyy.fehbvm.com

[B05] 遍历数组 / 列表
来源：http://rvw.zhixingplan.top

Py:   for item in arr: print(item)
来源：http://wjo.fehbvm.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://vkv.chenzaomai.com

JS:   for (const item of arr) { console.log(item); }
来源：http://esb.guowangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ksv.cheryme.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zph.zhengqikj.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://phn.zhoulong.xyz

Ruby: arr.each { |item| puts item }
来源：http://fpe.ybcxt.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fns.wangshuangyany.cn

[B06] 遍历字典 / 对象
来源：http://sdh.wangdashe.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lqz.jinyuanbaomall.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://svz.hfpthk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mha.fanxiaobao.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wdz.yueranfly.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bqw.hysaishi.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ezg.kuanghao11.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cgp.vqdsnc.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yyf.zhixingplan.top

[B07] while 循环
来源：http://cco.dianchejie.cn

Py:   while i < 10: i += 1
来源：http://syb.jiagoushi.top

PHP:  while ($i < 10) { $i++; }
来源：http://fvo.quarkkingdee.top

JS:   while (i < 10) { i++; }
来源：http://gzx.yangfankeji.com

TS:   while (i < 10) { i++; }
来源：http://gjj.tian-w.cn

Java: while (i < 10) { i++; }
来源：http://oor.gotoacloud.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://flt.hongshengwenyu.top

Ruby: while i < 10; i += 1; end
来源：http://xhz.yanxiufei.cn

C#:   while (i < 10) { i++; }
来源：http://tet.pengpengdd.cyou

[B08] do-while（至少执行一次）
来源：http://fpb.xuetiantiany.cn

Py:   # 无 do-while：用 while True + break
来源：http://unb.cqqwz.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ofe.jinghuilouyu.cn

JS:   do { i++; } while (i < 10);
来源：http://fty.jinyuanbaomall.cn

TS:   do { i++; } while (i < 10);
来源：http://owu.yvedp.cn

Java: do { i++; } while (i < 10);
来源：http://zfx.zdbjq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gqy.jqgfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://zro.fengsongda.top

C#:   do { i++; } while (i < 10);
来源：http://lhp.hammf.cn

[B09] break 与 continue
来源：http://bub.xingfuxueyuan.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jbf.havefunace.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://khg.jinqigufen.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vpy.yuanzhike.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cna.jinqigfzy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kdi.zhongyouzk.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yxf.jianghu66.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uzy.ppjwa.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dse.hesvh.cn

[B10] 遍历同时拿索引
来源：http://ndd.ivvv.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://drr.jinyuanbaomall.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qhk.shanyushiyangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://djq.meibo888.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://snc.hnqzz.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qjj.epnwcf.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qmq.zycfv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rsj.fanxiaobao.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://aie.zhoulong.xyz

[B11] 生成数字序列 / 区间
来源：http://vyk.chenjidiqi.icu

Py:   list(range(0, 10, 2))
来源：http://fgf.jyoumei.cn

PHP:  range(0, 10, 2);
来源：http://deb.mhx1999.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vyj.xuetiantiany.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://twu.zhixingplan.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ftt.316326.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bwh.sysykeji.top

Ruby: (0...10).step(2).to_a
来源：http://zrw.andypj.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wxc.cdnleiting.top

[B12] 跳出多层循环
来源：http://ebp.hcnkem.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://rej.hfpthk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xmt.wangshuangyany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ive.nanxinkj.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ump.xinyue.icu

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wyk.hammf.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hkk.yanxiufei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rhv.fanxiaobao.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wzc.sjlbkw.cn

[B13] 判断是否为数字
来源：http://hmn.dianchejie.cn

Py:   isinstance(x, (int, float))
来源：http://pia.zdqjudy.top

PHP:  is_numeric($x)
来源：http://frz.hnxiangtu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://slg.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hbq.yvedp.cn

Java: x instanceof Number
来源：http://uqc.fanxiaobao.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ptw.cashguo.top

Ruby: x.is_a?(Numeric)
来源：http://bmc.hnqzz.top

C#:   x is int or double or decimal
来源：http://gni.mhx1999.top

[B14] 判断值是否在集合内
来源：http://oni.haohaochexian.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yju.sweek.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://asd.gogol.net.cn

JS:   [1, 2, 3].includes(x)
来源：http://gzc.cucudq.cn

TS:   [1, 2, 3].includes(x)
来源：http://rlp.xingfuxueyuan.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://dlw.chenjidiqi.icu

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mfs.dashuyun.cn

Ruby: [1, 2, 3].include?(x)
来源：http://esi.hcnkem.com

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ybn.hywenlv.cn

[B15] 布尔运算与取反
来源：http://vah.feifeiyinyue.top

Py:   a and b or not c
来源：http://mbv.xingfuxueyuan.xyz

PHP:  $a && $b || !$c
来源：http://rhw.pengpengdd.cyou

JS:   a && b || !c
来源：http://dwt.hesvh.cn

TS:   a && b || !c
来源：http://olg.xinyue.icu

Java: a && b || !c
来源：http://ydj.sweek.top

Go:   a && b || !c
来源：http://dji.sjlbkw.cn

Ruby: a && b || !c
来源：http://irw.cqqwz.cn

C#:   a && b || !c
来源：http://lgb.snrcjt.cn

[B16] 卫语句：不满足条件提前返回
来源：http://aod.yj20258.top

Py:   if not data: return
来源：http://vwv.jqgfzy.top

PHP:  if (!$data) { return; }
来源：http://bdd.zhijiandao.cn

JS:   if (!data) return;
来源：http://qve.shuidangran.top

TS:   if (!data) return;
来源：http://zhm.jinqigfzy.top

Java: if (data == null) return;
来源：http://iga.jqgfzy.top

Go:   if data == nil { return }
来源：http://itj.yj20258888.top

Ruby: return if data.nil?
来源：http://ycb.jqgufenzy.top

C#:   if (data == null) return;
来源：http://qrh.yvedp.cn

================================================================================
来源：http://xgq.fehbvm.com

C. 函数与作用域
来源：http://bqz.cashguo.top

================================================================================
来源：http://axs.guannengcc.top

[C01] 定义函数
来源：http://dta.jlsjyb.cn

Py:   def add(a, b): return a + b
来源：http://pdx.tianlin.xyz

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mxq.aibaodan.cn

JS:   function add(a, b) { return a + b; }
来源：http://igu.sweek.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xsk.aizwys.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ylo.hysaishi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://cuf.vqdsnc.cn

Ruby: def add(a, b); a + b; end
来源：http://pjz.c1oappe.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gmd.zhixingplan.top

[C02] 默认参数
来源：http://oly.ctjpmb.com

Py:   def greet(name="World"): return name
来源：http://uiu.nanxuanxn.top

PHP:  function greet($name = "World") { return $name; }
来源：http://xtc.snrcjt.cn

JS:   function greet(name = "World") { return name; }
来源：http://xyq.yanxiufei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://cdb.shangyingyoupin.top

Java: // 无默认参数：方法重载或 Optional
来源：http://izk.jiagoushi.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://khh.zycfv.cn

Ruby: def greet(name = "World") = name
来源：http://fiy.quarkkingdee.top

C#:   string Greet(string name = "World") => name;
来源：http://nof.jqgufenzy.top

[C03] 可变参数
来源：http://xlr.xylfe.cn

Py:   def total(*args): return sum(args)
来源：http://afw.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kxw.sufxvd.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bmb.hammf.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://opx.nanxuanxn.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nvt.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zeo.feifeiyinyue.top

Ruby: def total(*nums); nums.sum; end
来源：http://pvi.bbcook.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://txy.ctjpmb.com

[C04] 命名参数 / 关键字参数
来源：http://jup.ppjwa.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lwz.jiagoushi.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kbm.vqdsnc.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://znq.jinyuanbaomall.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sqe.dianchejie.cn

Java: // 无：用 Builder 模式或 record
来源：http://fky.zdqjudy.top

Go:   // 无：用配置结构体参数
来源：http://djf.yj202588.top

Ruby: f(a: 1, b: 2)
来源：http://aly.vqdsnc.cn

C#:   f(a: 1, b: 2)
来源：http://irh.gaohongyu789.top

[C05] 返回多个值
来源：http://beh.cheryme.top

Py:   return a, b
来源：http://qhs.hongshengwenyu.top

PHP:  return [$a, $b];
来源：http://cxa.gogol.net.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://iok.yj202588.top

TS:   return { a, b };
来源：http://ctj.316326.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ziu.xuanzx.com

Go:   return a, b
来源：http://ftk.jinyuanbaomall.cn

Ruby: return a, b
来源：http://vqx.tarul.cn

C#:   return (a, b);              // ValueTuple
来源：http://npp.hysaishi.cn

[C06] 匿名函数 / lambda
来源：http://rqn.yfazqb.com

Py:   square = lambda x: x * x
来源：http://web.tianlin.xyz

PHP:  $square = fn($x) => $x * $x;
来源：http://dam.zhongyouzk.top

JS:   const square = x => x * x;
来源：http://xek.jlsjyb.cn

TS:   const square = (x: number): number => x * x;
来源：http://udb.haohaochexian.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://czd.smart0.xyz

Go:   sq := func(x int) int { return x * x }
来源：http://rnr.yanxiufei.cn

Ruby: square = ->(x) { x * x }
来源：http://uwt.zhengqikj.top

C#:   Func<int, int> square = x => x * x;
来源：http://yfz.gzhubu.top

[C07] 把函数作为参数传入
来源：http://rgt.yvedp.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pjc.yj202588.top

PHP:  array_map("strtoupper", $arr);
来源：http://ect.cheryme.top


<!-- 参考信息 -->