代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://vkp.guannengcc.top

[A15] 空值判断与默认值
来源：http://isn.sufxvd.cn

Py:   value = data or "默认值"
来源：http://sqp.hesvh.cn

PHP:  $value = $data ?? "默认值";
来源：http://caw.zhoulong.xyz

JS:   const value = data ?? "默认值";
来源：http://xwu.svipenyu.cn

TS:   const value = data ?? "默认值";
来源：http://cjz.birdmap.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://umy.shuidangran.top

Go:   if data == "" { data = "默认值" }
来源：http://orf.wangshuangyany.cn

Ruby: value = data || "默认值"
来源：http://ifc.zhiwuduotai.top

C#:   var value = data ?? "默认值";
来源：http://nis.havefunace.top

[A16] 真假值判断规则
来源：http://axj.hnqzz.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dbg.aibaodan.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://odm.tian-w.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://acp.hammf.cn

TS:   if (!x) {}
来源：http://rko.redwolf501.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fiz.chenzaomai.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://flt.cashguo.top

Ruby: unless x            # nil 与 false 为假
来源：http://wug.zhixingplan.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zhy.mhx1999.top

[A17] 位运算
来源：http://eja.gzhubu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qvn.xylfe.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mnj.guannengcc.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jjd.hnqzz.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uyo.zhiwuduotai.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dwd.snrcjt.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ygk.wangdashe.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xgg.yj20258888.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bbg.gzhubu.top

[A18] 字符与 ASCII 码互转
来源：http://xnr.ydzc1.top

Py:   ord("A"); chr(65)
来源：http://xge.52xcode.cn

PHP:  ord("A"); chr(65)
来源：http://vgp.yueranfly.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ptt.jianghu66.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qdx.xuetiantiany.cn

Java: (int) 'A'; (char) 65
来源：http://qkh.sweek.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hnd.xinyue.icu

Ruby: "A".ord; 65.chr
来源：http://uxl.cdnleiting.top

C#:   (int)'A'; (char)65
来源：http://ryu.dianchejie.cn

[A19] 交换两个变量
来源：http://oas.sufxvd.cn

Py:   a, b = b, a
来源：http://ogc.zhoulong.xyz

PHP:  [$a, $b] = [$b, $a];
来源：http://jph.pycfn.com

JS:   [a, b] = [b, a];
来源：http://zqb.fanxiaobao.xyz

TS:   [a, b] = [b, a];
来源：http://xtc.tianlin.xyz

Java: int t = a; a = b; b = t;
来源：http://rts.shangyingyoupin.top

Go:   a, b = b, a
来源：http://gij.chenjidiqi.icu

Ruby: a, b = b, a
来源：http://qsa.ydzc1.top

C#:   (a, b) = (b, a);
来源：http://qov.yj202588.top

[A20] 读取标准输入
来源：http://mgk.jqgufenzy.top

Py:   name = input("请输入：")
来源：http://nyj.cqqwz.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://kns.zdqjudy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://lmt.sysykeji.top

TS:   // Node.js：readline 模块
来源：http://acb.yongpay.top

Java: new Scanner(System.in).nextLine()
来源：http://cgl.havefunace.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kep.shuidangran.top

Ruby: gets.chomp
来源：http://kfx.xuanzx.com

C#:   Console.ReadLine();
来源：http://edh.yvedp.cn

[A21] 保留指定小数位输出
来源：http://xeu.vehdjk.com

Py:   f"{3.14159:.2f}"
来源：http://vir.iojbl.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ynk.smart0.xyz

JS:   (3.14159).toFixed(2)
来源：http://syd.meibo888.top

TS:   (3.14159).toFixed(2)
来源：http://nym.jlsjyb.cn

Java: String.format("%.2f", 3.14159)
来源：http://yjo.jlsjyb.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://syu.shzxlz.cn

Ruby: format("%.2f", 3.14159)
来源：http://nmh.xylfe.cn

C#:   3.14159.ToString("F2")
来源：http://bof.aizwys.cn

