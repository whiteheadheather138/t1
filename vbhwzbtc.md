代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://wkj.sjlbkw.cn

[A15] 空值判断与默认值
来源：http://joj.nanxinkj.top

Py:   value = data or "默认值"
来源：http://vgc.ivvv.top

PHP:  $value = $data ?? "默认值";
来源：http://coc.wangdashe.top

JS:   const value = data ?? "默认值";
来源：http://rmm.nanxinkj.top

TS:   const value = data ?? "默认值";
来源：http://bjr.sufxvd.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://juy.zdbjq.cn

Go:   if data == "" { data = "默认值" }
来源：http://jlx.ctjpmb.com

Ruby: value = data || "默认值"
来源：http://ifc.c1oappe.top

C#:   var value = data ?? "默认值";
来源：http://bqf.vqdsnc.cn

[A16] 真假值判断规则
来源：http://sel.cdnleiting.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zpr.yonumen.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://tcj.sysykeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://bkc.yuxming.cn

TS:   if (!x) {}
来源：http://vcy.mhx1999.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qds.sjlbkw.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ntt.daria6918.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gjx.yonumen.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yab.iojbl.cn

[A17] 位运算
来源：http://gqj.pengpengdd.cyou

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://djz.wangshuangyany.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uzl.meibo888.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fkb.shuidangran.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hmr.jqgufenzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nlg.yueranfly.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://iss.iojbl.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mjx.kuanghao11.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zeu.aizwys.cn

[A18] 字符与 ASCII 码互转
来源：http://lsv.ywan-chungtsiang.top

Py:   ord("A"); chr(65)
来源：http://mhn.sxryk.cn

PHP:  ord("A"); chr(65)
来源：http://bcm.pycfn.com

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jvb.bbcook.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ggd.andypj.xyz

Java: (int) 'A'; (char) 65
来源：http://mvx.chenlongwang.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://icx.fktsv.cn

Ruby: "A".ord; 65.chr
来源：http://ctw.daxiang520.top

C#:   (int)'A'; (char)65
来源：http://adj.hnxiangtu.top

[A19] 交换两个变量
来源：http://cgj.ctjpmb.com

Py:   a, b = b, a
来源：http://htk.birdmap.top

PHP:  [$a, $b] = [$b, $a];
来源：http://qum.yonumen.top

JS:   [a, b] = [b, a];
来源：http://bpu.quarkkingdee.top

TS:   [a, b] = [b, a];
来源：http://ore.feifeiyinyue.top

Java: int t = a; a = b; b = t;
来源：http://drh.yuanzhike.top

Go:   a, b = b, a
来源：http://ufl.sjlbkw.cn

Ruby: a, b = b, a
来源：http://ezz.yongpay.top

C#:   (a, b) = (b, a);
来源：http://wsy.yuanzhike.top

[A20] 读取标准输入
来源：http://nsz.xylfe.cn

Py:   name = input("请输入：")
来源：http://mca.chenzaomai.com

PHP:  $name = trim(fgets(STDIN));
来源：http://tre.shuidangran.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rxc.ydzc1.top

TS:   // Node.js：readline 模块
来源：http://prf.shangyingyoupin.top

Java: new Scanner(System.in).nextLine()
来源：http://oph.yanxiufei.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://lik.sysykeji.top

Ruby: gets.chomp
来源：http://rxx.zhiwuduotai.top

C#:   Console.ReadLine();
来源：http://mju.zdbjq.cn

[A21] 保留指定小数位输出
来源：http://rjf.hcnkem.com

Py:   f"{3.14159:.2f}"
来源：http://kup.daxiang520.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jvb.dianchejie.cn

JS:   (3.14159).toFixed(2)
来源：http://ine.yongpay.top

TS:   (3.14159).toFixed(2)
来源：http://wxy.hcnkem.com

Java: String.format("%.2f", 3.14159)
来源：http://bsk.jqgfzy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vvz.cashguo.top

Ruby: format("%.2f", 3.14159)
来源：http://rye.9152youxi.cn

C#:   3.14159.ToString("F2")
来源：http://aeo.shanyushiyangkeji.top

