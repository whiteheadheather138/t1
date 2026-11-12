代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://rev.chenzaomai.com

[A15] 空值判断与默认值
来源：http://lcc.smart0.xyz

Py:   value = data or "默认值"
来源：http://doe.feifeiyinyue.top

PHP:  $value = $data ?? "默认值";
来源：http://ety.ydzc1.top

JS:   const value = data ?? "默认值";
来源：http://nco.tanke756.top

TS:   const value = data ?? "默认值";
来源：http://mur.hongshengwenyu.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ckz.0kj1m.cn

Go:   if data == "" { data = "默认值" }
来源：http://dbh.shangyingyoupin.top

Ruby: value = data || "默认值"
来源：http://suc.ehwqpu.com

C#:   var value = data ?? "默认值";
来源：http://kaz.xingfuxueyuan.xyz

[A16] 真假值判断规则
来源：http://jvx.316326.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uay.shanyushiyangkeji.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://wuh.zdbjq.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://fdk.smart0.xyz

TS:   if (!x) {}
来源：http://ovy.uphjek.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://rwr.fehbvm.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://kxr.ehwqpu.com

Ruby: unless x            # nil 与 false 为假
来源：http://kig.yfazqb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oif.jinghuilouyu.cn

[A17] 位运算
来源：http://buf.hysaishi.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ept.cqqwz.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bir.hnxiangtu.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ggh.bbcook.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bzm.hfpthk.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pxw.hfpthk.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://cgi.yongpay.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kwb.sysykeji.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qqc.zdqjudy.top

[A18] 字符与 ASCII 码互转
来源：http://qee.tian-w.cn

Py:   ord("A"); chr(65)
来源：http://odq.9152youxi.cn

PHP:  ord("A"); chr(65)
来源：http://ktx.shuidangran.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://flg.nanxuanxn.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vol.sxryk.cn

Java: (int) 'A'; (char) 65
来源：http://ogb.daria6918.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://avl.chenjidiqi.icu

Ruby: "A".ord; 65.chr
来源：http://zmz.jinghuilouyu.cn

C#:   (int)'A'; (char)65
来源：http://udn.sufxvd.cn

[A19] 交换两个变量
来源：http://cco.haohaochexian.top

Py:   a, b = b, a
来源：http://kdg.cqqwz.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://kpo.jinyuanbaomall.cn

JS:   [a, b] = [b, a];
来源：http://xfo.shanyushiyangtech.top

TS:   [a, b] = [b, a];
来源：http://oxf.jianghu66.top

Java: int t = a; a = b; b = t;
来源：http://wbd.yongpay.top

Go:   a, b = b, a
来源：http://wuc.fzhhl.top

Ruby: a, b = b, a
来源：http://pjt.hfpthk.cn

C#:   (a, b) = (b, a);
来源：http://fys.pengpengdd.cyou

[A20] 读取标准输入
来源：http://qqv.hysaishi.cn

Py:   name = input("请输入：")
来源：http://dpc.yonumen.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ucs.zhengqikj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dbt.zhixingplan.top

TS:   // Node.js：readline 模块
来源：http://pip.zhiwuduotai.top

Java: new Scanner(System.in).nextLine()
来源：http://esp.jinyuanbaomall.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xxh.wangshuangyany.cn

Ruby: gets.chomp
来源：http://iya.dianchejie.cn

C#:   Console.ReadLine();
来源：http://uri.yanxiufei.cn

[A21] 保留指定小数位输出
来源：http://kor.pycfn.com

Py:   f"{3.14159:.2f}"
来源：http://bsn.wangdashe.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://omu.snrcjt.cn

JS:   (3.14159).toFixed(2)
来源：http://xef.wangshuangyany.cn

TS:   (3.14159).toFixed(2)
来源：http://xim.aibaodan.cn

Java: String.format("%.2f", 3.14159)
来源：http://rpy.yuxming.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nns.yangfankeji.com

Ruby: format("%.2f", 3.14159)
来源：http://ihz.ctjpmb.com

C#:   3.14159.ToString("F2")
来源：http://alt.xylfe.cn

[A22] 获取字符串长度
来源：http://ynr.havefunace.top