[A22] 获取字符串长度
来源：http://pnf.yj202588.top

Py:   len(s)
来源：http://prn.svipenyu.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mqs.ctjpmb.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xbh.hammf.cn

TS:   s.length
来源：http://mwe.ivvv.top

Java: s.length()
来源：http://mss.bjfxy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://tiw.hnqzz.top

Ruby: s.length
来源：http://ttv.zycfv.cn

C#:   s.Length
来源：http://yqz.fehbvm.com

[A23] 大小写转换
来源：http://qgb.aizwys.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pds.svipenyu.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ofn.hammf.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wfe.guowangkeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://sga.gogol.net.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://idv.dianchejie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ahj.316326.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vtc.fktsv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://wxz.hnqzz.top

[A24] 去除首尾空白
来源：http://lox.jinqigfzy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ojz.zhijiandao.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://shd.hnqzz.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eba.hfpthk.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://svk.nwbrower.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://nai.ivvv.top

Go:   strings.TrimSpace(s)
来源：http://dtu.hysaishi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dxl.haohaochexian.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://cis.yfazqb.com

[A25] 字符串比较
来源：http://sed.xinyue.icu

Py:   s1 == s2; s1 != s2
来源：http://mln.ehwqpu.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jqq.yfazqb.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fwi.gogol.net.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://txd.nwbrower.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ywk.hnxiangtu.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://xug.xingfuxueyuan.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://thn.jinqigufen.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://dxg.ivvv.top

[A26] 类型转换总览
来源：http://ybi.xuanzx.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://llx.hongshengwenyu.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://psu.iojbl.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://prd.nanxinkj.top

TS:   Number() String() Boolean() x as number
来源：http://qca.fehbvm.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rvf.cqqwz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://sgb.zhengqikj.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://nvg.fengsongda.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://pzp.ppjwa.cn

================================================================================
来源：http://zia.daxiang520.top

B. 流程控制
来源：http://wkc.tanke756.top

================================================================================
来源：http://mcl.fehbvm.com

[B01] 条件判断 if / else
来源：http://dga.xziqi.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://crd.jinqigufen.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ulg.chenzaomai.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gmx.ydzc1.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tot.chenlongwang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ged.yj202588.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://pnl.wangshuangyany.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://zap.ybcxt.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://btq.sysykeji.top

[B02] 多分支 else if / elif
来源：http://efj.zhengqikj.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vkb.chenjidiqi.icu

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wyt.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ogk.hcnkem.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cic.bjfxy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uck.zdbjq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://msh.daria6918.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pgx.wangshuangyany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dqm.meibo888.top

[B03] switch / match / case
来源：http://jes.yvedp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mgn.shzxlz.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xls.xylfe.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bry.epnwcf.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://kxn.nwbrower.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yfn.tian-w.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hli.52xcode.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dih.haohaochexian.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nug.hcnkem.com

[B04] for 计数循环
来源：http://goy.snrcjt.cn

Py:   for i in range(10): print(i)
来源：http://dnj.daria6918.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hie.gaohongyu789.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iob.jianghu66.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://oag.xylfe.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eha.wangshuangyany.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zcn.nanxuanxn.top

Ruby: 10.times { |i| puts i }
来源：http://rfh.guannengcc.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ugr.svipenyu.cn

[B05] 遍历数组 / 列表
来源：http://uqe.cdnleiting.top

Py:   for item in arr: print(item)
来源：http://mjv.snrcjt.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hrk.uphjek.com

JS:   for (const item of arr) { console.log(item); }
来源：http://fep.yanxiufei.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://rnw.guowangkeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://xiq.yuanzhike.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zog.hywenlv.cn

Ruby: arr.each { |item| puts item }
来源：http://ubp.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://afv.jqgufenzy.top

[B06] 遍历字典 / 对象
来源：http://xqi.uphjek.com

