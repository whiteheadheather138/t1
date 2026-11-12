代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://edy.ydjk.org.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lre.sxryk.cn

Go:   // 单行；/* 多行 */
来源：http://ehh.sjlbkw.cn

Ruby: # 单行；=begin 多行 =end
来源：http://res.gzhubu.top

C#:   // 单行；/* 多行 */
来源：http://wqb.cheryme.top

[A15] 空值判断与默认值
来源：http://acy.cheryme.top

Py:   value = data or "默认值"
来源：http://ckw.chenjidiqi.icu

PHP:  $value = $data ?? "默认值";
来源：http://ctb.zhoulong.xyz

JS:   const value = data ?? "默认值";
来源：http://ejc.zhaomingkeji.xyz

TS:   const value = data ?? "默认值";
来源：http://lca.sysykeji.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jko.xylfe.cn

Go:   if data == "" { data = "默认值" }
来源：http://vat.nanxuanxn.top

Ruby: value = data || "默认值"
来源：http://fwn.52xcode.cn

C#:   var value = data ?? "默认值";
来源：http://gjl.yongpay.top

[A16] 真假值判断规则
来源：http://idw.sysykeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://tib.yvedp.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://xau.fehbvm.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://pig.gzhubu.top

TS:   if (!x) {}
来源：http://lth.tianlin.xyz

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://cvp.nanxinkj.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dtx.kuanghao11.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ybb.bjfxy.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://xbr.fehbvm.com

[A17] 位运算
来源：http://lem.fehbvm.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lre.ybcxt.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hvv.hnqzz.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mst.yvedp.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ggu.jinyuanbaomall.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fbm.tarul.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://bka.zycfv.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://exo.xziqi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://uze.chenlongwang.top

[A18] 字符与 ASCII 码互转
来源：http://qcj.cashguo.top

Py:   ord("A"); chr(65)
来源：http://smn.guannengcc.top

PHP:  ord("A"); chr(65)
来源：http://lit.jinyuanbaomall.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://zdv.guowangkeji.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mac.yuxming.cn

Java: (int) 'A'; (char) 65
来源：http://qnw.yonumen.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://gpb.gogol.net.cn

Ruby: "A".ord; 65.chr
来源：http://gnq.jinyuanbaomall.cn

C#:   (int)'A'; (char)65
来源：http://qkg.tanke756.top

[A19] 交换两个变量
来源：http://fnr.gotoacloud.top

Py:   a, b = b, a
来源：http://zvj.hysaishi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://eas.fktsv.cn

JS:   [a, b] = [b, a];
来源：http://qms.xingfuxueyuan.xyz

TS:   [a, b] = [b, a];
来源：http://xdo.wangshuangyany.cn

Java: int t = a; a = b; b = t;
来源：http://shh.9152youxi.cn

Go:   a, b = b, a
来源：http://cfu.ppjwa.cn

Ruby: a, b = b, a
来源：http://iju.iojbl.cn

C#:   (a, b) = (b, a);
来源：http://bwc.fzhhl.top

[A20] 读取标准输入
来源：http://luw.yj202588.top

Py:   name = input("请输入：")
来源：http://gfx.yj20258.top

PHP:  $name = trim(fgets(STDIN));
来源：http://usl.zycfv.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://fym.shanyushiyangtech.top

TS:   // Node.js：readline 模块
来源：http://bjg.uphjek.com

Java: new Scanner(System.in).nextLine()
来源：http://vkv.zhiwuduotai.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ajt.ybcxt.top

Ruby: gets.chomp
来源：http://hgy.ydzc1.top

C#:   Console.ReadLine();
来源：http://vmu.yanxiufei.cn

[A21] 保留指定小数位输出
来源：http://bbf.zdbjq.cn

Py:   f"{3.14159:.2f}"
来源：http://bwf.yuanzhike.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://oaj.ywan-chungtsiang.top

JS:   (3.14159).toFixed(2)
来源：http://dpn.vqdsnc.cn

TS:   (3.14159).toFixed(2)
来源：http://ahq.pycfn.com

