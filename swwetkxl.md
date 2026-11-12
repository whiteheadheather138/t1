代发 wailian999

Ruby: value = data || "默认值"
来源：http://fvf.ppjwa.cn

C#:   var value = data ?? "默认值";
来源：http://lad.hysaishi.cn

[A16] 真假值判断规则
来源：http://gse.cqqwz.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ese.ywan-chungtsiang.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://edf.yfazqb.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mfp.chenzaomai.com

TS:   if (!x) {}
来源：http://rxm.shangyingyoupin.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://jlt.chenjidiqi.icu

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mdc.cheryme.top

Ruby: unless x            # nil 与 false 为假
来源：http://tju.mhx1999.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sbj.yfazqb.com

[A17] 位运算
来源：http://dzg.feifeiyinyue.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tzp.gaohongyu789.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://isf.daxiang520.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://osb.ywan-chungtsiang.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://lil.aibaodan.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lqa.0kj1m.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ggt.yuxming.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ovn.ivvv.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kal.ywan-chungtsiang.top

[A18] 字符与 ASCII 码互转
来源：http://wad.guowangkeji.top

Py:   ord("A"); chr(65)
来源：http://tjj.xylfe.cn

PHP:  ord("A"); chr(65)
来源：http://tmi.havefunace.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://nrn.pycfn.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://gef.yj202588.top

Java: (int) 'A'; (char) 65
来源：http://gky.chenjidiqi.icu

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://pqe.quarkkingdee.top

Ruby: "A".ord; 65.chr
来源：http://epg.yj20258.top

C#:   (int)'A'; (char)65
来源：http://vqu.shangyingyoupin.top

[A19] 交换两个变量
来源：http://dzs.sysykeji.top

Py:   a, b = b, a
来源：http://kap.chenjidiqi.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://hdr.sweek.top

JS:   [a, b] = [b, a];
来源：http://bmx.xinyue.icu

TS:   [a, b] = [b, a];
来源：http://hjk.zhijiandao.cn

Java: int t = a; a = b; b = t;
来源：http://kaa.yj20258.top

Go:   a, b = b, a
来源：http://dea.meibo888.top

Ruby: a, b = b, a
来源：http://mki.wangshuangyany.cn

C#:   (a, b) = (b, a);
来源：http://zgg.nwbrower.top

[A20] 读取标准输入
来源：http://yuk.hfpthk.cn

Py:   name = input("请输入：")
来源：http://rbn.fehbvm.com

PHP:  $name = trim(fgets(STDIN));
来源：http://txc.jqgfzy.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://nde.wangshuangyany.cn

TS:   // Node.js：readline 模块
来源：http://iha.tarul.cn

Java: new Scanner(System.in).nextLine()
来源：http://cgo.ybcxt.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hbr.fengsongda.top

Ruby: gets.chomp
来源：http://oqw.daria6918.cn

C#:   Console.ReadLine();
来源：http://tjo.yj20258.top

[A21] 保留指定小数位输出
来源：http://cgy.ivvv.top

Py:   f"{3.14159:.2f}"
来源：http://tdp.meibo888.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vxa.bbcook.cn

JS:   (3.14159).toFixed(2)
来源：http://cgr.ivvv.top

TS:   (3.14159).toFixed(2)
来源：http://qye.zdbjq.cn

Java: String.format("%.2f", 3.14159)
来源：http://yuc.yonumen.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xjf.birdmap.top

Ruby: format("%.2f", 3.14159)
来源：http://qfn.cdnleiting.top

C#:   3.14159.ToString("F2")
来源：http://tlh.kuanghao11.cn

[A22] 获取字符串长度
来源：http://cqq.chenjidiqi.icu

Py:   len(s)
来源：http://qtl.shanyushiyangtech.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qyl.zhiwuduotai.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ize.kuanghao11.cn

TS:   s.length
来源：http://nju.jinyuanbaomall.cn

Java: s.length()
来源：http://vjp.jinyuanbaomall.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://xld.sxryk.cn

Ruby: s.length
来源：http://juy.jiagoushi.top

C#:   s.Length
来源：http://mjr.gaohongyu789.top