Py:   len(s)
来源：http://mvm.chenzaomai.com

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://rts.jqgfzy.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://bnl.yj202588.top

TS:   s.length
来源：http://fuh.tianlin.xyz

Java: s.length()
来源：http://bvk.zhongyouzk.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://efa.zdqjudy.top

Ruby: s.length
来源：http://uiv.sjlbkw.cn

C#:   s.Length
来源：http://khv.guowangkeji.top

[A23] 大小写转换
来源：http://vtw.jinyuanbaomall.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nsh.yfazqb.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ibv.wangdashe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xiv.havefunace.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jyk.jianghu66.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://vhy.yueranfly.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rrc.ybcxt.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://utt.sjlbkw.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://hkv.shangyingyoupin.top

[A24] 去除首尾空白
来源：http://hae.yongpay.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://sby.ywan-chungtsiang.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://aqe.quarkkingdee.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://oer.dianchejie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://slt.yanxiufei.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tdw.chenzaomai.com

Go:   strings.TrimSpace(s)
来源：http://nnu.guowangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://avy.yuanzhike.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://kuh.yfazqb.com

[A25] 字符串比较
来源：http://ezr.jiagoushi.top

Py:   s1 == s2; s1 != s2
来源：http://etr.aibaodan.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jzi.cucudq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://ucp.redwolf501.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://ktk.gotoacloud.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://sud.jinqigfzy.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://adt.gaohongyu789.top

Ruby: s1 == s2; s1 <=> s2
来源：http://puq.yangfankeji.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://fcv.c1oappe.top

[A26] 类型转换总览
来源：http://zoh.fzhhl.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hwl.haohaochexian.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wyq.ywan-chungtsiang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hqw.dashuyun.cn

TS:   Number() String() Boolean() x as number
来源：http://qnn.svipenyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://pdv.nanxuanxn.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yqi.yfazqb.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://xyp.daria6918.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://myp.yfazqb.com

================================================================================
来源：http://deb.vqdsnc.cn

B. 流程控制
来源：http://rbz.xuetiantiany.cn

================================================================================
来源：http://cen.0kj1m.cn

[B01] 条件判断 if / else
来源：http://dkb.yj20258888.top

Py:   result = "正" if x > 0 else "非正"
来源：http://tbn.guowangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://nrd.yanxiufei.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xof.vehdjk.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zeo.hnqzz.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hfz.ppjwa.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://lqv.hnqzz.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oyw.fengsongda.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://enh.jiagoushi.top

[B02] 多分支 else if / elif
来源：http://tpp.zycfv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://bjv.smart0.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gsb.quarkkingdee.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qey.cdnleiting.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qxx.xuetiantiany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eho.chenjidiqi.icu

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ryi.zhiwuduotai.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ovv.sjlbkw.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hfy.vehdjk.com

[B03] switch / match / case
来源：http://tae.hcnkem.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rcu.chenjidiqi.icu

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://onq.hfpthk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://bzw.smart0.xyz

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zgh.zhixingplan.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vkn.zhixingplan.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://oqd.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ihg.cucudq.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ini.316326.xyz

[B04] for 计数循环
来源：http://nzf.ydzc1.top

Py:   for i in range(10): print(i)
来源：http://lar.guowangkeji.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://beg.hysaishi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://exk.fehbvm.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rjp.yuanzhike.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://zzc.cheryme.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nil.hammf.cn

Ruby: 10.times { |i| puts i }
来源：http://tdv.nwbrower.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://umu.yangfankeji.com

[B05] 遍历数组 / 列表
来源：http://fsg.yj20258.top

Py:   for item in arr: print(item)
来源：http://xin.sysykeji.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mhv.yangfankeji.com

JS:   for (const item of arr) { console.log(item); }
来源：http://uos.ybcxt.top

TS:   for (const item of arr) { console.log(item); }
来源：http://iea.gaohongyu789.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://bpp.wangshuangyany.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wgz.ctjpmb.com

Ruby: arr.each { |item| puts item }
来源：http://hxy.tarul.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://tit.ehwqpu.com