[A22] 获取字符串长度
来源：http://fio.shuidangran.top

Py:   len(s)
来源：http://sjy.yongpay.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://xit.yanxiufei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://jry.jiagoushi.top

TS:   s.length
来源：http://phf.shanyushiyangkeji.top

Java: s.length()
来源：http://bbn.sxryk.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://sga.bbcook.cn

Ruby: s.length
来源：http://cvp.cashguo.top

C#:   s.Length
来源：http://ccp.jlsjyb.cn

[A23] 大小写转换
来源：http://bsn.jyoumei.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rns.chenjidiqi.icu

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vjy.sjlbkw.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hwv.jiagoushi.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xpw.snrcjt.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ndm.daria6918.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://thg.zhixingplan.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://atk.ehwqpu.com

C#:   s.ToUpper(); s.ToLower()
来源：http://mvl.guowangkeji.top

[A24] 去除首尾空白
来源：http://kih.tianlin.xyz

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ebq.aizwys.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wxh.vqdsnc.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qrr.jinqigfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dre.zhixingplan.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gnh.guannengcc.top

Go:   strings.TrimSpace(s)
来源：http://ibu.wangdashe.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bmv.hnqzz.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://lcj.jinyuanbaomall.cn

[A25] 字符串比较
来源：http://uqu.smart0.xyz

Py:   s1 == s2; s1 != s2
来源：http://ppm.vqdsnc.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sxb.daxiang520.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://msr.yj20258888.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gpq.ehwqpu.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://frs.gogol.net.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mmm.zhaomingkeji.xyz

Ruby: s1 == s2; s1 <=> s2
来源：http://ybp.gogol.net.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://sbc.xuanzx.com

[A26] 类型转换总览
来源：http://nll.shuidangran.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kce.cdnleiting.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ons.gogol.net.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://iyq.zdqjudy.top

TS:   Number() String() Boolean() x as number
来源：http://bia.bjfxy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ssc.hysaishi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rrv.tianlin.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://twj.zdbjq.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://idb.xinyue.icu

================================================================================
来源：http://mgv.fzhhl.top

B. 流程控制
来源：http://gsn.jyoumei.cn

================================================================================
来源：http://xvz.jinqigufen.top

[B01] 条件判断 if / else
来源：http://qaq.guannengcc.top

Py:   result = "正" if x > 0 else "非正"
来源：http://glr.yonumen.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ydm.smart0.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pkf.9152youxi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hxm.sxryk.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://tip.sufxvd.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xfs.jiagoushi.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://cnq.xylfe.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://gns.sxryk.cn

[B02] 多分支 else if / elif
来源：http://zju.hammf.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xwr.hcnkem.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kin.shzxlz.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rcu.dianchejie.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mqd.jianghu66.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mac.meibo888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://jgd.nanxuanxn.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xtr.gotoacloud.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sfn.c1oappe.top

[B03] switch / match / case
来源：http://nvf.52xcode.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blc.zhengqikj.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://nld.yuanzhike.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fxq.epnwcf.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yhi.sufxvd.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vev.zhongyouzk.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dqk.yuanzhike.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://gvp.shanyushiyangtech.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ekh.birdmap.top

[B04] for 计数循环
来源：http://opx.dashuyun.cn

Py:   for i in range(10): print(i)
来源：http://ivj.shuidangran.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hde.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pdi.jqgufenzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ulf.shuidangran.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zgj.gogol.net.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://czk.pycfn.com

Ruby: 10.times { |i| puts i }
来源：http://bto.hywenlv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://cyy.chenjidiqi.icu

[B05] 遍历数组 / 列表
来源：http://iob.shangyingyoupin.top

Py:   for item in arr: print(item)
来源：http://urc.wangshuangyany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ndh.daria6918.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://ups.birdmap.top

TS:   for (const item of arr) { console.log(item); }
来源：http://ain.jinghuilouyu.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://kjv.jinyuanbaomall.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://joz.yonumen.top

Ruby: arr.each { |item| puts item }
来源：http://mpz.yanxiufei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://bzr.birdmap.top

[B06] 遍历字典 / 对象
来源：http://hqk.zhongyouzk.top

