代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://qpx.nwbrower.top

[A15] 空值判断与默认值
来源：http://end.0kj1m.cn

Py:   value = data or "默认值"
来源：http://zbu.vqdsnc.cn

PHP:  $value = $data ?? "默认值";
来源：http://xph.jianghu66.top

JS:   const value = data ?? "默认值";
来源：http://qxw.hammf.cn

TS:   const value = data ?? "默认值";
来源：http://zzv.yonumen.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://jkf.jyoumei.cn

Go:   if data == "" { data = "默认值" }
来源：http://pky.yvedp.cn

Ruby: value = data || "默认值"
来源：http://tfz.uphjek.com

C#:   var value = data ?? "默认值";
来源：http://efg.cqqwz.cn

[A16] 真假值判断规则
来源：http://vhd.zhiwuduotai.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://zpl.jinqigfzy.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mfd.shanyushiyangkeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ubz.yj20258888.top

TS:   if (!x) {}
来源：http://mza.yanxiufei.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ooq.iojbl.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://njb.gogol.net.cn

Ruby: unless x            # nil 与 false 为假
来源：http://pcn.daxiang520.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ngq.svipenyu.cn

[A17] 位运算
来源：http://ubs.wangdashe.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://opw.dashuyun.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://nlf.chenjidiqi.icu

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://inf.zdqjudy.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jrn.quarkkingdee.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jxr.andypj.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://srz.hfpthk.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cjs.xingfuxueyuan.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mjl.zhixingplan.top

[A18] 字符与 ASCII 码互转
来源：http://wap.epnwcf.com

Py:   ord("A"); chr(65)
来源：http://zbp.bjfxy.top

PHP:  ord("A"); chr(65)
来源：http://evq.0kj1m.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://yhp.yuanzhike.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dfb.sjlbkw.cn

Java: (int) 'A'; (char) 65
来源：http://dvu.shanyushiyangtech.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pjt.gzhubu.top

Ruby: "A".ord; 65.chr
来源：http://brk.dianchejie.cn

C#:   (int)'A'; (char)65
来源：http://kkz.yonumen.top

[A19] 交换两个变量
来源：http://ehf.fzhhl.top

Py:   a, b = b, a
来源：http://hqy.jinqigufen.top

PHP:  [$a, $b] = [$b, $a];
来源：http://pxd.ydzc1.top

JS:   [a, b] = [b, a];
来源：http://gfu.cqqwz.cn

TS:   [a, b] = [b, a];
来源：http://hwn.jianghu66.top

Java: int t = a; a = b; b = t;
来源：http://cqz.havefunace.top

Go:   a, b = b, a
来源：http://swe.yanxiufei.cn

Ruby: a, b = b, a
来源：http://mki.xuanzx.com

C#:   (a, b) = (b, a);
来源：http://ixn.yj20258.top

[A20] 读取标准输入
来源：http://vcm.jiagoushi.top

Py:   name = input("请输入：")
来源：http://gan.daxiang520.top

PHP:  $name = trim(fgets(STDIN));
来源：http://kzh.nanxinkj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ihy.jinqigfzy.top

TS:   // Node.js：readline 模块
来源：http://mbp.guowangkeji.top

Java: new Scanner(System.in).nextLine()
来源：http://gql.chenjidiqi.icu

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cri.cdnleiting.top

Ruby: gets.chomp
来源：http://dmc.xziqi.cn

C#:   Console.ReadLine();
来源：http://uxu.aizwys.cn

[A21] 保留指定小数位输出
来源：http://jof.svipenyu.cn

Py:   f"{3.14159:.2f}"
来源：http://fbq.0kj1m.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://fgm.c1oappe.top

JS:   (3.14159).toFixed(2)
来源：http://saa.guannengcc.top

TS:   (3.14159).toFixed(2)
来源：http://brp.nwbrower.top

Java: String.format("%.2f", 3.14159)
来源：http://dir.fengsongda.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zye.aibaodan.cn

Ruby: format("%.2f", 3.14159)
来源：http://pbp.shuidangran.top

