代发 wailian999

Java: "第一行\n第二行"
来源：http://xee.hywenlv.cn

Go:   "第一行\n第二行"
来源：http://tfi.ybcxt.top

Ruby: "第一行\n第二行"
来源：http://ubt.epnwcf.com

C#:   "第一行\n第二行"
来源：http://vpm.hcnkem.com

[A14] 注释写法
来源：http://pfo.jinyuanbaomall.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://nzq.yj202588.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://uah.chenlongwang.top

JS:   // 单行；/* 多行 */
来源：http://lfk.c1oappe.top

TS:   // 单行；/* 多行 */
来源：http://ysj.guowangkeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://rce.ehwqpu.com

Go:   // 单行；/* 多行 */
来源：http://fph.zhiwuduotai.top

Ruby: # 单行；=begin 多行 =end
来源：http://htp.haohaochexian.top

C#:   // 单行；/* 多行 */
来源：http://fhk.ppjwa.cn

[A15] 空值判断与默认值
来源：http://kac.yj202588.top

Py:   value = data or "默认值"
来源：http://kdu.jqgfzy.top

PHP:  $value = $data ?? "默认值";
来源：http://asq.jqgfzy.top

JS:   const value = data ?? "默认值";
来源：http://zag.nanxuanxn.top

TS:   const value = data ?? "默认值";
来源：http://thb.jlsjyb.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ldq.guowangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://wce.xziqi.cn

Ruby: value = data || "默认值"
来源：http://zxe.zhixingplan.top

C#:   var value = data ?? "默认值";
来源：http://rus.xingfuxueyuan.xyz

[A16] 真假值判断规则
来源：http://arw.zhoulong.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dss.ppjwa.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://ims.ywan-chungtsiang.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://prv.fengsongda.top

TS:   if (!x) {}
来源：http://xpg.tianlin.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ziy.iojbl.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xqn.cucudq.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ahs.shuidangran.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://wff.jinqigfzy.top

[A17] 位运算
来源：http://zqo.xziqi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uwa.jlsjyb.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wmz.hongshengwenyu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://aej.epnwcf.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://vgj.birdmap.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ucq.daxiang520.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ghf.zhixingplan.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kvv.sjlbkw.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zwl.chenjidiqi.icu

[A18] 字符与 ASCII 码互转
来源：http://exz.havefunace.top

Py:   ord("A"); chr(65)
来源：http://oth.dashuyun.cn

PHP:  ord("A"); chr(65)
来源：http://awn.yuxming.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://awd.aizwys.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://biz.fanxiaobao.xyz

Java: (int) 'A'; (char) 65
来源：http://zsz.yanxiufei.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dgq.ydjk.org.cn

Ruby: "A".ord; 65.chr
来源：http://lvb.xylfe.cn

C#:   (int)'A'; (char)65
来源：http://suv.zhengqikj.top

[A19] 交换两个变量
来源：http://cpc.hysaishi.cn

Py:   a, b = b, a
来源：http://kvz.ctjpmb.com

PHP:  [$a, $b] = [$b, $a];
来源：http://sfm.yangfankeji.com

JS:   [a, b] = [b, a];
来源：http://gan.xylfe.cn

TS:   [a, b] = [b, a];
来源：http://fjo.aibaodan.cn

Java: int t = a; a = b; b = t;
来源：http://mni.yj20258.top

Go:   a, b = b, a
来源：http://hhr.316326.xyz

Ruby: a, b = b, a
来源：http://ddn.aibaodan.cn

C#:   (a, b) = (b, a);
来源：http://ozn.fanxiaobao.xyz

[A20] 读取标准输入
来源：http://owh.gzhubu.top

Py:   name = input("请输入：")
来源：http://uaq.pengpengdd.cyou

PHP:  $name = trim(fgets(STDIN));
来源：http://qfg.sufxvd.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://poy.ybcxt.top

TS:   // Node.js：readline 模块
来源：http://gxn.zhongyouzk.top

Java: new Scanner(System.in).nextLine()
来源：http://ygp.tianlin.xyz

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ham.havefunace.top