Py:   for k, v in d.items(): print(k, v)
来源：http://hkj.jyoumei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fqd.0kj1m.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://nbk.yongpay.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tqf.ydzc1.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://pvz.chenjidiqi.icu

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gwv.yueranfly.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://cql.ydjk.org.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://ilr.cucudq.cn

[B07] while 循环
来源：http://eab.jinqigfzy.top

Py:   while i < 10: i += 1
来源：http://vut.gaohongyu789.top

PHP:  while ($i < 10) { $i++; }
来源：http://ppz.shzxlz.cn

JS:   while (i < 10) { i++; }
来源：http://rtl.xuanzx.com

TS:   while (i < 10) { i++; }
来源：http://nlc.uphjek.com

Java: while (i < 10) { i++; }
来源：http://wlx.hcnkem.com

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yhg.ehwqpu.com

Ruby: while i < 10; i += 1; end
来源：http://pps.cqqwz.cn

C#:   while (i < 10) { i++; }
来源：http://jzi.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://jrv.fktsv.cn

Py:   # 无 do-while：用 while True + break
来源：http://ysq.gaohongyu789.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gfr.chenlongwang.top

JS:   do { i++; } while (i < 10);
来源：http://ywa.zhixingplan.top

TS:   do { i++; } while (i < 10);
来源：http://gou.jiagoushi.top

Java: do { i++; } while (i < 10);
来源：http://qrf.shzxlz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://mml.yfazqb.com

Ruby: begin; i += 1; end while i < 10
来源：http://ttm.yongpay.top

C#:   do { i++; } while (i < 10);
来源：http://gcw.ppjwa.cn

[B09] break 与 continue
来源：http://alq.hongshengwenyu.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://ubr.feifeiyinyue.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://sqb.jyoumei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tve.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dfr.yangfankeji.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rrf.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pmh.shuidangran.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ngi.jinqigufen.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gqx.fzhhl.top

[B10] 遍历同时拿索引
来源：http://tkq.gzhubu.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://kvb.jlsjyb.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://efq.yongpay.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ygt.hnqzz.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cro.hesvh.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cgr.fktsv.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://huw.xylfe.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ozu.hesvh.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://yqz.0kj1m.cn

[B11] 生成数字序列 / 区间
来源：http://lew.birdmap.top

Py:   list(range(0, 10, 2))
来源：http://zri.xinyue.icu

PHP:  range(0, 10, 2);
来源：http://oli.iojbl.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qqe.yangfankeji.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hsq.shangyingyoupin.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://sre.zhengqikj.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://izw.feifeiyinyue.top

Ruby: (0...10).step(2).to_a
来源：http://bsh.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iin.quarkkingdee.top

[B12] 跳出多层循环
来源：http://arw.redwolf501.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://igg.gogol.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jwh.gzhubu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rpy.jqgfzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://iqt.ydzc1.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://cmu.feifeiyinyue.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://pxm.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ses.pycfn.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://crj.jinghuilouyu.cn

[B13] 判断是否为数字
来源：http://sos.ywan-chungtsiang.top

Py:   isinstance(x, (int, float))
来源：http://xix.hongshengwenyu.top

PHP:  is_numeric($x)
来源：http://efp.cheryme.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vhl.cdnleiting.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://doh.yfazqb.com

Java: x instanceof Number
来源：http://amm.yongpay.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://yse.daria6918.cn

Ruby: x.is_a?(Numeric)
来源：http://hqt.hnqzz.top

C#:   x is int or double or decimal
来源：http://ckx.xingfuxueyuan.xyz

[B14] 判断值是否在集合内
来源：http://wtv.sufxvd.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://peb.jinghuilouyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rtd.epnwcf.com

JS:   [1, 2, 3].includes(x)
来源：http://emi.shanyushiyangtech.top

TS:   [1, 2, 3].includes(x)
来源：http://mfv.gotoacloud.top

Java: List.of(1, 2, 3).contains(x)
来源：http://pnb.bjfxy.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://sqr.wangshuangyany.cn

Ruby: [1, 2, 3].include?(x)
来源：http://vss.sxryk.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://uzr.sxryk.cn