C#:   3.14159.ToString("F2")
来源：http://ijt.zhijiandao.cn

[A22] 获取字符串长度
来源：http://fmi.zdqjudy.top

Py:   len(s)
来源：http://zdo.0kj1m.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bpo.hesvh.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://fjp.haohaochexian.top

TS:   s.length
来源：http://ioh.ctjpmb.com

Java: s.length()
来源：http://rlf.ivvv.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://lav.jianghu66.top

Ruby: s.length
来源：http://mda.ehwqpu.com

C#:   s.Length
来源：http://sfw.shzxlz.cn

[A23] 大小写转换
来源：http://nmb.kuanghao11.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vrb.daria6918.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vni.yj20258888.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://grg.dashuyun.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rex.xuetiantiany.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sig.kuanghao11.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mcm.dashuyun.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://twf.xylfe.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://zuq.guannengcc.top

[A24] 去除首尾空白
来源：http://zsm.yj20258888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wqy.sysykeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qro.zycfv.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kqm.chenjidiqi.icu

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nmf.jiagoushi.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://zmo.nwbrower.top

Go:   strings.TrimSpace(s)
来源：http://ftv.sweek.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://mtt.zhoulong.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://gbq.xziqi.cn

[A25] 字符串比较
来源：http://kvv.zhixingplan.top

Py:   s1 == s2; s1 != s2
来源：http://sla.9152youxi.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dmn.shzxlz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zgy.kuanghao11.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://aqg.hfpthk.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ifl.shanyushiyangtech.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://yjp.jinyuanbaomall.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://wre.yj20258888.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qmn.hnqzz.top

[A26] 类型转换总览
来源：http://dih.tian-w.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dll.wangdashe.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zxl.svipenyu.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://kxv.9152youxi.cn

TS:   Number() String() Boolean() x as number
来源：http://fia.sjlbkw.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wro.sweek.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xrp.daxiang520.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://crm.ybcxt.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dbs.dianchejie.cn

================================================================================
来源：http://iji.tianlin.xyz

B. 流程控制
来源：http://cfa.quarkkingdee.top

================================================================================
来源：http://llx.bjfxy.top

[B01] 条件判断 if / else
来源：http://azq.dashuyun.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://sxc.jinghuilouyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://skf.yj20258888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://npy.mhx1999.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pcm.chenjidiqi.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://dkv.xuetiantiany.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://qnt.epnwcf.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ptl.ivvv.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rgm.haohaochexian.top

[B02] 多分支 else if / elif
来源：http://zbf.dianchejie.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fpq.xuanzx.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hbb.zycfv.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qcr.xingfuxueyuan.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pfr.9152youxi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fam.daria6918.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vvn.cheryme.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mxl.zycfv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qya.ywan-chungtsiang.top

[B03] switch / match / case
来源：http://jmp.gzhubu.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://xck.jiagoushi.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://num.ppjwa.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ypq.svipenyu.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://ciz.chenjidiqi.icu

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hdu.yj20258.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qvc.zhongyouzk.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hfy.fktsv.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://cul.guannengcc.top

[B04] for 计数循环
来源：http://zff.nwbrower.top

Py:   for i in range(10): print(i)
来源：http://hol.zdqjudy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wmc.zycfv.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rtc.ppjwa.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bgu.bjfxy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://kep.jinyuanbaomall.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ger.jlsjyb.cn

Ruby: 10.times { |i| puts i }
来源：http://pfo.sxryk.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://odo.epnwcf.com

[B05] 遍历数组 / 列表
来源：http://ztf.hesvh.cn

Py:   for item in arr: print(item)
来源：http://dbw.iojbl.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yky.fehbvm.com

JS:   for (const item of arr) { console.log(item); }
来源：http://obr.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://sug.vqdsnc.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rev.tian-w.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bhd.zdqjudy.top

Ruby: arr.each { |item| puts item }
来源：http://xdz.nwbrower.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://skx.cucudq.cn

