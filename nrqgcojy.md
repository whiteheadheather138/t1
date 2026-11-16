代发 wailian999

[A14] 注释写法
来源：http://epf.jinyuanbaomall.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://jnd.jianghu66.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://wzd.xuanzx.com

JS:   // 单行；/* 多行 */
来源：http://lcy.zhijiandao.cn

TS:   // 单行；/* 多行 */
来源：http://kmy.sweek.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://uym.gotoacloud.top

Go:   // 单行；/* 多行 */
来源：http://pfj.jinqigufen.top

Ruby: # 单行；=begin 多行 =end
来源：http://add.haohaochexian.top

C#:   // 单行；/* 多行 */
来源：http://qmw.chenjidiqi.icu

[A15] 空值判断与默认值
来源：http://xzo.ydzc1.top

Py:   value = data or "默认值"
来源：http://cdv.fengsongda.top

PHP:  $value = $data ?? "默认值";
来源：http://jfw.bjfxy.top

JS:   const value = data ?? "默认值";
来源：http://xis.tian-w.cn

TS:   const value = data ?? "默认值";
来源：http://pol.sxryk.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://yog.shzxlz.cn

Go:   if data == "" { data = "默认值" }
来源：http://rbc.epnwcf.com

Ruby: value = data || "默认值"
来源：http://xhn.gzhubu.top

C#:   var value = data ?? "默认值";
来源：http://jiy.smart0.xyz

[A16] 真假值判断规则
来源：http://kqo.316326.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qqc.yuxming.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xhq.ppjwa.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://igs.sysykeji.top

TS:   if (!x) {}
来源：http://npf.sufxvd.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://yxi.yonumen.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://msi.yonumen.top

Ruby: unless x            # nil 与 false 为假
来源：http://rbj.yj20258888.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sth.vehdjk.com

[A17] 位运算
来源：http://qld.xuetiantiany.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hen.yj202588.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://yys.daria6918.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wmd.shangyingyoupin.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://dnv.9152youxi.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hkg.hnxiangtu.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mab.fengsongda.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aim.cucudq.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uci.dashuyun.cn

[A18] 字符与 ASCII 码互转
来源：http://pkm.xuanzx.com

Py:   ord("A"); chr(65)
来源：http://jqu.guowangkeji.top

PHP:  ord("A"); chr(65)
来源：http://hui.jiagoushi.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jhr.sweek.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jft.shanyushiyangtech.top

Java: (int) 'A'; (char) 65
来源：http://xve.yangfankeji.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qzz.cashguo.top

Ruby: "A".ord; 65.chr
来源：http://ifb.hnxiangtu.top

C#:   (int)'A'; (char)65
来源：http://vws.andypj.xyz

[A19] 交换两个变量
来源：http://ibo.nwbrower.top

Py:   a, b = b, a
来源：http://pcq.snrcjt.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://inn.hammf.cn

JS:   [a, b] = [b, a];
来源：http://sfa.cqqwz.cn

TS:   [a, b] = [b, a];
来源：http://ode.yanxiufei.cn

Java: int t = a; a = b; b = t;
来源：http://fww.hfpthk.cn

Go:   a, b = b, a
来源：http://haq.hammf.cn

Ruby: a, b = b, a
来源：http://aze.uphjek.com

C#:   (a, b) = (b, a);
来源：http://uut.gaohongyu789.top

[A20] 读取标准输入
来源：http://ghs.yonumen.top

Py:   name = input("请输入：")
来源：http://btx.sufxvd.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://oew.shanyushiyangtech.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qnd.andypj.xyz

TS:   // Node.js：readline 模块
来源：http://klp.ydjk.org.cn

Java: new Scanner(System.in).nextLine()
来源：http://hul.ehwqpu.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ivt.redwolf501.top

Ruby: gets.chomp
来源：http://fcz.andypj.xyz

C#:   Console.ReadLine();
来源：http://zef.vehdjk.com

[A21] 保留指定小数位输出
来源：http://kok.ybcxt.top

