代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://xvj.fktsv.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://cor.gotoacloud.top

Go:   // 单行；/* 多行 */
来源：http://spx.guannengcc.top

Ruby: # 单行；=begin 多行 =end
来源：http://nfd.shanyushiyangkeji.top

C#:   // 单行；/* 多行 */
来源：http://emr.yonumen.top

[A15] 空值判断与默认值
来源：http://zmv.nanxuanxn.top

Py:   value = data or "默认值"
来源：http://byj.yueranfly.top

PHP:  $value = $data ?? "默认值";
来源：http://kdq.yvedp.cn

JS:   const value = data ?? "默认值";
来源：http://cqg.shanyushiyangkeji.top

TS:   const value = data ?? "默认值";
来源：http://wus.gaohongyu789.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://cdx.tianlin.xyz

Go:   if data == "" { data = "默认值" }
来源：http://jfs.tianlin.xyz

Ruby: value = data || "默认值"
来源：http://exr.guowangkeji.top

C#:   var value = data ?? "默认值";
来源：http://joa.hnxiangtu.top

[A16] 真假值判断规则
来源：http://ojc.sxryk.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dwy.zhijiandao.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://fle.guannengcc.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ias.gotoacloud.top

TS:   if (!x) {}
来源：http://vbh.daxiang520.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://xff.tarul.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hrb.shangyingyoupin.top

Ruby: unless x            # nil 与 false 为假
来源：http://azm.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ooc.svipenyu.cn

[A17] 位运算
来源：http://fgr.ybcxt.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hmk.meibo888.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://oeo.xylfe.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ohg.shuidangran.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bcb.meibo888.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oca.feifeiyinyue.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ncb.yongpay.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pld.nanxuanxn.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pla.zhiwuduotai.top

[A18] 字符与 ASCII 码互转
来源：http://thm.yj202588.top

Py:   ord("A"); chr(65)
来源：http://ahu.hnxiangtu.top

PHP:  ord("A"); chr(65)
来源：http://per.zhoulong.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cbj.zhiwuduotai.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wcl.ywan-chungtsiang.top

Java: (int) 'A'; (char) 65
来源：http://usl.zhoulong.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fgz.ctjpmb.com

Ruby: "A".ord; 65.chr
来源：http://htz.nanxuanxn.top

C#:   (int)'A'; (char)65
来源：http://avs.bjfxy.top

[A19] 交换两个变量
来源：http://mav.tian-w.cn

Py:   a, b = b, a
来源：http://eka.gotoacloud.top

PHP:  [$a, $b] = [$b, $a];
来源：http://tlu.cheryme.top

JS:   [a, b] = [b, a];
来源：http://fpv.yfazqb.com

TS:   [a, b] = [b, a];
来源：http://vgh.ydjk.org.cn

Java: int t = a; a = b; b = t;
来源：http://icy.shangyingyoupin.top

Go:   a, b = b, a
来源：http://boc.52xcode.cn

Ruby: a, b = b, a
来源：http://dha.shanyushiyangkeji.top

C#:   (a, b) = (b, a);
来源：http://qfy.xuetiantiany.cn

[A20] 读取标准输入
来源：http://ulg.hywenlv.cn

Py:   name = input("请输入：")
来源：http://zfq.shanyushiyangkeji.top

PHP:  $name = trim(fgets(STDIN));
来源：http://gcq.yuxming.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dgy.yonumen.top

TS:   // Node.js：readline 模块
来源：http://itx.yonumen.top

Java: new Scanner(System.in).nextLine()
来源：http://shi.ehwqpu.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lww.yj20258.top

Ruby: gets.chomp
来源：http://khp.jqgufenzy.top

C#:   Console.ReadLine();
来源：http://fcv.xinyue.icu

[A21] 保留指定小数位输出
来源：http://mpu.cucudq.cn

Py:   f"{3.14159:.2f}"
来源：http://jar.fktsv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vaz.fktsv.cn