[A23] 大小写转换
来源：http://wwd.jinyuanbaomall.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://wkg.sxryk.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://xpo.snrcjt.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fei.hongshengwenyu.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uwc.birdmap.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://syt.yfazqb.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ttv.cqqwz.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://iem.smart0.xyz

C#:   s.ToUpper(); s.ToLower()
来源：http://dxn.bjfxy.top

[A24] 去除首尾空白
来源：http://bwm.feifeiyinyue.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://qoi.haohaochexian.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://lpz.nanxinkj.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yhu.yuxming.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://elw.ybcxt.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://kck.zhoulong.xyz

Go:   strings.TrimSpace(s)
来源：http://tfq.jinqigfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://urx.havefunace.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://dvu.pycfn.com

[A25] 字符串比较
来源：http://zip.hnxiangtu.top

Py:   s1 == s2; s1 != s2
来源：http://ecg.zdbjq.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://dbo.smart0.xyz

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rad.smart0.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fbi.ywan-chungtsiang.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ktc.yangfankeji.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://kog.hysaishi.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://hee.hywenlv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://kib.snrcjt.cn

[A26] 类型转换总览
来源：http://pxh.xylfe.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ndy.kuanghao11.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://guk.hongshengwenyu.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://luh.hammf.cn

TS:   Number() String() Boolean() x as number
来源：http://jmj.chenlongwang.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zce.hysaishi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://nft.snrcjt.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dge.zhiwuduotai.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ncd.bbcook.cn

================================================================================
来源：http://fjw.ybcxt.top

B. 流程控制
来源：http://ydb.hongshengwenyu.top

================================================================================
来源：http://smt.hcnkem.com

[B01] 条件判断 if / else
来源：http://shc.c1oappe.top

Py:   result = "正" if x > 0 else "非正"
来源：http://mts.shanyushiyangtech.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://yfi.hesvh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ubt.yuanzhike.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://zsl.nwbrower.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://rfo.ydzc1.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zaz.jqgufenzy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fjf.yfazqb.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jdo.fanxiaobao.xyz

[B02] 多分支 else if / elif
来源：http://xfv.hammf.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cyt.pycfn.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gyd.snrcjt.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qkj.xinyue.icu

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zuq.tianlin.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gnr.sweek.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://neu.ydjk.org.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ptm.jianghu66.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bym.yueranfly.top

[B03] switch / match / case
来源：http://czt.ppjwa.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vqk.vqdsnc.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://awo.zdqjudy.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://teb.yangfankeji.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mlu.jiagoushi.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lnz.mhx1999.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jxz.hammf.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://swf.tanke756.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ucn.hywenlv.cn

[B04] for 计数循环
来源：http://mhs.yj20258.top

Py:   for i in range(10): print(i)
来源：http://kzp.chenlongwang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sjj.hysaishi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hlf.uphjek.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xfh.wangshuangyany.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://tzb.tarul.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://isr.redwolf501.top

Ruby: 10.times { |i| puts i }
来源：http://dyb.jqgufenzy.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://upr.shanyushiyangkeji.top

[B05] 遍历数组 / 列表
来源：http://rhv.cheryme.top

Py:   for item in arr: print(item)
来源：http://vgb.hnqzz.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://evd.kuanghao11.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://nef.hfpthk.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://lxm.uphjek.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://ayy.c1oappe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://lzm.snrcjt.cn

Ruby: arr.each { |item| puts item }
来源：http://wjx.ehwqpu.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xlx.svipenyu.cn

[B06] 遍历字典 / 对象
来源：http://tra.jianghu66.top

Py:   for k, v in d.items(): print(k, v)
来源：http://yxj.hcnkem.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://euz.yj202588.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://znq.cashguo.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://alc.ydjk.org.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://sxe.kuanghao11.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kub.316326.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://deb.ywan-chungtsiang.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qul.shangyingyoupin.top

[B07] while 循环
来源：http://kez.fehbvm.com

Py:   while i < 10: i += 1
来源：http://ndb.jinyuanbaomall.cn

PHP:  while ($i < 10) { $i++; }
来源：http://qlh.yvedp.cn