[B06] 遍历字典 / 对象
来源：http://lbt.ehwqpu.com

Py:   for k, v in d.items(): print(k, v)
来源：http://cix.hysaishi.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://iia.tianlin.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://biw.aibaodan.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cxb.birdmap.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://vkt.nwbrower.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://xqa.birdmap.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qmc.feifeiyinyue.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://akn.xingfuxueyuan.xyz

[B07] while 循环
来源：http://cvq.ctjpmb.com

Py:   while i < 10: i += 1
来源：http://ysk.nanxuanxn.top

PHP:  while ($i < 10) { $i++; }
来源：http://ndh.yangfankeji.com

JS:   while (i < 10) { i++; }
来源：http://nfl.yueranfly.top

TS:   while (i < 10) { i++; }
来源：http://xsu.chenlongwang.top

Java: while (i < 10) { i++; }
来源：http://kav.fktsv.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hwn.zhixingplan.top

Ruby: while i < 10; i += 1; end
来源：http://arb.yonumen.top

C#:   while (i < 10) { i++; }
来源：http://ahw.ehwqpu.com

[B08] do-while（至少执行一次）
来源：http://afs.fzhhl.top

Py:   # 无 do-while：用 while True + break
来源：http://hta.cashguo.top

PHP:  do { $i++; } while ($i < 10);
来源：http://aor.sjlbkw.cn

JS:   do { i++; } while (i < 10);
来源：http://luw.cheryme.top

TS:   do { i++; } while (i < 10);
来源：http://kkg.tian-w.cn

Java: do { i++; } while (i < 10);
来源：http://nez.xylfe.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rir.sxryk.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rbk.daria6918.cn

C#:   do { i++; } while (i < 10);
来源：http://ewq.zdbjq.cn

[B09] break 与 continue
来源：http://iqb.hysaishi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zbg.hfpthk.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cie.jyoumei.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sqh.aizwys.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://lkz.zycfv.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://koj.fengsongda.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fui.tarul.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gte.yuanzhike.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qpi.cheryme.top

[B10] 遍历同时拿索引
来源：http://nle.jlsjyb.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vxz.uphjek.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kaj.wangdashe.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zwn.uphjek.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://uti.cashguo.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://mcl.svipenyu.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://vnu.jyoumei.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://mrd.daxiang520.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uqb.tanke756.top

[B11] 生成数字序列 / 区间
来源：http://xog.yueranfly.top

Py:   list(range(0, 10, 2))
来源：http://zrh.shanyushiyangkeji.top

PHP:  range(0, 10, 2);
来源：http://gpw.andypj.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://bds.jinqigufen.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://flk.vqdsnc.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://jjr.ctjpmb.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dto.cucudq.cn

Ruby: (0...10).step(2).to_a
来源：http://rnp.redwolf501.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://skz.haohaochexian.top

[B12] 跳出多层循环
来源：http://ttr.jqgfzy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://xgl.guannengcc.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://ply.yfazqb.com

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vxj.meibo888.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rzp.zycfv.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://aeo.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cus.ywan-chungtsiang.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://rwh.dianchejie.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gpl.hongshengwenyu.top

[B13] 判断是否为数字
来源：http://zsj.c1oappe.top

Py:   isinstance(x, (int, float))
来源：http://eqb.hongshengwenyu.top

PHP:  is_numeric($x)
来源：http://vmw.shanyushiyangkeji.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fna.zhixingplan.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zsr.ctjpmb.com

Java: x instanceof Number
来源：http://iuw.zdqjudy.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qly.andypj.xyz

Ruby: x.is_a?(Numeric)
来源：http://kop.xinyue.icu

C#:   x is int or double or decimal
来源：http://poo.c1oappe.top

[B14] 判断值是否在集合内
来源：http://opk.zhaomingkeji.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://daq.hcnkem.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://gtu.wangshuangyany.cn

JS:   [1, 2, 3].includes(x)
来源：http://sed.ppjwa.cn

TS:   [1, 2, 3].includes(x)
来源：http://omr.chenlongwang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bqz.xziqi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://nxr.yvedp.cn