[B15] 布尔运算与取反
来源：http://rmo.nanxinkj.top

Py:   a and b or not c
来源：http://amz.hnxiangtu.top

PHP:  $a && $b || !$c
来源：http://trn.hammf.cn

JS:   a && b || !c
来源：http://sjx.guannengcc.top

TS:   a && b || !c
来源：http://kiu.zhaomingkeji.xyz

Java: a && b || !c
来源：http://unt.zycfv.cn

Go:   a && b || !c
来源：http://ldu.zycfv.cn

Ruby: a && b || !c
来源：http://gvn.hongshengwenyu.top

C#:   a && b || !c
来源：http://btp.gotoacloud.top

[B16] 卫语句：不满足条件提前返回
来源：http://itv.316326.xyz

Py:   if not data: return
来源：http://prc.zhiwuduotai.top

PHP:  if (!$data) { return; }
来源：http://ecr.cashguo.top

JS:   if (!data) return;
来源：http://bgm.0kj1m.cn

TS:   if (!data) return;
来源：http://yuz.jqgfzy.top

Java: if (data == null) return;
来源：http://puo.shanyushiyangtech.top

Go:   if data == nil { return }
来源：http://xsc.tanke756.top

Ruby: return if data.nil?
来源：http://wjb.nanxuanxn.top

C#:   if (data == null) return;
来源：http://hta.redwolf501.top

================================================================================
来源：http://ewg.yueranfly.top

C. 函数与作用域
来源：http://rxf.chenzaomai.com

================================================================================
来源：http://sdo.vehdjk.com

[C01] 定义函数
来源：http://aht.vqdsnc.cn

Py:   def add(a, b): return a + b
来源：http://zkf.redwolf501.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qhe.cashguo.top

JS:   function add(a, b) { return a + b; }
来源：http://hoi.mhx1999.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kvy.aizwys.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://opo.chenjidiqi.icu

Go:   func add(a, b int) int { return a + b }
来源：http://cbu.hammf.cn

Ruby: def add(a, b); a + b; end
来源：http://fyv.jinqigfzy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zzu.9152youxi.cn

[C02] 默认参数
来源：http://pfc.bbcook.cn

Py:   def greet(name="World"): return name
来源：http://lkt.cheryme.top

PHP:  function greet($name = "World") { return $name; }
来源：http://iub.sysykeji.top

JS:   function greet(name = "World") { return name; }
来源：http://wmz.ybcxt.top

TS:   function greet(name: string = "World") { return name; }
来源：http://tcx.yanxiufei.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://smj.zhoulong.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://qul.pengpengdd.cyou

Ruby: def greet(name = "World") = name
来源：http://gql.ydjk.org.cn

C#:   string Greet(string name = "World") => name;
来源：http://tca.wangshuangyany.cn

[C03] 可变参数
来源：http://quq.gotoacloud.top

Py:   def total(*args): return sum(args)
来源：http://tjb.shanyushiyangkeji.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uny.zdqjudy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://dwj.sxryk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xhq.hnqzz.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lvi.yangfankeji.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gjk.hesvh.cn

Ruby: def total(*nums); nums.sum; end
来源：http://xwk.cashguo.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nma.shangyingyoupin.top

[C04] 命名参数 / 关键字参数
来源：http://vvf.fanxiaobao.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dnz.jianghu66.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fsq.aibaodan.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://yjp.yfazqb.com

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://von.ydjk.org.cn

Java: // 无：用 Builder 模式或 record
来源：http://qji.ydzc1.top

Go:   // 无：用配置结构体参数
来源：http://msx.chenlongwang.top

Ruby: f(a: 1, b: 2)
来源：http://vlq.yuanzhike.top

C#:   f(a: 1, b: 2)
来源：http://ayh.snrcjt.cn

[C05] 返回多个值
来源：http://nyx.hnxiangtu.top

Py:   return a, b
来源：http://dty.quarkkingdee.top

PHP:  return [$a, $b];
来源：http://zso.uphjek.com

JS:   return [a, b];             // 或 return { a, b };
来源：http://wxj.fktsv.cn

TS:   return { a, b };
来源：http://kui.birdmap.top


<!-- 参考信息 -->