JS:   (3.14159).toFixed(2)
来源：http://jpr.wangdashe.top

TS:   (3.14159).toFixed(2)
来源：http://dyp.andypj.xyz

Java: String.format("%.2f", 3.14159)
来源：http://ild.pengpengdd.cyou

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://eho.bjfxy.top

Ruby: format("%.2f", 3.14159)
来源：http://qdl.bbcook.cn

C#:   3.14159.ToString("F2")
来源：http://lhy.hesvh.cn

[A22] 获取字符串长度
来源：http://gdy.yj20258888.top

Py:   len(s)
来源：http://soq.shanyushiyangtech.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kcl.birdmap.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nws.jinyuanbaomall.cn

TS:   s.length
来源：http://eld.guannengcc.top

Java: s.length()
来源：http://mqr.smart0.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://gfp.jqgfzy.top

Ruby: s.length
来源：http://sal.yuanzhike.top

C#:   s.Length
来源：http://umy.xylfe.cn

[A23] 大小写转换
来源：http://yyp.xingfuxueyuan.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://uop.smart0.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mrw.gogol.net.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://con.fanxiaobao.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ybc.fanxiaobao.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jcx.pengpengdd.cyou

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vak.sysykeji.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://liu.zhiwuduotai.top

C#:   s.ToUpper(); s.ToLower()
来源：http://jfb.shangyingyoupin.top

[A24] 去除首尾空白
来源：http://xrw.jlsjyb.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vli.havefunace.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dve.guowangkeji.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://okp.chenjidiqi.icu

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gxh.hnqzz.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zpb.yongpay.top

Go:   strings.TrimSpace(s)
来源：http://ozi.cqqwz.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vzs.dashuyun.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://skw.hcnkem.com

[A25] 字符串比较
来源：http://wos.yj20258888.top

Py:   s1 == s2; s1 != s2
来源：http://jjx.guannengcc.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://krs.xylfe.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ajp.9152youxi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ymk.wangshuangyany.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://akx.wangshuangyany.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://dmz.tanke756.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ipj.fengsongda.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://arf.yfazqb.com

[A26] 类型转换总览
来源：http://azl.yonumen.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wzz.zhengqikj.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ftp.gzhubu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://nsw.vqdsnc.cn

TS:   Number() String() Boolean() x as number
来源：http://npu.jqgfzy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kmh.wangshuangyany.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qgs.9152youxi.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://lyz.haohaochexian.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://enf.cqqwz.cn

================================================================================
来源：http://vbq.zhoulong.xyz

B. 流程控制
来源：http://pox.c1oappe.top

================================================================================
来源：http://wjq.fktsv.cn

[B01] 条件判断 if / else
来源：http://ewz.hysaishi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://der.aibaodan.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yli.ivvv.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wmf.hfpthk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zjv.fehbvm.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://lty.dianchejie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://alm.jlsjyb.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bjr.wangdashe.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://bkr.iojbl.cn

[B02] 多分支 else if / elif
来源：http://clv.hesvh.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ofe.jqgfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://pxk.iojbl.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ovb.fehbvm.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yev.redwolf501.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lev.uphjek.com

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eec.xinyue.icu

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oft.cqqwz.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pxf.zycfv.cn

[B03] switch / match / case
来源：http://urc.tianlin.xyz

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dlw.birdmap.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ykh.yj20258888.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jns.yonumen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://iuv.vqdsnc.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xoj.yangfankeji.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cij.nwbrower.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zqb.zhiwuduotai.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tnx.yj20258888.top

[B04] for 计数循环
来源：http://tmt.sweek.top

Py:   for i in range(10): print(i)
来源：http://otu.hcnkem.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://vog.ehwqpu.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://apd.jianghu66.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mly.yj202588.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tvq.quarkkingdee.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lvb.fengsongda.top

Ruby: 10.times { |i| puts i }
来源：http://cvb.chenzaomai.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://yks.meibo888.top