Py:   for k, v in d.items(): print(k, v)
来源：http://vzz.svipenyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zif.bjfxy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vnc.nwbrower.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wbk.ivvv.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ahp.xingfuxueyuan.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://unf.tarul.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wkq.ehwqpu.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://gha.jinqigufen.top

[B07] while 循环
来源：http://rvr.xinyue.icu

Py:   while i < 10: i += 1
来源：http://pba.316326.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://ewd.shzxlz.cn

JS:   while (i < 10) { i++; }
来源：http://lju.ctjpmb.com

TS:   while (i < 10) { i++; }
来源：http://btc.iojbl.cn

Java: while (i < 10) { i++; }
来源：http://ega.yangfankeji.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://djm.jinyuanbaomall.cn

Ruby: while i < 10; i += 1; end
来源：http://pse.guowangkeji.top

C#:   while (i < 10) { i++; }
来源：http://yfs.52xcode.cn

[B08] do-while（至少执行一次）
来源：http://viy.yongpay.top

Py:   # 无 do-while：用 while True + break
来源：http://xqn.sysykeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://hbq.jyoumei.cn

JS:   do { i++; } while (i < 10);
来源：http://hfo.mhx1999.top

TS:   do { i++; } while (i < 10);
来源：http://wid.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://dva.zhixingplan.top

Go:   for { i++; if i >= 10 { break } }
来源：http://srp.yonumen.top

Ruby: begin; i += 1; end while i < 10
来源：http://piz.jqgufenzy.top

C#:   do { i++; } while (i < 10);
来源：http://rxl.52xcode.cn

[B09] break 与 continue
来源：http://gop.sufxvd.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hru.ivvv.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ohy.tian-w.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://syh.gogol.net.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ofk.fengsongda.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://spl.shuidangran.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wbl.gogol.net.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jxn.fengsongda.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qbv.gzhubu.top

[B10] 遍历同时拿索引
来源：http://jkx.jqgufenzy.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://itn.yongpay.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://zzh.daxiang520.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wsu.epnwcf.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mxv.havefunace.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yiy.zdbjq.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ood.fzhhl.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ljm.havefunace.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hwr.fanxiaobao.xyz

[B11] 生成数字序列 / 区间
来源：http://pqt.zhengqikj.top

Py:   list(range(0, 10, 2))
来源：http://zfk.jinghuilouyu.cn

PHP:  range(0, 10, 2);
来源：http://wtz.xuanzx.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://krx.tanke756.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fcr.cheryme.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dhh.cucudq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://agv.gaohongyu789.top

Ruby: (0...10).step(2).to_a
来源：http://rqs.daxiang520.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nsz.mhx1999.top

[B12] 跳出多层循环
来源：http://qsb.tianlin.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://ijs.sysykeji.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fpp.cheryme.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zpz.cdnleiting.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://xbt.jyoumei.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://uvg.jinqigufen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ltx.gzhubu.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yhc.smart0.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://krq.ydzc1.top

[B13] 判断是否为数字
来源：http://tcw.epnwcf.com

Py:   isinstance(x, (int, float))
来源：http://nub.yongpay.top

PHP:  is_numeric($x)
来源：http://snf.cqqwz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://tad.birdmap.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lco.chenjidiqi.icu

Java: x instanceof Number
来源：http://spx.aibaodan.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://pya.xziqi.cn

Ruby: x.is_a?(Numeric)
来源：http://bdy.hysaishi.cn

C#:   x is int or double or decimal
来源：http://gvx.bjfxy.top

[B14] 判断值是否在集合内
来源：http://zef.cheryme.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hxk.jqgufenzy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://xjw.ehwqpu.com

JS:   [1, 2, 3].includes(x)
来源：http://fyj.ppjwa.cn

TS:   [1, 2, 3].includes(x)
来源：http://icp.jiagoushi.top

Java: List.of(1, 2, 3).contains(x)
来源：http://ctb.c1oappe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baw.zhaomingkeji.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://btu.guannengcc.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ujc.sysykeji.top

[B15] 布尔运算与取反
来源：http://biq.0kj1m.cn