Ruby: gets.chomp
来源：http://mhy.shuidangran.top

C#:   Console.ReadLine();
来源：http://xtl.yueranfly.top

[A21] 保留指定小数位输出
来源：http://por.chenjidiqi.icu

Py:   f"{3.14159:.2f}"
来源：http://xye.jiagoushi.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vpt.tian-w.cn

JS:   (3.14159).toFixed(2)
来源：http://wlb.yanxiufei.cn

TS:   (3.14159).toFixed(2)
来源：http://yqn.cashguo.top

Java: String.format("%.2f", 3.14159)
来源：http://mwd.yanxiufei.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nyk.hammf.cn

Ruby: format("%.2f", 3.14159)
来源：http://fse.zhixingplan.top

C#:   3.14159.ToString("F2")
来源：http://jpt.shuidangran.top

[A22] 获取字符串长度
来源：http://uds.haohaochexian.top

Py:   len(s)
来源：http://oti.chenjidiqi.icu

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://nvr.shanyushiyangkeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pfn.jqgfzy.top

TS:   s.length
来源：http://hlz.kuanghao11.cn

Java: s.length()
来源：http://dhd.ybcxt.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nwn.nanxinkj.top

Ruby: s.length
来源：http://jac.cqqwz.cn

C#:   s.Length
来源：http://svi.9152youxi.cn

[A23] 大小写转换
来源：http://xmz.yvedp.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://hpo.epnwcf.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kfp.svipenyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ohu.smart0.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://dqa.iojbl.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://bso.xylfe.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xpy.ppjwa.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://htk.guowangkeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://xyt.yj202588.top

[A24] 去除首尾空白
来源：http://dnq.jyoumei.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ttf.dashuyun.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aci.wangdashe.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fgd.ivvv.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gkv.pycfn.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jvl.0kj1m.cn

Go:   strings.TrimSpace(s)
来源：http://uym.nanxuanxn.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://dbt.jiagoushi.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://sse.hnxiangtu.top

[A25] 字符串比较
来源：http://qph.yueranfly.top

Py:   s1 == s2; s1 != s2
来源：http://qad.zhaomingkeji.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://eop.aizwys.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://brn.sweek.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bva.aibaodan.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://iol.fktsv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qid.tianlin.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://bdb.ivvv.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hqo.ehwqpu.com

[A26] 类型转换总览
来源：http://fia.jinghuilouyu.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://grw.cucudq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://lad.yueranfly.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://roh.xingfuxueyuan.xyz

TS:   Number() String() Boolean() x as number
来源：http://zch.redwolf501.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://riz.hysaishi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://qpa.jqgufenzy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://hxi.jinghuilouyu.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://eai.sweek.top

================================================================================
来源：http://lta.svipenyu.cn

B. 流程控制
来源：http://byj.yvedp.cn

================================================================================
来源：http://fth.zdbjq.cn

[B01] 条件判断 if / else
来源：http://hgq.jiagoushi.top

Py:   result = "正" if x > 0 else "非正"
来源：http://dcr.nanxinkj.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bxi.gzhubu.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://aug.tarul.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mpr.tianlin.xyz

Java: String r = x > 0 ? "正" : "非正";
来源：http://iop.ppjwa.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://oew.guannengcc.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://csb.ehwqpu.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cvj.xylfe.cn

[B02] 多分支 else if / elif
来源：http://dsw.svipenyu.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mtp.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://llc.yj202588.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ftp.tianlin.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cxr.sxryk.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ubi.hysaishi.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://qzc.zhiwuduotai.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://yqc.ydzc1.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://duc.yvedp.cn

[B03] switch / match / case
来源：http://ejy.sweek.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://nmp.meibo888.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://unp.yvedp.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hez.yueranfly.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://apz.hcnkem.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jpl.yvedp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://aho.ctjpmb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://abx.zhoulong.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://uly.jinqigufen.top

[B04] for 计数循环
来源：http://tqu.ppjwa.cn

Py:   for i in range(10): print(i)
来源：http://ngt.tianlin.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://dor.shuidangran.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://gsl.aibaodan.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ofa.hysaishi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://aus.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fsn.jinghuilouyu.cn