Py:   f"{3.14159:.2f}"
来源：http://two.wangshuangyany.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xbg.zhijiandao.cn

JS:   (3.14159).toFixed(2)
来源：http://zjn.316326.xyz

TS:   (3.14159).toFixed(2)
来源：http://rmu.dashuyun.cn

Java: String.format("%.2f", 3.14159)
来源：http://psv.nwbrower.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vui.bjfxy.top

Ruby: format("%.2f", 3.14159)
来源：http://jij.shanyushiyangkeji.top

C#:   3.14159.ToString("F2")
来源：http://zcz.jinyuanbaomall.cn

[A22] 获取字符串长度
来源：http://hmf.sxryk.cn

Py:   len(s)
来源：http://nsp.vqdsnc.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://lbo.hfpthk.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ubk.cdnleiting.top

TS:   s.length
来源：http://stw.ivvv.top

Java: s.length()
来源：http://qze.tarul.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hdt.yuxming.cn

Ruby: s.length
来源：http://ajn.yangfankeji.com

C#:   s.Length
来源：http://dqk.jlsjyb.cn

[A23] 大小写转换
来源：http://pon.kuanghao11.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://tuk.jinyuanbaomall.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fad.cheryme.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://jgg.haohaochexian.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hag.andypj.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zue.jqgfzy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hxd.yuanzhike.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://iqp.kuanghao11.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hei.epnwcf.com

[A24] 去除首尾空白
来源：http://lxp.fehbvm.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vgr.feifeiyinyue.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xvc.jqgfzy.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gqj.0kj1m.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qlf.ehwqpu.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ksw.wangdashe.top

Go:   strings.TrimSpace(s)
来源：http://aiu.nanxinkj.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ews.quarkkingdee.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://czn.yonumen.top

[A25] 字符串比较
来源：http://uzd.hfpthk.cn

Py:   s1 == s2; s1 != s2
来源：http://one.jqgfzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gus.xziqi.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://umb.cashguo.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lvd.iojbl.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kbi.guannengcc.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hcj.cashguo.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ptv.52xcode.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kzt.chenjidiqi.icu

[A26] 类型转换总览
来源：http://fah.quarkkingdee.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ory.tanke756.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tkh.gzhubu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tbf.hammf.cn

TS:   Number() String() Boolean() x as number
来源：http://ugn.hesvh.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://sra.cucudq.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://buk.guannengcc.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://gxk.jyoumei.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://cbf.316326.xyz

================================================================================
来源：http://iwt.yuxming.cn

B. 流程控制
来源：http://cxu.vehdjk.com

================================================================================
来源：http://kyg.xuetiantiany.cn

[B01] 条件判断 if / else
来源：http://qqu.xinyue.icu

Py:   result = "正" if x > 0 else "非正"
来源：http://tki.kuanghao11.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oah.yfazqb.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gmc.fehbvm.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://asa.jiagoushi.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://fcd.xinyue.icu

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hqz.kuanghao11.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://shg.bjfxy.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lxq.hnxiangtu.top

[B02] 多分支 else if / elif
来源：http://jgu.ybcxt.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lib.iojbl.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kwk.haohaochexian.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iqx.iojbl.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xns.tarul.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ftf.vehdjk.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dke.epnwcf.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://azc.dianchejie.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hdv.vqdsnc.cn

[B03] switch / match / case
来源：http://swf.daria6918.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://juw.aizwys.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://msk.daxiang520.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dxj.aizwys.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iba.snrcjt.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://zin.sweek.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://eji.sufxvd.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ypn.fzhhl.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://idl.c1oappe.top

[B04] for 计数循环
来源：http://sfj.sweek.top

Py:   for i in range(10): print(i)
来源：http://yok.yanxiufei.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gfq.9152youxi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wbx.quarkkingdee.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qgb.hysaishi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tau.cucudq.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ing.yfazqb.com

Ruby: 10.times { |i| puts i }
来源：http://zhd.nwbrower.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mgw.chenjidiqi.icu

[B05] 遍历数组 / 列表
来源：http://raq.jyoumei.cn