Java: String.format("%.2f", 3.14159)
来源：http://ncj.gaohongyu789.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://gcz.havefunace.top

Ruby: format("%.2f", 3.14159)
来源：http://wws.zhijiandao.cn

C#:   3.14159.ToString("F2")
来源：http://pvl.zhiwuduotai.top

[A22] 获取字符串长度
来源：http://ptw.hywenlv.cn

Py:   len(s)
来源：http://tbk.yanxiufei.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ajr.zdbjq.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bdd.jinqigufen.top

TS:   s.length
来源：http://xos.jiagoushi.top

Java: s.length()
来源：http://gzn.aibaodan.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hwu.nwbrower.top

Ruby: s.length
来源：http://vkv.fehbvm.com

C#:   s.Length
来源：http://xuz.ydzc1.top

[A23] 大小写转换
来源：http://ppa.fanxiaobao.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://gvh.quarkkingdee.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rna.sufxvd.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://uch.redwolf501.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ahk.hysaishi.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://rgo.ctjpmb.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mrd.xuetiantiany.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lnb.shuidangran.top

C#:   s.ToUpper(); s.ToLower()
来源：http://isa.sysykeji.top

[A24] 去除首尾空白
来源：http://knw.fehbvm.com

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://zaa.cheryme.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zyq.aizwys.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vyn.fzhhl.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xzg.yongpay.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ezg.shanyushiyangkeji.top

Go:   strings.TrimSpace(s)
来源：http://yut.xuetiantiany.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ocz.hywenlv.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ela.hnxiangtu.top

[A25] 字符串比较
来源：http://dit.hywenlv.cn

Py:   s1 == s2; s1 != s2
来源：http://gkf.yfazqb.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jub.daria6918.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://gkm.hesvh.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://kkm.zhaomingkeji.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xms.zhaomingkeji.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lqw.ehwqpu.com

Ruby: s1 == s2; s1 <=> s2
来源：http://qtn.fktsv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://cmr.daxiang520.top

[A26] 类型转换总览
来源：http://xzx.quarkkingdee.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://pvt.xinyue.icu

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://our.fktsv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zxu.gaohongyu789.top

TS:   Number() String() Boolean() x as number
来源：http://mcr.chenzaomai.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ilk.tarul.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://ekq.dashuyun.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://pnu.hammf.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hlt.bbcook.cn

================================================================================
来源：http://hqn.aizwys.cn

B. 流程控制
来源：http://mtd.aizwys.cn

================================================================================
来源：http://bic.pycfn.com

[B01] 条件判断 if / else
来源：http://bow.nanxuanxn.top

Py:   result = "正" if x > 0 else "非正"
来源：http://bye.jqgfzy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://czk.yuanzhike.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yrh.yvedp.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kuu.ehwqpu.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://rvi.xuetiantiany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bws.jlsjyb.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jty.gogol.net.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://psh.epnwcf.com

[B02] 多分支 else if / elif
来源：http://kox.chenlongwang.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://eyd.316326.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rbf.yanxiufei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jgw.nwbrower.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://chm.fengsongda.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uqz.fanxiaobao.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ctg.yonumen.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://eol.jinqigfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://heh.feifeiyinyue.top

[B03] switch / match / case
来源：http://saa.sxryk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mvo.pycfn.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kwh.zdbjq.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://exp.gaohongyu789.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gxn.tarul.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://plm.hesvh.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nqd.jiagoushi.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://eel.yj20258.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zoj.zhijiandao.cn

[B04] for 计数循环
来源：http://geu.jyoumei.cn

Py:   for i in range(10): print(i)
来源：http://xel.havefunace.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://klp.zdbjq.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mpl.vqdsnc.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zrq.tanke756.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://rqs.nanxinkj.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nkk.pycfn.com

Ruby: 10.times { |i| puts i }
来源：http://qcp.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://sev.c1oappe.top

[B05] 遍历数组 / 列表
来源：http://mmt.0kj1m.cn

Py:   for item in arr: print(item)
来源：http://ebk.ydjk.org.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lmj.tianlin.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://fqc.fktsv.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://bay.zhixingplan.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://rzp.havefunace.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://iyt.haohaochexian.top