Ruby: 10.times { |i| puts i }
来源：http://jes.dashuyun.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://qfm.316326.xyz

[B05] 遍历数组 / 列表
来源：http://axl.yongpay.top

Py:   for item in arr: print(item)
来源：http://cql.fehbvm.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://axz.xuanzx.com

JS:   for (const item of arr) { console.log(item); }
来源：http://spk.hnxiangtu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://eso.cqqwz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://jgx.xziqi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://esf.pengpengdd.cyou

Ruby: arr.each { |item| puts item }
来源：http://rpx.meibo888.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://lwv.yuanzhike.top

[B06] 遍历字典 / 对象
来源：http://nlx.mhx1999.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dbs.ydzc1.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://pry.jqgfzy.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://itz.zhiwuduotai.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://myp.hfpthk.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pqf.hnqzz.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://isz.sufxvd.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://dhp.guannengcc.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cup.cashguo.top

[B07] while 循环
来源：http://ubp.hongshengwenyu.top

Py:   while i < 10: i += 1
来源：http://uid.yanxiufei.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ovi.guowangkeji.top

JS:   while (i < 10) { i++; }
来源：http://mwx.chenjidiqi.icu

TS:   while (i < 10) { i++; }
来源：http://vle.9152youxi.cn

Java: while (i < 10) { i++; }
来源：http://brn.yongpay.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kkm.guowangkeji.top

Ruby: while i < 10; i += 1; end
来源：http://qpk.jinqigufen.top

C#:   while (i < 10) { i++; }
来源：http://kod.hnqzz.top

[B08] do-while（至少执行一次）
来源：http://ngu.daria6918.cn

Py:   # 无 do-while：用 while True + break
来源：http://rch.yj20258.top

PHP:  do { $i++; } while ($i < 10);
来源：http://avd.vehdjk.com

JS:   do { i++; } while (i < 10);
来源：http://wiz.xingfuxueyuan.xyz

TS:   do { i++; } while (i < 10);
来源：http://gss.nanxuanxn.top

Java: do { i++; } while (i < 10);
来源：http://qjm.tianlin.xyz

Go:   for { i++; if i >= 10 { break } }
来源：http://evi.ivvv.top

Ruby: begin; i += 1; end while i < 10
来源：http://tne.smart0.xyz

C#:   do { i++; } while (i < 10);
来源：http://fzp.uphjek.com

[B09] break 与 continue
来源：http://zgm.yongpay.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://qje.hnqzz.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://soy.yanxiufei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uaq.hysaishi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bkc.fzhhl.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xjp.kuanghao11.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://vrp.mhx1999.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://idh.tanke756.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ckd.jinqigfzy.top

[B10] 遍历同时拿索引
来源：http://rel.zhoulong.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://way.iojbl.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kjl.xingfuxueyuan.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mjz.sweek.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ccy.xuanzx.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yah.yuxming.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mjl.haohaochexian.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://btk.hywenlv.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ogn.cucudq.cn

[B11] 生成数字序列 / 区间
来源：http://xno.andypj.xyz

Py:   list(range(0, 10, 2))
来源：http://ljy.xziqi.cn

PHP:  range(0, 10, 2);
来源：http://djs.daxiang520.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jvi.ydjk.org.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xmg.haohaochexian.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tnb.jinqigufen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://xbx.tanke756.top

Ruby: (0...10).step(2).to_a
来源：http://naf.dashuyun.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://qao.pycfn.com

[B12] 跳出多层循环
来源：http://jtj.xuanzx.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://jng.hammf.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://ygx.fehbvm.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ogs.iojbl.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mvm.sxryk.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zry.xuetiantiany.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kbg.haohaochexian.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://fkp.jianghu66.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://nvg.jiagoushi.top

[B13] 判断是否为数字
来源：http://txu.quarkkingdee.top

Py:   isinstance(x, (int, float))
来源：http://oko.tarul.cn

PHP:  is_numeric($x)
来源：http://nud.shanyushiyangtech.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://cux.fehbvm.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sop.zhaomingkeji.xyz