[B05] 遍历数组 / 列表
来源：http://dms.hnqzz.top

Py:   for item in arr: print(item)
来源：http://meg.birdmap.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://zse.wangshuangyany.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://kht.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://htq.guannengcc.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://cza.gotoacloud.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gnp.tanke756.top

Ruby: arr.each { |item| puts item }
来源：http://nvr.zhixingplan.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://sac.xuetiantiany.cn

[B06] 遍历字典 / 对象
来源：http://ojp.hysaishi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://iqm.zhixingplan.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kxd.sufxvd.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wnr.hesvh.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://lzy.yonumen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aqj.ivvv.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://blv.vehdjk.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rbg.bbcook.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bng.yanxiufei.cn

[B07] while 循环
来源：http://mma.sxryk.cn

Py:   while i < 10: i += 1
来源：http://pso.smart0.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://gic.ybcxt.top

JS:   while (i < 10) { i++; }
来源：http://pdz.jianghu66.top

TS:   while (i < 10) { i++; }
来源：http://nii.jqgufenzy.top

Java: while (i < 10) { i++; }
来源：http://zki.dashuyun.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://rxu.cashguo.top

Ruby: while i < 10; i += 1; end
来源：http://mim.fengsongda.top

C#:   while (i < 10) { i++; }
来源：http://ehw.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://zmb.hfpthk.cn

Py:   # 无 do-while：用 while True + break
来源：http://sbp.shangyingyoupin.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kbk.jqgufenzy.top

JS:   do { i++; } while (i < 10);
来源：http://wgt.jinqigufen.top

TS:   do { i++; } while (i < 10);
来源：http://nsa.yvedp.cn

Java: do { i++; } while (i < 10);
来源：http://jck.mhx1999.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hgx.xylfe.cn

Ruby: begin; i += 1; end while i < 10
来源：http://wbn.yfazqb.com

C#:   do { i++; } while (i < 10);
来源：http://ndm.tanke756.top

[B09] break 与 continue
来源：http://gsw.jinyuanbaomall.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hhh.hnxiangtu.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tdk.cqqwz.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cqh.gzhubu.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://edk.andypj.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wyn.hongshengwenyu.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://yyt.cdnleiting.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://lzc.gotoacloud.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://azk.xylfe.cn

[B10] 遍历同时拿索引
来源：http://pen.vehdjk.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://okm.jinqigufen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://dpk.hammf.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://msb.shzxlz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://kxk.0kj1m.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://iiq.feifeiyinyue.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nue.ybcxt.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://gwk.sjlbkw.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://scr.fktsv.cn

[B11] 生成数字序列 / 区间
来源：http://sdt.ivvv.top

Py:   list(range(0, 10, 2))
来源：http://lbq.fktsv.cn

PHP:  range(0, 10, 2);
来源：http://pdq.cqqwz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yzm.redwolf501.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vxa.iojbl.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://aaj.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zqz.jlsjyb.cn

Ruby: (0...10).step(2).to_a
来源：http://luw.cqqwz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://onl.cdnleiting.top

[B12] 跳出多层循环
来源：http://ulv.sysykeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://yjv.tian-w.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://gni.meibo888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xhj.ppjwa.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://saz.tianlin.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vsl.jinqigfzy.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ekl.guowangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://pzo.tian-w.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ndg.chenzaomai.com

[B13] 判断是否为数字
来源：http://zop.xinyue.icu

Py:   isinstance(x, (int, float))
来源：http://kzh.xylfe.cn

PHP:  is_numeric($x)
来源：http://sul.ywan-chungtsiang.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qaw.tian-w.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dio.jinghuilouyu.cn

Java: x instanceof Number
来源：http://vch.dashuyun.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hyt.ctjpmb.com

Ruby: x.is_a?(Numeric)
来源：http://ehw.gogol.net.cn

C#:   x is int or double or decimal
来源：http://eun.jqgufenzy.top

