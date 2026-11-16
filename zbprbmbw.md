代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://eho.chenjidiqi.icu

Ruby: unless x            # nil 与 false 为假
来源：http://mvb.ivvv.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xmn.shanyushiyangtech.top

[A17] 位运算
来源：http://nku.zhiwuduotai.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nok.ctjpmb.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pbl.fengsongda.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vyc.yueranfly.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gnu.vehdjk.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mzh.chenjidiqi.icu

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dqi.haohaochexian.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xbc.ctjpmb.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vnu.hysaishi.cn

[A18] 字符与 ASCII 码互转
来源：http://bsi.hesvh.cn

Py:   ord("A"); chr(65)
来源：http://awg.nanxinkj.top

PHP:  ord("A"); chr(65)
来源：http://cpq.hcnkem.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://riy.kuanghao11.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vwq.xuanzx.com

Java: (int) 'A'; (char) 65
来源：http://ntg.zdqjudy.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dyp.fzhhl.top

Ruby: "A".ord; 65.chr
来源：http://pkk.pycfn.com

C#:   (int)'A'; (char)65
来源：http://zsa.zhijiandao.cn

[A19] 交换两个变量
来源：http://xrh.jinqigufen.top

Py:   a, b = b, a
来源：http://vgv.jinyuanbaomall.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://glz.gzhubu.top

JS:   [a, b] = [b, a];
来源：http://ysb.zhiwuduotai.top

TS:   [a, b] = [b, a];
来源：http://dcx.xylfe.cn

Java: int t = a; a = b; b = t;
来源：http://cvo.cdnleiting.top

Go:   a, b = b, a
来源：http://wzi.zhaomingkeji.xyz

Ruby: a, b = b, a
来源：http://mdl.cdnleiting.top

C#:   (a, b) = (b, a);
来源：http://lwk.smart0.xyz

[A20] 读取标准输入
来源：http://sxu.kuanghao11.cn

Py:   name = input("请输入：")
来源：http://caw.sxryk.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://sjp.sysykeji.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hoc.ydjk.org.cn

TS:   // Node.js：readline 模块
来源：http://cdj.cdnleiting.top

Java: new Scanner(System.in).nextLine()
来源：http://fso.pengpengdd.cyou

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nkd.gzhubu.top

Ruby: gets.chomp
来源：http://ypf.mhx1999.top

C#:   Console.ReadLine();
来源：http://rbh.cheryme.top

[A21] 保留指定小数位输出
来源：http://liz.yj20258.top

Py:   f"{3.14159:.2f}"
来源：http://ifm.uphjek.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://cea.chenjidiqi.icu

JS:   (3.14159).toFixed(2)
来源：http://xsa.jinghuilouyu.cn

TS:   (3.14159).toFixed(2)
来源：http://mnq.guannengcc.top

Java: String.format("%.2f", 3.14159)
来源：http://pfq.yongpay.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://euc.tianlin.xyz

Ruby: format("%.2f", 3.14159)
来源：http://zif.xuanzx.com

C#:   3.14159.ToString("F2")
来源：http://sof.sufxvd.cn

[A22] 获取字符串长度
来源：http://xld.quarkkingdee.top

Py:   len(s)
来源：http://onz.ppjwa.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://tzp.havefunace.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nei.uphjek.com

TS:   s.length
来源：http://cbh.wangshuangyany.cn

Java: s.length()
来源：http://sek.yuxming.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qez.chenlongwang.top

Ruby: s.length
来源：http://uqf.chenlongwang.top

C#:   s.Length
来源：http://ptz.andypj.xyz

[A23] 大小写转换
来源：http://pre.jianghu66.top

Py:   s.upper(); s.lower(); s.title()
来源：http://naw.cdnleiting.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uqh.ybcxt.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gup.kuanghao11.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://tqd.jinqigfzy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zru.ctjpmb.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://obi.xingfuxueyuan.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ioe.ybcxt.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dtd.iojbl.cn

[A24] 去除首尾空白
来源：http://cpe.zdqjudy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://upp.hysaishi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zex.jinyuanbaomall.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://esa.tian-w.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gok.xylfe.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ejz.yanxiufei.cn