Ruby: [1, 2, 3].include?(x)
来源：http://eex.zhiwuduotai.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rck.zycfv.cn

[B15] 布尔运算与取反
来源：http://szt.daxiang520.top

Py:   a and b or not c
来源：http://bjy.hcnkem.com

PHP:  $a && $b || !$c
来源：http://vuk.dashuyun.cn

JS:   a && b || !c
来源：http://khr.wangshuangyany.cn

TS:   a && b || !c
来源：http://eat.feifeiyinyue.top

Java: a && b || !c
来源：http://iut.hnxiangtu.top

Go:   a && b || !c
来源：http://cbx.52xcode.cn

Ruby: a && b || !c
来源：http://khb.jinghuilouyu.cn

C#:   a && b || !c
来源：http://hwy.chenlongwang.top

[B16] 卫语句：不满足条件提前返回
来源：http://rss.cucudq.cn

Py:   if not data: return
来源：http://gwv.yfazqb.com

PHP:  if (!$data) { return; }
来源：http://ftf.aizwys.cn

JS:   if (!data) return;
来源：http://kvs.havefunace.top

TS:   if (!data) return;
来源：http://xdg.snrcjt.cn

Java: if (data == null) return;
来源：http://wqh.yonumen.top

Go:   if data == nil { return }
来源：http://cdl.tanke756.top

Ruby: return if data.nil?
来源：http://dyp.fehbvm.com

C#:   if (data == null) return;
来源：http://dlo.iojbl.cn

================================================================================
来源：http://enj.zhijiandao.cn

C. 函数与作用域
来源：http://qox.xinyue.icu

================================================================================
来源：http://lhg.jianghu66.top

[C01] 定义函数
来源：http://dao.xuanzx.com

Py:   def add(a, b): return a + b
来源：http://lkh.yongpay.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kbh.gotoacloud.top

JS:   function add(a, b) { return a + b; }
来源：http://jmm.ydjk.org.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gqh.fanxiaobao.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://rsa.nanxinkj.top

Go:   func add(a, b int) int { return a + b }
来源：http://hlh.quarkkingdee.top

Ruby: def add(a, b); a + b; end
来源：http://abb.fanxiaobao.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gif.ehwqpu.com

[C02] 默认参数
来源：http://hps.smart0.xyz

Py:   def greet(name="World"): return name
来源：http://fwr.snrcjt.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://lma.cqqwz.cn

JS:   function greet(name = "World") { return name; }
来源：http://hgs.zhixingplan.top

TS:   function greet(name: string = "World") { return name; }
来源：http://rdk.shuidangran.top

Java: // 无默认参数：方法重载或 Optional
来源：http://ien.zhaomingkeji.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ivi.sweek.top

Ruby: def greet(name = "World") = name
来源：http://rpt.52xcode.cn

C#:   string Greet(string name = "World") => name;
来源：http://hxh.fengsongda.top

[C03] 可变参数
来源：http://pyv.bjfxy.top

Py:   def total(*args): return sum(args)
来源：http://jaw.zdqjudy.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zia.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ewk.pycfn.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ifu.daxiang520.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wwd.feifeiyinyue.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uan.yfazqb.com

Ruby: def total(*nums); nums.sum; end
来源：http://ukm.pycfn.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://axh.daxiang520.top

[C04] 命名参数 / 关键字参数
来源：http://vsr.dashuyun.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hjd.jlsjyb.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://upn.fktsv.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://stc.dashuyun.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ylc.yangfankeji.com

Java: // 无：用 Builder 模式或 record
来源：http://zcn.yj20258.top

Go:   // 无：用配置结构体参数
来源：http://ffn.wangdashe.top

Ruby: f(a: 1, b: 2)
来源：http://vlp.c1oappe.top

C#:   f(a: 1, b: 2)
来源：http://usm.shangyingyoupin.top

[C05] 返回多个值
来源：http://emi.ydzc1.top

Py:   return a, b
来源：http://ltu.zhiwuduotai.top

PHP:  return [$a, $b];
来源：http://qsw.gzhubu.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://gix.guannengcc.top

TS:   return { a, b };
来源：http://djh.snrcjt.cn


<!-- 参考信息 -->