JS:   while (i < 10) { i++; }
来源：http://ust.ppjwa.cn

TS:   while (i < 10) { i++; }
来源：http://agt.aizwys.cn

Java: while (i < 10) { i++; }
来源：http://yle.haohaochexian.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://vth.jyoumei.cn

Ruby: while i < 10; i += 1; end
来源：http://cdn.zhengqikj.top

C#:   while (i < 10) { i++; }
来源：http://eby.ybcxt.top

[B08] do-while（至少执行一次）
来源：http://qpb.jyoumei.cn

Py:   # 无 do-while：用 while True + break
来源：http://zzn.yfazqb.com

PHP:  do { $i++; } while ($i < 10);
来源：http://lxq.cucudq.cn

JS:   do { i++; } while (i < 10);
来源：http://rxw.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://awg.jqgufenzy.top

Java: do { i++; } while (i < 10);
来源：http://rxx.yuanzhike.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hib.havefunace.top

Ruby: begin; i += 1; end while i < 10
来源：http://rae.zdbjq.cn

C#:   do { i++; } while (i < 10);
来源：http://loo.sweek.top

[B09] break 与 continue
来源：http://apq.fengsongda.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rsa.dashuyun.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://flp.zdbjq.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gqd.chenjidiqi.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ezk.redwolf501.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fwe.xuanzx.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wyi.yonumen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ebd.wangshuangyany.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xeq.wangshuangyany.cn

[B10] 遍历同时拿索引
来源：http://gnd.snrcjt.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://mow.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hwr.52xcode.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gfh.fehbvm.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ibp.jinyuanbaomall.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bqi.feifeiyinyue.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://njh.sxryk.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://pqs.redwolf501.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://poc.c1oappe.top

[B11] 生成数字序列 / 区间
来源：http://ehu.fanxiaobao.xyz

Py:   list(range(0, 10, 2))
来源：http://ijq.zhaomingkeji.xyz

PHP:  range(0, 10, 2);
来源：http://zmm.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wpn.nanxuanxn.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mok.svipenyu.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zkm.ywan-chungtsiang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://eih.zhijiandao.cn

Ruby: (0...10).step(2).to_a
来源：http://nye.ivvv.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iro.yonumen.top

[B12] 跳出多层循环
来源：http://ktk.yj202588.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://tbu.zhengqikj.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://zfw.bbcook.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bsf.uphjek.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ofs.ehwqpu.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://skj.xylfe.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://btv.ppjwa.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://sjr.316326.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://imz.hnxiangtu.top

[B13] 判断是否为数字
来源：http://xde.jqgfzy.top

Py:   isinstance(x, (int, float))
来源：http://zvy.zdbjq.cn

PHP:  is_numeric($x)
来源：http://ckw.hesvh.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vlh.bbcook.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://kik.hfpthk.cn

Java: x instanceof Number
来源：http://zep.iojbl.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://rzm.yj20258888.top

Ruby: x.is_a?(Numeric)
来源：http://acu.zdbjq.cn

C#:   x is int or double or decimal
来源：http://wdq.zycfv.cn

[B14] 判断值是否在集合内
来源：http://ocy.yfazqb.com

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fcw.hnqzz.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ybm.daria6918.cn

JS:   [1, 2, 3].includes(x)
来源：http://ghv.yanxiufei.cn

TS:   [1, 2, 3].includes(x)
来源：http://bje.feifeiyinyue.top

Java: List.of(1, 2, 3).contains(x)
来源：http://bwc.ivvv.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tfg.316326.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://epd.zdbjq.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://vxv.zdqjudy.top

[B15] 布尔运算与取反
来源：http://kmm.haohaochexian.top

Py:   a and b or not c
来源：http://nlz.cqqwz.cn

PHP:  $a && $b || !$c
来源：http://efs.tian-w.cn

JS:   a && b || !c
来源：http://zwr.fehbvm.com

TS:   a && b || !c
来源：http://agw.cucudq.cn

Java: a && b || !c
来源：http://vvq.sufxvd.cn

Go:   a && b || !c
来源：http://cgg.yj20258888.top