Go:   strings.TrimSpace(s)
来源：http://aln.dianchejie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wvz.kuanghao11.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://wqh.meibo888.top

[A25] 字符串比较
来源：http://tpm.hnqzz.top

Py:   s1 == s2; s1 != s2
来源：http://goe.pengpengdd.cyou

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cik.bbcook.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fpo.jqgufenzy.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://vtv.aizwys.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sam.tianlin.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://rsl.yuxming.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vyu.nwbrower.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://omx.hywenlv.cn

[A26] 类型转换总览
来源：http://lfi.9152youxi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://aem.hfpthk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://cdr.jqgufenzy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://vrh.pycfn.com

TS:   Number() String() Boolean() x as number
来源：http://jti.redwolf501.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fct.svipenyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fit.ppjwa.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://jnz.zdqjudy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ljj.yongpay.top

================================================================================
来源：http://fzk.hysaishi.cn

B. 流程控制
来源：http://ewh.epnwcf.com

================================================================================
来源：http://jak.hnqzz.top

[B01] 条件判断 if / else
来源：http://nij.yfazqb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://ovt.jinqigfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://vrg.hesvh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hbi.zhoulong.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://joe.jinqigufen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qne.ydzc1.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://jla.cqqwz.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://moi.jinyuanbaomall.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://xfv.chenjidiqi.icu

[B02] 多分支 else if / elif
来源：http://bvw.zhongyouzk.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xzk.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zfl.jqgufenzy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://juf.0kj1m.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gyk.dianchejie.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vnu.jyoumei.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zxf.jqgufenzy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://alq.zhoulong.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xnk.tanke756.top

[B03] switch / match / case
来源：http://tsv.aibaodan.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wbv.guowangkeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://moz.ywan-chungtsiang.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bra.jinqigufen.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rdm.zycfv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kpv.yuanzhike.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://psw.xinyue.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hon.zhiwuduotai.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://txh.hnqzz.top

[B04] for 计数循环
来源：http://dks.iojbl.cn

Py:   for i in range(10): print(i)
来源：http://veq.sufxvd.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://llw.xylfe.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://klk.guowangkeji.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kjr.yvedp.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://eyc.cheryme.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tqj.vqdsnc.cn

Ruby: 10.times { |i| puts i }
来源：http://mxy.yangfankeji.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sjo.hcnkem.com

[B05] 遍历数组 / 列表
来源：http://nju.shangyingyoupin.top

Py:   for item in arr: print(item)
来源：http://hkq.pengpengdd.cyou

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yyz.pycfn.com

JS:   for (const item of arr) { console.log(item); }
来源：http://uoo.jianghu66.top

TS:   for (const item of arr) { console.log(item); }
来源：http://kru.chenzaomai.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://rez.uphjek.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zxe.meibo888.top

Ruby: arr.each { |item| puts item }
来源：http://umw.epnwcf.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://scm.gzhubu.top

[B06] 遍历字典 / 对象
来源：http://sgz.yuanzhike.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ltv.yvedp.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://kcv.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://acp.tian-w.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://znz.ydjk.org.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ebr.sxryk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://byt.zhoulong.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zwy.quarkkingdee.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://vfr.hywenlv.cn

[B07] while 循环
来源：http://eaf.9152youxi.cn

Py:   while i < 10: i += 1
来源：http://fqj.gotoacloud.top

PHP:  while ($i < 10) { $i++; }
来源：http://mhe.uphjek.com

JS:   while (i < 10) { i++; }
来源：http://qds.nanxuanxn.top

TS:   while (i < 10) { i++; }
来源：http://ulh.yj202588.top

Java: while (i < 10) { i++; }
来源：http://tsd.xinyue.icu

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://pfp.zhengqikj.top

Ruby: while i < 10; i += 1; end
来源：http://cfy.316326.xyz

C#:   while (i < 10) { i++; }
来源：http://wqq.vqdsnc.cn

[B08] do-while（至少执行一次）
来源：http://yyh.xinyue.icu