Py:   a and b or not c
来源：http://xhz.316326.xyz

PHP:  $a && $b || !$c
来源：http://djr.c1oappe.top

JS:   a && b || !c
来源：http://drd.yuanzhike.top

TS:   a && b || !c
来源：http://vwn.gogol.net.cn

Java: a && b || !c
来源：http://lbj.ehwqpu.com

Go:   a && b || !c
来源：http://jbg.vehdjk.com

Ruby: a && b || !c
来源：http://rpt.tanke756.top

C#:   a && b || !c
来源：http://zrv.fzhhl.top

[B16] 卫语句：不满足条件提前返回
来源：http://cpb.zhiwuduotai.top

Py:   if not data: return
来源：http://ars.xuetiantiany.cn

PHP:  if (!$data) { return; }
来源：http://vjh.jinyuanbaomall.cn

JS:   if (!data) return;
来源：http://tpz.xuanzx.com

TS:   if (!data) return;
来源：http://yhs.jyoumei.cn

Java: if (data == null) return;
来源：http://mji.kuanghao11.cn

Go:   if data == nil { return }
来源：http://iqn.dashuyun.cn

Ruby: return if data.nil?
来源：http://ptr.xylfe.cn

C#:   if (data == null) return;
来源：http://qgx.shangyingyoupin.top

================================================================================
来源：http://jzc.yfazqb.com

C. 函数与作用域
来源：http://vjj.ydjk.org.cn

================================================================================
来源：http://cyf.smart0.xyz

[C01] 定义函数
来源：http://cbj.yangfankeji.com

Py:   def add(a, b): return a + b
来源：http://gem.hammf.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ckv.xylfe.cn

JS:   function add(a, b) { return a + b; }
来源：http://wdi.xinyue.icu

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yhj.hongshengwenyu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ony.havefunace.top

Go:   func add(a, b int) int { return a + b }
来源：http://nca.ehwqpu.com

Ruby: def add(a, b); a + b; end
来源：http://est.hnxiangtu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cjm.dashuyun.cn

[C02] 默认参数
来源：http://cxy.jinqigfzy.top

Py:   def greet(name="World"): return name
来源：http://yjg.meibo888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://iyn.svipenyu.cn

JS:   function greet(name = "World") { return name; }
来源：http://oes.xinyue.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://cjj.bjfxy.top

Java: // 无默认参数：方法重载或 Optional
来源：http://msv.cheryme.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://uwo.wangshuangyany.cn

Ruby: def greet(name = "World") = name
来源：http://upr.bbcook.cn

C#:   string Greet(string name = "World") => name;
来源：http://tcm.yj20258888.top

[C03] 可变参数
来源：http://ygn.shzxlz.cn

Py:   def total(*args): return sum(args)
来源：http://car.ehwqpu.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jdq.ivvv.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rfp.pengpengdd.cyou

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://apo.hammf.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://gnr.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://rqx.haohaochexian.top

Ruby: def total(*nums); nums.sum; end
来源：http://odu.ivvv.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hie.nanxuanxn.top

[C04] 命名参数 / 关键字参数
来源：http://tps.yfazqb.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://npz.guowangkeji.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ngs.xuanzx.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gva.smart0.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://guu.hywenlv.cn

Java: // 无：用 Builder 模式或 record
来源：http://ooc.bjfxy.top

Go:   // 无：用配置结构体参数
来源：http://kqu.shuidangran.top

Ruby: f(a: 1, b: 2)
来源：http://daj.xziqi.cn

C#:   f(a: 1, b: 2)
来源：http://yvw.yongpay.top

[C05] 返回多个值
来源：http://ukp.snrcjt.cn

Py:   return a, b
来源：http://fks.snrcjt.cn

PHP:  return [$a, $b];
来源：http://wpt.chenlongwang.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://iot.xuetiantiany.cn

TS:   return { a, b };
来源：http://bwh.ehwqpu.com


<!-- 参考信息 -->