Ruby: arr.each { |item| puts item }
来源：http://woy.meibo888.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wli.jinqigufen.top

[B06] 遍历字典 / 对象
来源：http://ubh.dashuyun.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tcm.hnqzz.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://cfg.hesvh.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ndw.tian-w.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wrk.ybcxt.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://nku.xylfe.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ptj.zhoulong.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://fqz.jinyuanbaomall.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mva.yuanzhike.top

[B07] while 循环
来源：http://phs.yongpay.top

Py:   while i < 10: i += 1
来源：http://mnm.hammf.cn

PHP:  while ($i < 10) { $i++; }
来源：http://rfw.haohaochexian.top

JS:   while (i < 10) { i++; }
来源：http://zan.jyoumei.cn

TS:   while (i < 10) { i++; }
来源：http://tog.jqgufenzy.top

Java: while (i < 10) { i++; }
来源：http://qyy.zhoulong.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nbf.xingfuxueyuan.xyz

Ruby: while i < 10; i += 1; end
来源：http://ohf.yonumen.top

C#:   while (i < 10) { i++; }
来源：http://jql.zhoulong.xyz

[B08] do-while（至少执行一次）
来源：http://ect.zdqjudy.top

Py:   # 无 do-while：用 while True + break
来源：http://smc.svipenyu.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://dbl.gogol.net.cn

JS:   do { i++; } while (i < 10);
来源：http://bqk.ybcxt.top

TS:   do { i++; } while (i < 10);
来源：http://inm.yj20258.top

Java: do { i++; } while (i < 10);
来源：http://qkm.tian-w.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://grp.daria6918.cn

Ruby: begin; i += 1; end while i < 10
来源：http://lvi.hesvh.cn

C#:   do { i++; } while (i < 10);
来源：http://pbd.hcnkem.com

[B09] break 与 continue
来源：http://mhf.xuanzx.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jrs.ywan-chungtsiang.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hsj.daria6918.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wtu.wangdashe.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://eni.chenzaomai.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vzw.dianchejie.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fba.kuanghao11.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dmx.quarkkingdee.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qvj.andypj.xyz

[B10] 遍历同时拿索引
来源：http://svq.shangyingyoupin.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fet.pengpengdd.cyou

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rdq.dashuyun.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://owz.gogol.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://vjs.xuanzx.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vai.yj202588.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vwh.yuxming.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://toq.tarul.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jil.tian-w.cn

[B11] 生成数字序列 / 区间
来源：http://ppm.yj202588.top

Py:   list(range(0, 10, 2))
来源：http://zni.pycfn.com

PHP:  range(0, 10, 2);
来源：http://iac.ivvv.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://izw.c1oappe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://cew.guowangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nrj.yanxiufei.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kvm.sufxvd.cn

Ruby: (0...10).step(2).to_a
来源：http://cnw.tianlin.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://pfl.ybcxt.top

[B12] 跳出多层循环
来源：http://xrb.zhijiandao.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://wsj.zhixingplan.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ovn.shangyingyoupin.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xtx.zhoulong.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ooa.c1oappe.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://dwb.hnqzz.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kxn.kuanghao11.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wlp.tarul.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://rse.316326.xyz

[B13] 判断是否为数字
来源：http://cjh.jqgufenzy.top

Py:   isinstance(x, (int, float))
来源：http://vcb.birdmap.top

PHP:  is_numeric($x)
来源：http://snd.fengsongda.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://asy.cheryme.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dhy.iojbl.cn

Java: x instanceof Number
来源：http://hfa.svipenyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vfc.hfpthk.cn

Ruby: x.is_a?(Numeric)
来源：http://nut.daxiang520.top

C#:   x is int or double or decimal
来源：http://wxc.yongpay.top

[B14] 判断值是否在集合内
来源：http://hdl.yongpay.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yqs.ydjk.org.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lbg.bbcook.cn

JS:   [1, 2, 3].includes(x)
来源：http://hdy.cashguo.top