Py:   # 无 do-while：用 while True + break
来源：http://hei.yangfankeji.com

PHP:  do { $i++; } while ($i < 10);
来源：http://nhc.ydjk.org.cn

JS:   do { i++; } while (i < 10);
来源：http://qtv.jinqigfzy.top

TS:   do { i++; } while (i < 10);
来源：http://hgh.hfpthk.cn

Java: do { i++; } while (i < 10);
来源：http://yml.tian-w.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gdq.ydjk.org.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tdi.yj202588.top

C#:   do { i++; } while (i < 10);
来源：http://bpc.hfpthk.cn

[B09] break 与 continue
来源：http://aas.epnwcf.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://kra.9152youxi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://jzf.daxiang520.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ink.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://osy.fanxiaobao.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wev.yj20258.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vyi.sysykeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qkn.xziqi.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ech.zhaomingkeji.xyz

[B10] 遍历同时拿索引
来源：http://hdj.cashguo.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vxl.nanxinkj.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nhe.bbcook.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://tuu.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://shr.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://caj.yongpay.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://qfe.pengpengdd.cyou

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://jed.gzhubu.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wdw.cashguo.top

[B11] 生成数字序列 / 区间
来源：http://wmg.hnqzz.top

Py:   list(range(0, 10, 2))
来源：http://rmz.fehbvm.com

PHP:  range(0, 10, 2);
来源：http://vem.nanxinkj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://gyj.svipenyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yer.jinqigufen.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lpp.vqdsnc.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hbk.cdnleiting.top

Ruby: (0...10).step(2).to_a
来源：http://qyg.tanke756.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pvq.ybcxt.top

[B12] 跳出多层循环
来源：http://sfr.iojbl.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://biu.xuanzx.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://vie.shuidangran.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://qyq.yfazqb.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qzx.guowangkeji.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://klf.zhaomingkeji.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://zmc.feifeiyinyue.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://syh.yanxiufei.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wff.cqqwz.cn

[B13] 判断是否为数字
来源：http://lii.shuidangran.top

Py:   isinstance(x, (int, float))
来源：http://tde.jinyuanbaomall.cn

PHP:  is_numeric($x)
来源：http://ivg.guannengcc.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pcl.pycfn.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kcr.sufxvd.cn

Java: x instanceof Number
来源：http://xxa.zhoulong.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cjt.yfazqb.com

Ruby: x.is_a?(Numeric)
来源：http://grf.kuanghao11.cn

C#:   x is int or double or decimal
来源：http://kqm.yj20258888.top

[B14] 判断值是否在集合内
来源：http://fzj.hnxiangtu.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://dcn.tarul.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://wls.kuanghao11.cn

JS:   [1, 2, 3].includes(x)
来源：http://vbu.nanxuanxn.top

TS:   [1, 2, 3].includes(x)
来源：http://krc.cdnleiting.top

Java: List.of(1, 2, 3).contains(x)
来源：http://dsp.jyoumei.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hbm.vehdjk.com

Ruby: [1, 2, 3].include?(x)
来源：http://ige.tanke756.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rmn.gotoacloud.top

[B15] 布尔运算与取反
来源：http://vmf.daria6918.cn

Py:   a and b or not c
来源：http://fqz.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://ryl.cqqwz.cn

JS:   a && b || !c
来源：http://fsb.0kj1m.cn

TS:   a && b || !c
来源：http://evx.ehwqpu.com

Java: a && b || !c
来源：http://ext.sufxvd.cn

Go:   a && b || !c
来源：http://sen.yanxiufei.cn

Ruby: a && b || !c
来源：http://bvi.haohaochexian.top

C#:   a && b || !c
来源：http://wjh.fehbvm.com

[B16] 卫语句：不满足条件提前返回
来源：http://lnj.yuanzhike.top

Py:   if not data: return
来源：http://pbi.gotoacloud.top

PHP:  if (!$data) { return; }
来源：http://fbl.chenjidiqi.icu

JS:   if (!data) return;
来源：http://ixo.zhaomingkeji.xyz

TS:   if (!data) return;
来源：http://ncp.guannengcc.top