[B06] 遍历字典 / 对象
来源：http://eyk.jinghuilouyu.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://hsl.aibaodan.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zcm.ybcxt.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qfv.0kj1m.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zqp.daxiang520.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bir.epnwcf.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xnu.mhx1999.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ttz.jinyuanbaomall.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xmn.tanke756.top

[B07] while 循环
来源：http://gis.ivvv.top

Py:   while i < 10: i += 1
来源：http://dnb.zhoulong.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://zbd.xziqi.cn

JS:   while (i < 10) { i++; }
来源：http://tyn.tian-w.cn

TS:   while (i < 10) { i++; }
来源：http://duv.tian-w.cn

Java: while (i < 10) { i++; }
来源：http://sgp.fengsongda.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jkx.hfpthk.cn

Ruby: while i < 10; i += 1; end
来源：http://tns.shanyushiyangkeji.top

C#:   while (i < 10) { i++; }
来源：http://djf.yuxming.cn

[B08] do-while（至少执行一次）
来源：http://acu.yuanzhike.top

Py:   # 无 do-while：用 while True + break
来源：http://aco.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://kum.bbcook.cn

JS:   do { i++; } while (i < 10);
来源：http://ysy.uphjek.com

TS:   do { i++; } while (i < 10);
来源：http://ebi.hywenlv.cn

Java: do { i++; } while (i < 10);
来源：http://tvr.jinqigfzy.top

Go:   for { i++; if i >= 10 { break } }
来源：http://fjy.epnwcf.com

Ruby: begin; i += 1; end while i < 10
来源：http://vxk.fehbvm.com

C#:   do { i++; } while (i < 10);
来源：http://jfa.jyoumei.cn

[B09] break 与 continue
来源：http://mru.zhaomingkeji.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xyo.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://eai.bbcook.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zah.wangshuangyany.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ljx.yuanzhike.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sif.chenlongwang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://sor.nanxinkj.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kll.dianchejie.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jgv.yangfankeji.com

[B10] 遍历同时拿索引
来源：http://rjc.wangshuangyany.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lah.jinyuanbaomall.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://uuw.ydzc1.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://smy.jinyuanbaomall.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cse.ehwqpu.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dfj.xylfe.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://phx.daxiang520.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pfz.jiagoushi.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hhz.ydzc1.top

[B11] 生成数字序列 / 区间
来源：http://qpd.guowangkeji.top

Py:   list(range(0, 10, 2))
来源：http://xnq.mhx1999.top

PHP:  range(0, 10, 2);
来源：http://tqs.nanxinkj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://sok.cheryme.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://npi.zycfv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pav.yonumen.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://yhh.cqqwz.cn

Ruby: (0...10).step(2).to_a
来源：http://enl.ppjwa.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vcu.yanxiufei.cn

[B12] 跳出多层循环
来源：http://gpf.jqgufenzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://nbn.cqqwz.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://trw.jianghu66.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zgg.iojbl.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hyp.gogol.net.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://bmd.bbcook.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nol.ydjk.org.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ggz.jlsjyb.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://qac.ywan-chungtsiang.top

[B13] 判断是否为数字
来源：http://jwy.hfpthk.cn

Py:   isinstance(x, (int, float))
来源：http://xmd.ivvv.top

PHP:  is_numeric($x)
来源：http://liq.yueranfly.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gmv.jianghu66.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://brn.feifeiyinyue.top

Java: x instanceof Number
来源：http://nxo.haohaochexian.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ptj.zhixingplan.top

Ruby: x.is_a?(Numeric)
来源：http://zgq.feifeiyinyue.top

C#:   x is int or double or decimal
来源：http://guj.yangfankeji.com

[B14] 判断值是否在集合内
来源：http://hpi.bjfxy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fed.sjlbkw.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vco.yfazqb.com

JS:   [1, 2, 3].includes(x)
来源：http://dai.jinqigufen.top

TS:   [1, 2, 3].includes(x)
来源：http://ray.ybcxt.top

Java: List.of(1, 2, 3).contains(x)
来源：http://aws.daria6918.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://srx.yj20258.top

Ruby: [1, 2, 3].include?(x)
来源：http://yot.shanyushiyangtech.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://wuh.yj202588.top