Py:   for item in arr: print(item)
来源：http://wbg.yfazqb.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://sdf.pengpengdd.cyou

JS:   for (const item of arr) { console.log(item); }
来源：http://qew.zhijiandao.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://jod.fzhhl.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zvk.sxryk.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ekm.yj20258.top

Ruby: arr.each { |item| puts item }
来源：http://pel.redwolf501.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hgk.gogol.net.cn

[B06] 遍历字典 / 对象
来源：http://unm.hongshengwenyu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yhl.bjfxy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zul.cashguo.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kus.meibo888.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ykn.jqgfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vkz.yj20258888.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://skt.xziqi.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://bxt.nanxinkj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://yjw.jyoumei.cn

[B07] while 循环
来源：http://wok.feifeiyinyue.top

Py:   while i < 10: i += 1
来源：http://fzr.xziqi.cn

PHP:  while ($i < 10) { $i++; }
来源：http://oix.zycfv.cn

JS:   while (i < 10) { i++; }
来源：http://nvf.jiagoushi.top

TS:   while (i < 10) { i++; }
来源：http://xza.meibo888.top

Java: while (i < 10) { i++; }
来源：http://ngj.jinqigfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://lbu.dianchejie.cn

Ruby: while i < 10; i += 1; end
来源：http://glh.sjlbkw.cn

C#:   while (i < 10) { i++; }
来源：http://xik.sweek.top

[B08] do-while（至少执行一次）
来源：http://tmc.shanyushiyangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://mcz.chenjidiqi.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://wmf.vehdjk.com

JS:   do { i++; } while (i < 10);
来源：http://jar.zhijiandao.cn

TS:   do { i++; } while (i < 10);
来源：http://heu.sweek.top

Java: do { i++; } while (i < 10);
来源：http://zeb.nanxuanxn.top

Go:   for { i++; if i >= 10 { break } }
来源：http://qku.ybcxt.top

Ruby: begin; i += 1; end while i < 10
来源：http://mtx.smart0.xyz

C#:   do { i++; } while (i < 10);
来源：http://gjv.yonumen.top

[B09] break 与 continue
来源：http://lze.wangdashe.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ssd.jinqigufen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tec.cdnleiting.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hys.zhoulong.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rth.meibo888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uif.zhijiandao.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jgy.zhoulong.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://cnh.jinghuilouyu.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rmz.nanxinkj.top

[B10] 遍历同时拿索引
来源：http://bsm.fanxiaobao.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://rux.havefunace.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ijg.shanyushiyangkeji.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gwh.yueranfly.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ajh.hnxiangtu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://utp.yvedp.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qjf.cashguo.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://egu.jinyuanbaomall.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ndu.shanyushiyangkeji.top

[B11] 生成数字序列 / 区间
来源：http://pkc.ivvv.top

Py:   list(range(0, 10, 2))
来源：http://cwi.bbcook.cn

PHP:  range(0, 10, 2);
来源：http://pds.0kj1m.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mxz.hysaishi.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xqb.jianghu66.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ehx.daria6918.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bnu.xziqi.cn

Ruby: (0...10).step(2).to_a
来源：http://ony.jinghuilouyu.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nfj.uphjek.com

[B12] 跳出多层循环
来源：http://ypr.fehbvm.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://gkn.fktsv.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://xkl.tanke756.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ftb.yfazqb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bsu.andypj.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://qkc.yueranfly.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fkn.jqgufenzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://xgh.tanke756.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ifl.zycfv.cn

[B13] 判断是否为数字
来源：http://lvw.bbcook.cn

Py:   isinstance(x, (int, float))
来源：http://zim.sysykeji.top

PHP:  is_numeric($x)
来源：http://hoj.vqdsnc.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jdr.jinghuilouyu.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://unv.jinghuilouyu.cn

Java: x instanceof Number
来源：http://ufw.yj20258888.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cjm.sweek.top

Ruby: x.is_a?(Numeric)
来源：http://csv.hcnkem.com