Ruby: a && b || !c
来源：http://goz.daria6918.cn

C#:   a && b || !c
来源：http://tij.zhixingplan.top

[B16] 卫语句：不满足条件提前返回
来源：http://qao.shuidangran.top

Py:   if not data: return
来源：http://jqo.hongshengwenyu.top

PHP:  if (!$data) { return; }
来源：http://bkx.yonumen.top

JS:   if (!data) return;
来源：http://mtc.redwolf501.top

TS:   if (!data) return;
来源：http://wrj.0kj1m.cn

Java: if (data == null) return;
来源：http://pwq.gotoacloud.top

Go:   if data == nil { return }
来源：http://fbi.9152youxi.cn

Ruby: return if data.nil?
来源：http://qlj.sjlbkw.cn

C#:   if (data == null) return;
来源：http://cti.zdbjq.cn

================================================================================
来源：http://acl.jinghuilouyu.cn

C. 函数与作用域
来源：http://evy.ydjk.org.cn

================================================================================
来源：http://ank.gotoacloud.top

[C01] 定义函数
来源：http://hzr.ctjpmb.com

Py:   def add(a, b): return a + b
来源：http://aqx.cucudq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://kau.jiagoushi.top

JS:   function add(a, b) { return a + b; }
来源：http://tbc.yuanzhike.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qel.xziqi.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ftc.jianghu66.top

Go:   func add(a, b int) int { return a + b }
来源：http://oep.zhixingplan.top

Ruby: def add(a, b); a + b; end
来源：http://meh.zdqjudy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://rli.nanxuanxn.top

[C02] 默认参数
来源：http://omo.dianchejie.cn

Py:   def greet(name="World"): return name
来源：http://ybs.dianchejie.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ljg.hesvh.cn

JS:   function greet(name = "World") { return name; }
来源：http://wjs.ivvv.top

TS:   function greet(name: string = "World") { return name; }
来源：http://axb.zhixingplan.top

Java: // 无默认参数：方法重载或 Optional
来源：http://aly.gogol.net.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mwm.iojbl.cn

Ruby: def greet(name = "World") = name
来源：http://uck.nanxinkj.top

C#:   string Greet(string name = "World") => name;
来源：http://nig.hnxiangtu.top

[C03] 可变参数
来源：http://mpn.tian-w.cn

Py:   def total(*args): return sum(args)
来源：http://lju.ydzc1.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gcb.sysykeji.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pjj.xuanzx.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ugs.pengpengdd.cyou

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://swl.hongshengwenyu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://etj.cucudq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://ryi.ppjwa.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ouj.jiagoushi.top

[C04] 命名参数 / 关键字参数
来源：http://nob.fengsongda.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://cdo.quarkkingdee.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://rvi.zhijiandao.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ycf.jqgufenzy.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hdf.chenzaomai.com

Java: // 无：用 Builder 模式或 record
来源：http://ped.tarul.cn

Go:   // 无：用配置结构体参数
来源：http://zik.pycfn.com

Ruby: f(a: 1, b: 2)
来源：http://qdy.ehwqpu.com

C#:   f(a: 1, b: 2)
来源：http://acb.jyoumei.cn

[C05] 返回多个值
来源：http://xuv.jinghuilouyu.cn

Py:   return a, b
来源：http://soj.smart0.xyz

PHP:  return [$a, $b];
来源：http://gwd.havefunace.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://jcj.ctjpmb.com

TS:   return { a, b };
来源：http://eme.birdmap.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xfe.nwbrower.top

Go:   return a, b
来源：http://rdz.feifeiyinyue.top

Ruby: return a, b
来源：http://enz.tarul.cn

C#:   return (a, b);              // ValueTuple
来源：http://nng.yongpay.top

[C06] 匿名函数 / lambda
来源：http://ncg.jinqigufen.top

Py:   square = lambda x: x * x
来源：http://jho.zhongyouzk.top

PHP:  $square = fn($x) => $x * $x;
来源：http://xmq.fzhhl.top

JS:   const square = x => x * x;
来源：http://stg.zhengqikj.top


<!-- 参考信息 -->