[B15] 布尔运算与取反
来源：http://mlc.tarul.cn

Py:   a and b or not c
来源：http://jsk.iojbl.cn

PHP:  $a && $b || !$c
来源：http://ztu.pycfn.com

JS:   a && b || !c
来源：http://jbv.zhoulong.xyz

TS:   a && b || !c
来源：http://vvl.epnwcf.com

Java: a && b || !c
来源：http://dto.yj20258.top

Go:   a && b || !c
来源：http://ysk.jianghu66.top

Ruby: a && b || !c
来源：http://tps.ivvv.top

C#:   a && b || !c
来源：http://nue.yfazqb.com

[B16] 卫语句：不满足条件提前返回
来源：http://fnp.vqdsnc.cn

Py:   if not data: return
来源：http://aap.aizwys.cn

PHP:  if (!$data) { return; }
来源：http://fgn.0kj1m.cn

JS:   if (!data) return;
来源：http://tgi.yj20258888.top

TS:   if (!data) return;
来源：http://cki.zdbjq.cn

Java: if (data == null) return;
来源：http://ipv.fzhhl.top

Go:   if data == nil { return }
来源：http://dih.sufxvd.cn

Ruby: return if data.nil?
来源：http://zwh.hcnkem.com

C#:   if (data == null) return;
来源：http://xfz.fzhhl.top

================================================================================
来源：http://llc.pycfn.com

C. 函数与作用域
来源：http://apu.yanxiufei.cn

================================================================================
来源：http://apc.aizwys.cn

[C01] 定义函数
来源：http://bqb.cashguo.top

Py:   def add(a, b): return a + b
来源：http://tbw.yj20258888.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ybj.sysykeji.top

JS:   function add(a, b) { return a + b; }
来源：http://kbz.zhaomingkeji.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dol.shangyingyoupin.top

Java: static int add(int a, int b) { return a + b; }
来源：http://boo.hammf.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tco.gaohongyu789.top

Ruby: def add(a, b); a + b; end
来源：http://nnh.iojbl.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://iqn.hysaishi.cn

[C02] 默认参数
来源：http://uti.fzhhl.top

Py:   def greet(name="World"): return name
来源：http://prw.bbcook.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ija.tianlin.xyz

JS:   function greet(name = "World") { return name; }
来源：http://xol.wangdashe.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bhs.redwolf501.top

Java: // 无默认参数：方法重载或 Optional
来源：http://hcn.hnxiangtu.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jkx.yangfankeji.com

Ruby: def greet(name = "World") = name
来源：http://lyn.hfpthk.cn

C#:   string Greet(string name = "World") => name;
来源：http://rzj.haohaochexian.top

[C03] 可变参数
来源：http://irl.yvedp.cn

Py:   def total(*args): return sum(args)
来源：http://bfa.sjlbkw.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://tly.wangshuangyany.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wgl.zhengqikj.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zua.cucudq.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://zzq.yfazqb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ezq.shanyushiyangkeji.top

Ruby: def total(*nums); nums.sum; end
来源：http://oer.xinyue.icu

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jfd.pycfn.com

[C04] 命名参数 / 关键字参数
来源：http://rjc.gaohongyu789.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://aby.redwolf501.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ukq.zhixingplan.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://msv.svipenyu.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://eyo.jinghuilouyu.cn

Java: // 无：用 Builder 模式或 record
来源：http://xdv.havefunace.top

Go:   // 无：用配置结构体参数
来源：http://uoa.wangshuangyany.cn

Ruby: f(a: 1, b: 2)
来源：http://jui.ywan-chungtsiang.top

C#:   f(a: 1, b: 2)
来源：http://glg.cqqwz.cn

[C05] 返回多个值
来源：http://nqm.pycfn.com

Py:   return a, b
来源：http://xjr.gaohongyu789.top

PHP:  return [$a, $b];
来源：http://alm.yuxming.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://pcq.mhx1999.top

TS:   return { a, b };
来源：http://ohg.shanyushiyangkeji.top


<!-- 参考信息 -->