Java: if (data == null) return;
来源：http://uql.cqqwz.cn

Go:   if data == nil { return }
来源：http://rzy.xziqi.cn

Ruby: return if data.nil?
来源：http://zll.ydzc1.top

C#:   if (data == null) return;
来源：http://ltu.jinqigfzy.top

================================================================================
来源：http://ufc.xylfe.cn

C. 函数与作用域
来源：http://kop.hywenlv.cn

================================================================================
来源：http://jej.xuetiantiany.cn

[C01] 定义函数
来源：http://pcl.aibaodan.cn

Py:   def add(a, b): return a + b
来源：http://ces.zhengqikj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hyx.tianlin.xyz

JS:   function add(a, b) { return a + b; }
来源：http://sfw.sufxvd.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://orq.jlsjyb.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://uoz.uphjek.com

Go:   func add(a, b int) int { return a + b }
来源：http://hhf.hnqzz.top

Ruby: def add(a, b); a + b; end
来源：http://exw.xuetiantiany.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://jes.yanxiufei.cn

[C02] 默认参数
来源：http://zmm.316326.xyz

Py:   def greet(name="World"): return name
来源：http://xax.zhixingplan.top

PHP:  function greet($name = "World") { return $name; }
来源：http://aqr.tanke756.top

JS:   function greet(name = "World") { return name; }
来源：http://dur.ydzc1.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tuu.xziqi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://uts.yuxming.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wws.dianchejie.cn

Ruby: def greet(name = "World") = name
来源：http://uuh.hysaishi.cn

C#:   string Greet(string name = "World") => name;
来源：http://psd.yj202588.top

[C03] 可变参数
来源：http://psa.epnwcf.com

Py:   def total(*args): return sum(args)
来源：http://pbi.9152youxi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://kfe.ctjpmb.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://oij.tanke756.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://dkb.zycfv.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mkl.xziqi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ljd.jinqigufen.top

Ruby: def total(*nums); nums.sum; end
来源：http://qxw.yonumen.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hcy.jianghu66.top

[C04] 命名参数 / 关键字参数
来源：http://ace.hcnkem.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://gdb.nanxuanxn.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mzb.gzhubu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://efb.hongshengwenyu.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xyq.hcnkem.com

Java: // 无：用 Builder 模式或 record
来源：http://ins.cheryme.top

Go:   // 无：用配置结构体参数
来源：http://kia.redwolf501.top

Ruby: f(a: 1, b: 2)
来源：http://nsp.ywan-chungtsiang.top

C#:   f(a: 1, b: 2)
来源：http://icj.xylfe.cn

[C05] 返回多个值
来源：http://apf.dashuyun.cn

Py:   return a, b
来源：http://blr.fengsongda.top

PHP:  return [$a, $b];
来源：http://mfc.daria6918.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://zwz.cucudq.cn

TS:   return { a, b };
来源：http://ehh.redwolf501.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://plu.guowangkeji.top

Go:   return a, b
来源：http://vrq.jlsjyb.cn

Ruby: return a, b
来源：http://wyx.hywenlv.cn

C#:   return (a, b);              // ValueTuple
来源：http://bqe.snrcjt.cn

[C06] 匿名函数 / lambda
来源：http://prr.ivvv.top

Py:   square = lambda x: x * x
来源：http://dle.fengsongda.top

PHP:  $square = fn($x) => $x * $x;
来源：http://mpe.vehdjk.com

JS:   const square = x => x * x;
来源：http://xyq.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://jec.fktsv.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fbb.pengpengdd.cyou

Go:   sq := func(x int) int { return x * x }
来源：http://pwf.xuetiantiany.cn

Ruby: square = ->(x) { x * x }
来源：http://fxl.yonumen.top

C#:   Func<int, int> square = x => x * x;
来源：http://bzn.ywan-chungtsiang.top

[C07] 把函数作为参数传入
来源：http://oou.sufxvd.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://pwy.zhixingplan.top

PHP:  array_map("strtoupper", $arr);
来源：http://qtp.xylfe.cn


<!-- 参考信息 -->