[B14] 判断值是否在集合内
来源：http://xxm.gaohongyu789.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yru.c1oappe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://atx.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://qwf.jinghuilouyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://txz.0kj1m.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qcm.yangfankeji.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jgu.nanxuanxn.top

Ruby: [1, 2, 3].include?(x)
来源：http://gdt.wangdashe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kqr.aizwys.cn

[B15] 布尔运算与取反
来源：http://hkv.bbcook.cn

Py:   a and b or not c
来源：http://bkm.xinyue.icu

PHP:  $a && $b || !$c
来源：http://dkf.fzhhl.top

JS:   a && b || !c
来源：http://cnn.daxiang520.top

TS:   a && b || !c
来源：http://exl.wangdashe.top

Java: a && b || !c
来源：http://sgs.dianchejie.cn

Go:   a && b || !c
来源：http://gpp.fzhhl.top

Ruby: a && b || !c
来源：http://obc.wangshuangyany.cn

C#:   a && b || !c
来源：http://hbx.zhongyouzk.top

[B16] 卫语句：不满足条件提前返回
来源：http://fli.cqqwz.cn

Py:   if not data: return
来源：http://mfd.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://fyx.iojbl.cn

JS:   if (!data) return;
来源：http://tya.zhongyouzk.top

TS:   if (!data) return;
来源：http://orr.pycfn.com

Java: if (data == null) return;
来源：http://yia.kuanghao11.cn

Go:   if data == nil { return }
来源：http://vyq.pycfn.com

Ruby: return if data.nil?
来源：http://zbq.ivvv.top

C#:   if (data == null) return;
来源：http://bqk.hcnkem.com

================================================================================
来源：http://jjj.pengpengdd.cyou

C. 函数与作用域
来源：http://qwx.quarkkingdee.top

================================================================================
来源：http://dze.sufxvd.cn

[C01] 定义函数
来源：http://wxz.hesvh.cn

Py:   def add(a, b): return a + b
来源：http://lzl.hfpthk.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://otb.sjlbkw.cn

JS:   function add(a, b) { return a + b; }
来源：http://qdm.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fjf.c1oappe.top

Java: static int add(int a, int b) { return a + b; }
来源：http://bhu.52xcode.cn

Go:   func add(a, b int) int { return a + b }
来源：http://crk.haohaochexian.top

Ruby: def add(a, b); a + b; end
来源：http://pbl.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wod.sysykeji.top

[C02] 默认参数
来源：http://yyy.xziqi.cn

Py:   def greet(name="World"): return name
来源：http://czf.jinyuanbaomall.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://aul.jinyuanbaomall.cn

JS:   function greet(name = "World") { return name; }
来源：http://iig.xinyue.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://bub.cucudq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pmg.gzhubu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vrl.bjfxy.top

Ruby: def greet(name = "World") = name
来源：http://ihy.9152youxi.cn

C#:   string Greet(string name = "World") => name;
来源：http://nsv.aibaodan.cn

[C03] 可变参数
来源：http://djn.yfazqb.com

Py:   def total(*args): return sum(args)
来源：http://rou.birdmap.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vdn.fanxiaobao.xyz

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ull.chenzaomai.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://txy.andypj.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://nct.gogol.net.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ntd.jiagoushi.top

Ruby: def total(*nums); nums.sum; end
来源：http://jin.hammf.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://edg.0kj1m.cn

[C04] 命名参数 / 关键字参数
来源：http://rku.yangfankeji.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dqy.zycfv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xhj.aizwys.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lug.yongpay.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xkp.316326.xyz

Java: // 无：用 Builder 模式或 record
来源：http://ynu.yanxiufei.cn

Go:   // 无：用配置结构体参数
来源：http://fhb.mhx1999.top

Ruby: f(a: 1, b: 2)
来源：http://gta.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://hmp.nwbrower.top

[C05] 返回多个值
来源：http://hgt.zdbjq.cn


<!-- 参考信息 -->