TS:   [1, 2, 3].includes(x)
来源：http://gvg.zhiwuduotai.top

Java: List.of(1, 2, 3).contains(x)
来源：http://kcg.fehbvm.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://jsn.9152youxi.cn

Ruby: [1, 2, 3].include?(x)
来源：http://gnp.kuanghao11.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dmj.hcnkem.com

[B15] 布尔运算与取反
来源：http://ikc.zhoulong.xyz

Py:   a and b or not c
来源：http://zno.shangyingyoupin.top

PHP:  $a && $b || !$c
来源：http://euz.bjfxy.top

JS:   a && b || !c
来源：http://eso.wangshuangyany.cn

TS:   a && b || !c
来源：http://znb.jqgufenzy.top

Java: a && b || !c
来源：http://jqa.shanyushiyangkeji.top

Go:   a && b || !c
来源：http://kpe.cashguo.top

Ruby: a && b || !c
来源：http://mqe.yuxming.cn

C#:   a && b || !c
来源：http://rvn.jqgufenzy.top

[B16] 卫语句：不满足条件提前返回
来源：http://lbx.hcnkem.com

Py:   if not data: return
来源：http://rxd.ehwqpu.com

PHP:  if (!$data) { return; }
来源：http://wnc.fanxiaobao.xyz

JS:   if (!data) return;
来源：http://xty.gaohongyu789.top

TS:   if (!data) return;
来源：http://dsq.yfazqb.com

Java: if (data == null) return;
来源：http://tuy.ydzc1.top

Go:   if data == nil { return }
来源：http://dvf.hfpthk.cn

Ruby: return if data.nil?
来源：http://qpv.jianghu66.top

C#:   if (data == null) return;
来源：http://soh.jinqigufen.top

================================================================================
来源：http://nwo.yj202588.top

C. 函数与作用域
来源：http://vhl.0kj1m.cn

================================================================================
来源：http://yox.sweek.top

[C01] 定义函数
来源：http://utc.gogol.net.cn

Py:   def add(a, b): return a + b
来源：http://atz.meibo888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ini.shanyushiyangtech.top

JS:   function add(a, b) { return a + b; }
来源：http://odw.zhongyouzk.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://iyw.guowangkeji.top

Java: static int add(int a, int b) { return a + b; }
来源：http://eon.zycfv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hkg.zhixingplan.top

Ruby: def add(a, b); a + b; end
来源：http://mhg.quarkkingdee.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vuz.andypj.xyz

[C02] 默认参数
来源：http://ubk.ydzc1.top

Py:   def greet(name="World"): return name
来源：http://iqr.hammf.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://mom.dashuyun.cn

JS:   function greet(name = "World") { return name; }
来源：http://zri.jyoumei.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://wtt.quarkkingdee.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ybq.tian-w.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ary.yueranfly.top

Ruby: def greet(name = "World") = name
来源：http://ywa.yongpay.top

C#:   string Greet(string name = "World") => name;
来源：http://fij.yueranfly.top

[C03] 可变参数
来源：http://nek.9152youxi.cn

Py:   def total(*args): return sum(args)
来源：http://dof.zdqjudy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://owm.shangyingyoupin.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://vpb.hesvh.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://crc.jinqigufen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ive.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tlk.xylfe.cn

Ruby: def total(*nums); nums.sum; end
来源：http://aae.xingfuxueyuan.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://usm.xinyue.icu

[C04] 命名参数 / 关键字参数
来源：http://vdb.xziqi.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dtq.shzxlz.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eos.yj202588.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vqy.xingfuxueyuan.xyz

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wou.nwbrower.top

Java: // 无：用 Builder 模式或 record
来源：http://dpf.yanxiufei.cn

Go:   // 无：用配置结构体参数
来源：http://wyx.hysaishi.cn

Ruby: f(a: 1, b: 2)
来源：http://fhr.zhongyouzk.top

C#:   f(a: 1, b: 2)
来源：http://drt.jinghuilouyu.cn

[C05] 返回多个值
来源：http://adv.yvedp.cn


<!-- 参考信息 -->