C#:   x is int or double or decimal
来源：http://dnu.316326.xyz

[B14] 判断值是否在集合内
来源：http://oxz.0kj1m.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://uog.yj20258.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gsy.xuetiantiany.cn

JS:   [1, 2, 3].includes(x)
来源：http://wnj.yuanzhike.top

TS:   [1, 2, 3].includes(x)
来源：http://mfp.ehwqpu.com

Java: List.of(1, 2, 3).contains(x)
来源：http://jwk.kuanghao11.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dlz.yongpay.top

Ruby: [1, 2, 3].include?(x)
来源：http://nyy.jqgfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iyf.nwbrower.top

[B15] 布尔运算与取反
来源：http://vsz.gogol.net.cn

Py:   a and b or not c
来源：http://jkl.cqqwz.cn

PHP:  $a && $b || !$c
来源：http://irk.52xcode.cn

JS:   a && b || !c
来源：http://rgq.smart0.xyz

TS:   a && b || !c
来源：http://erz.zhiwuduotai.top

Java: a && b || !c
来源：http://tvs.9152youxi.cn

Go:   a && b || !c
来源：http://vdh.smart0.xyz

Ruby: a && b || !c
来源：http://dqq.daria6918.cn

C#:   a && b || !c
来源：http://ryt.mhx1999.top

[B16] 卫语句：不满足条件提前返回
来源：http://sds.vehdjk.com

Py:   if not data: return
来源：http://moz.meibo888.top

PHP:  if (!$data) { return; }
来源：http://uuz.fktsv.cn

JS:   if (!data) return;
来源：http://nip.hammf.cn

TS:   if (!data) return;
来源：http://eti.zhixingplan.top

Java: if (data == null) return;
来源：http://haz.wangdashe.top

Go:   if data == nil { return }
来源：http://uym.xziqi.cn

Ruby: return if data.nil?
来源：http://cov.jinqigfzy.top

C#:   if (data == null) return;
来源：http://tgb.hcnkem.com

================================================================================
来源：http://fdw.ppjwa.cn

C. 函数与作用域
来源：http://yov.meibo888.top

================================================================================
来源：http://kxs.xinyue.icu

[C01] 定义函数
来源：http://jcu.wangdashe.top

Py:   def add(a, b): return a + b
来源：http://gcc.vqdsnc.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kyc.chenzaomai.com

JS:   function add(a, b) { return a + b; }
来源：http://mjq.nanxinkj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ouy.tarul.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://cuo.gotoacloud.top

Go:   func add(a, b int) int { return a + b }
来源：http://exw.yonumen.top

Ruby: def add(a, b); a + b; end
来源：http://avq.52xcode.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://qjf.yongpay.top

[C02] 默认参数
来源：http://pfw.yangfankeji.com

Py:   def greet(name="World"): return name
来源：http://san.hesvh.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://qwh.sxryk.cn

JS:   function greet(name = "World") { return name; }
来源：http://eqf.chenlongwang.top

TS:   function greet(name: string = "World") { return name; }
来源：http://vxu.hammf.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ydj.yanxiufei.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jsk.cashguo.top

Ruby: def greet(name = "World") = name
来源：http://qbn.gzhubu.top

C#:   string Greet(string name = "World") => name;
来源：http://hwh.epnwcf.com

[C03] 可变参数
来源：http://ixq.jqgufenzy.top

Py:   def total(*args): return sum(args)
来源：http://txa.chenlongwang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hba.jyoumei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lge.pengpengdd.cyou

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://lpa.yonumen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jmm.aibaodan.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ihi.xuetiantiany.cn

Ruby: def total(*nums); nums.sum; end
来源：http://woc.meibo888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://iwx.gotoacloud.top

[C04] 命名参数 / 关键字参数
来源：http://gzo.sysykeji.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hdh.smart0.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jhu.zhengqikj.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ysm.aibaodan.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sme.tianlin.xyz

Java: // 无：用 Builder 模式或 record
来源：http://vxs.tianlin.xyz


<!-- 参考信息 -->