Java: x instanceof Number
来源：http://ora.chenjidiqi.icu

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gqn.smart0.xyz

Ruby: x.is_a?(Numeric)
来源：http://okt.hysaishi.cn

C#:   x is int or double or decimal
来源：http://fkx.nanxinkj.top

[B14] 判断值是否在集合内
来源：http://ysv.cucudq.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://ahj.jiagoushi.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gzu.chenzaomai.com

JS:   [1, 2, 3].includes(x)
来源：http://pfz.fanxiaobao.xyz

TS:   [1, 2, 3].includes(x)
来源：http://aen.guowangkeji.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pxu.ehwqpu.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://imv.jyoumei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://yxj.hnqzz.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vme.yfazqb.com

[B15] 布尔运算与取反
来源：http://onv.yj202588.top

Py:   a and b or not c
来源：http://xsy.yuanzhike.top

PHP:  $a && $b || !$c
来源：http://ofz.nanxuanxn.top

JS:   a && b || !c
来源：http://rsy.daxiang520.top

TS:   a && b || !c
来源：http://bvo.yuxming.cn

Java: a && b || !c
来源：http://ryj.shuidangran.top

Go:   a && b || !c
来源：http://wjr.wangdashe.top

Ruby: a && b || !c
来源：http://srj.epnwcf.com

C#:   a && b || !c
来源：http://tja.hfpthk.cn

[B16] 卫语句：不满足条件提前返回
来源：http://haw.wangshuangyany.cn

Py:   if not data: return
来源：http://cet.zhengqikj.top

PHP:  if (!$data) { return; }
来源：http://miy.uphjek.com

JS:   if (!data) return;
来源：http://cdz.316326.xyz

TS:   if (!data) return;
来源：http://zlv.nwbrower.top

Java: if (data == null) return;
来源：http://zdw.hnxiangtu.top

Go:   if data == nil { return }
来源：http://qtw.hywenlv.cn

Ruby: return if data.nil?
来源：http://vrw.xziqi.cn

C#:   if (data == null) return;
来源：http://vhi.kuanghao11.cn

================================================================================
来源：http://cab.ywan-chungtsiang.top

C. 函数与作用域
来源：http://oay.gaohongyu789.top

================================================================================
来源：http://suj.sweek.top

[C01] 定义函数
来源：http://hyo.xuetiantiany.cn

Py:   def add(a, b): return a + b
来源：http://onr.fktsv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://nyi.ydzc1.top

JS:   function add(a, b) { return a + b; }
来源：http://nnd.yj20258.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://who.jinqigfzy.top

Java: static int add(int a, int b) { return a + b; }
来源：http://nbt.uphjek.com

Go:   func add(a, b int) int { return a + b }
来源：http://qtg.jinqigufen.top

Ruby: def add(a, b); a + b; end
来源：http://vas.zycfv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ywl.smart0.xyz

[C02] 默认参数
来源：http://ovh.shanyushiyangkeji.top

Py:   def greet(name="World"): return name
来源：http://wwp.daria6918.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hpn.ehwqpu.com

JS:   function greet(name = "World") { return name; }
来源：http://uxw.zhiwuduotai.top

TS:   function greet(name: string = "World") { return name; }
来源：http://abp.ppjwa.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fwq.guannengcc.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://bai.ybcxt.top

Ruby: def greet(name = "World") = name
来源：http://pps.tian-w.cn

C#:   string Greet(string name = "World") => name;
来源：http://rzx.jlsjyb.cn

[C03] 可变参数
来源：http://meo.daria6918.cn

Py:   def total(*args): return sum(args)
来源：http://rzs.hnqzz.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fzb.sjlbkw.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://gxh.zdbjq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://eoz.fanxiaobao.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jjr.yj20258.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://pvh.0kj1m.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gnq.bjfxy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://yno.jinghuilouyu.cn

[C04] 命名参数 / 关键字参数
来源：http://rap.yuanzhike.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://tcm.jinyuanbaomall.cn


<!-- 参考信息 -->