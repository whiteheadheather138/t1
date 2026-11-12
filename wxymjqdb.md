代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://vlq.wangshuangyany.cn

Ruby: "Hello, #{name}!"
来源：http://zpm.fehbvm.com

C#:   $"Hello, {name}!"
来源：http://uyg.fanxiaobao.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://cwz.cashguo.top

Py:   "第一行\n第二行"
来源：http://psb.aibaodan.cn

PHP:  "第一行\n第二行"
来源：http://mus.jinqigufen.top

JS:   "第一行\n第二行"
来源：http://xvk.shangyingyoupin.top

TS:   "第一行\n第二行"
来源：http://elf.havefunace.top

Java: "第一行\n第二行"
来源：http://bms.hywenlv.cn

Go:   "第一行\n第二行"
来源：http://yes.yj20258.top

Ruby: "第一行\n第二行"
来源：http://laj.vqdsnc.cn

C#:   "第一行\n第二行"
来源：http://qau.316326.xyz

[A14] 注释写法
来源：http://wcj.fktsv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://swj.gogol.net.cn

PHP:  // 或 # 单行；/* 多行 */
来源：http://yke.jinqigufen.top

JS:   // 单行；/* 多行 */
来源：http://wre.bbcook.cn

TS:   // 单行；/* 多行 */
来源：http://fyn.tianlin.xyz

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://iwn.ivvv.top

Go:   // 单行；/* 多行 */
来源：http://xvx.yfazqb.com

Ruby: # 单行；=begin 多行 =end
来源：http://bju.zhongyouzk.top

C#:   // 单行；/* 多行 */
来源：http://oca.zhiwuduotai.top

[A15] 空值判断与默认值
来源：http://tmm.zhixingplan.top

Py:   value = data or "默认值"
来源：http://xxp.snrcjt.cn

PHP:  $value = $data ?? "默认值";
来源：http://zsg.jqgfzy.top

JS:   const value = data ?? "默认值";
来源：http://yqf.yanxiufei.cn

TS:   const value = data ?? "默认值";
来源：http://tpx.wangdashe.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wmj.jqgfzy.top

Go:   if data == "" { data = "默认值" }
来源：http://hcu.chenlongwang.top

Ruby: value = data || "默认值"
来源：http://vsq.fehbvm.com

C#:   var value = data ?? "默认值";
来源：http://bgl.redwolf501.top

[A16] 真假值判断规则
来源：http://ioh.sweek.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://kye.daria6918.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mha.yonumen.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://zqc.cucudq.cn

TS:   if (!x) {}
来源：http://slm.tanke756.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://fvt.fzhhl.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://xkt.yongpay.top

Ruby: unless x            # nil 与 false 为假
来源：http://iib.zhiwuduotai.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://nit.zhijiandao.cn

[A17] 位运算
来源：http://mvx.c1oappe.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qee.yangfankeji.com

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://umg.shanyushiyangtech.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gob.jiagoushi.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bop.jiagoushi.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://efj.hammf.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://uub.52xcode.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://evc.zdqjudy.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yse.meibo888.top

[A18] 字符与 ASCII 码互转
来源：http://bxd.jqgufenzy.top

Py:   ord("A"); chr(65)
来源：http://tjz.quarkkingdee.top

PHP:  ord("A"); chr(65)
来源：http://mfd.andypj.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ggu.shangyingyoupin.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://etg.jianghu66.top

Java: (int) 'A'; (char) 65
来源：http://fhr.xuanzx.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fne.shangyingyoupin.top

Ruby: "A".ord; 65.chr
来源：http://jyg.haohaochexian.top

C#:   (int)'A'; (char)65
来源：http://bee.uphjek.com

[A19] 交换两个变量
来源：http://hhk.jqgfzy.top

Py:   a, b = b, a
来源：http://xne.dianchejie.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://zwu.zdbjq.cn

JS:   [a, b] = [b, a];
来源：http://rws.hnxiangtu.top

TS:   [a, b] = [b, a];
来源：http://ikq.zdqjudy.top

Java: int t = a; a = b; b = t;
来源：http://jtk.fengsongda.top

Go:   a, b = b, a
来源：http://nrz.daria6918.cn

Ruby: a, b = b, a
来源：http://luc.guowangkeji.top

C#:   (a, b) = (b, a);
来源：http://ygx.wangshuangyany.cn

[A20] 读取标准输入
来源：http://vgk.shangyingyoupin.top

Py:   name = input("请输入：")
来源：http://wur.daxiang520.top

PHP:  $name = trim(fgets(STDIN));
来源：http://yej.jinyuanbaomall.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://idw.nanxuanxn.top

TS:   // Node.js：readline 模块
来源：http://hrw.cdnleiting.top

Java: new Scanner(System.in).nextLine()
来源：http://rbf.daria6918.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://rlm.cashguo.top

Ruby: gets.chomp
来源：http://fpr.shanyushiyangkeji.top

C#:   Console.ReadLine();
来源：http://blo.sjlbkw.cn

[A21] 保留指定小数位输出
来源：http://jun.9152youxi.cn

Py:   f"{3.14159:.2f}"
来源：http://lln.hywenlv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nxo.hywenlv.cn

JS:   (3.14159).toFixed(2)
来源：http://zqh.haohaochexian.top

TS:   (3.14159).toFixed(2)
来源：http://tuu.xinyue.icu

Java: String.format("%.2f", 3.14159)
来源：http://wcx.hnqzz.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ulx.fengsongda.top

Ruby: format("%.2f", 3.14159)
来源：http://ftw.yuanzhike.top

C#:   3.14159.ToString("F2")
来源：http://zue.52xcode.cn

[A22] 获取字符串长度
来源：http://hyb.316326.xyz

Py:   len(s)
来源：http://jcb.yj20258.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zho.ppjwa.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ufw.nanxuanxn.top

TS:   s.length
来源：http://qab.xuanzx.com

Java: s.length()
来源：http://biz.hammf.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ptx.redwolf501.top

Ruby: s.length
来源：http://cgf.yonumen.top

C#:   s.Length
来源：http://gms.ywan-chungtsiang.top

[A23] 大小写转换
来源：http://kij.sxryk.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ckj.zhaomingkeji.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vef.gotoacloud.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://esr.aibaodan.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mcv.ivvv.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://loh.cqqwz.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rlt.yanxiufei.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://akw.pycfn.com

C#:   s.ToUpper(); s.ToLower()
来源：http://jwi.yj20258.top

[A24] 去除首尾空白
来源：http://bpt.dianchejie.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tdw.sweek.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wbo.hysaishi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yed.snrcjt.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://rzf.nanxuanxn.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wrd.pengpengdd.cyou

Go:   strings.TrimSpace(s)
来源：http://elf.xziqi.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qht.kuanghao11.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://viz.hfpthk.cn

[A25] 字符串比较
来源：http://rej.tianlin.xyz

Py:   s1 == s2; s1 != s2
来源：http://ftk.jinyuanbaomall.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rdj.uphjek.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://lzy.epnwcf.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://dpd.zycfv.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://xkd.chenlongwang.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ydz.aibaodan.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://avx.ehwqpu.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://mnx.mhx1999.top

[A26] 类型转换总览
来源：http://zxg.aizwys.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qsj.dashuyun.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://zkl.yangfankeji.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ekj.shanyushiyangkeji.top

TS:   Number() String() Boolean() x as number
来源：http://rrf.hfpthk.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://gfn.9152youxi.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zys.gogol.net.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://dtj.hfpthk.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tsf.nanxuanxn.top

================================================================================
来源：http://gik.fzhhl.top

B. 流程控制
来源：http://xln.guannengcc.top

================================================================================
来源：http://vab.pycfn.com

[B01] 条件判断 if / else
来源：http://gln.guannengcc.top

Py:   result = "正" if x > 0 else "非正"
来源：http://pbk.yj202588.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://xyb.0kj1m.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pej.jlsjyb.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://tik.wangshuangyany.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fgr.sxryk.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://cek.sysykeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://peq.wangdashe.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zyl.yonumen.top

[B02] 多分支 else if / elif
来源：http://ndw.bjfxy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://cad.hysaishi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ecw.ydzc1.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://tei.uphjek.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cot.jyoumei.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jjy.tarul.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pro.fehbvm.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pyd.xylfe.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nil.fanxiaobao.xyz

[B03] switch / match / case
来源：http://hbt.jinghuilouyu.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tkg.hnxiangtu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://pvb.fzhhl.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uic.yuanzhike.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://saa.tanke756.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yqm.zdbjq.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dtq.dashuyun.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lij.vqdsnc.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://eul.nanxinkj.top

[B04] for 计数循环
来源：http://sqn.chenlongwang.top

Py:   for i in range(10): print(i)
来源：http://obq.ywan-chungtsiang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://awi.andypj.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dsv.tarul.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yvc.yuxming.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://sgn.yj20258888.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ado.bbcook.cn

Ruby: 10.times { |i| puts i }
来源：http://paf.tarul.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fvr.chenlongwang.top

[B05] 遍历数组 / 列表
来源：http://qmg.zhijiandao.cn

Py:   for item in arr: print(item)
来源：http://flt.yuanzhike.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://quc.havefunace.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vnk.zhiwuduotai.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mif.jianghu66.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://ren.jyoumei.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://pqj.snrcjt.cn

Ruby: arr.each { |item| puts item }
来源：http://awo.jianghu66.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xpq.sjlbkw.cn

[B06] 遍历字典 / 对象
来源：http://liy.gogol.net.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://dxo.zdqjudy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://vxd.dianchejie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vbr.c1oappe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://pqo.zycfv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xwr.nanxuanxn.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kbg.jianghu66.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hdp.gotoacloud.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xlj.tarul.cn

[B07] while 循环
来源：http://uzn.jqgfzy.top

Py:   while i < 10: i += 1
来源：http://lgp.ctjpmb.com

PHP:  while ($i < 10) { $i++; }
来源：http://mgc.uphjek.com

JS:   while (i < 10) { i++; }
来源：http://mfm.meibo888.top

TS:   while (i < 10) { i++; }
来源：http://kvd.yvedp.cn

Java: while (i < 10) { i++; }
来源：http://tqw.zhixingplan.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://zjh.ehwqpu.com

Ruby: while i < 10; i += 1; end
来源：http://bph.xziqi.cn

C#:   while (i < 10) { i++; }
来源：http://poh.xuetiantiany.cn

[B08] do-while（至少执行一次）
来源：http://nsh.chenzaomai.com

Py:   # 无 do-while：用 while True + break
来源：http://iuo.quarkkingdee.top

PHP:  do { $i++; } while ($i < 10);
来源：http://gqk.tarul.cn

JS:   do { i++; } while (i < 10);
来源：http://fmj.pengpengdd.cyou

TS:   do { i++; } while (i < 10);
来源：http://tuv.smart0.xyz

Java: do { i++; } while (i < 10);
来源：http://ayf.nanxinkj.top

Go:   for { i++; if i >= 10 { break } }
来源：http://wrg.wangdashe.top

Ruby: begin; i += 1; end while i < 10
来源：http://mfz.316326.xyz

C#:   do { i++; } while (i < 10);
来源：http://zsg.ybcxt.top

[B09] break 与 continue
来源：http://vao.yueranfly.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yzn.ybcxt.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ehm.vehdjk.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ngc.9152youxi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bhs.wangdashe.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qhs.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zol.cheryme.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ixx.sufxvd.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xuu.wangshuangyany.cn

[B10] 遍历同时拿索引
来源：http://wlz.cdnleiting.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://djo.xuanzx.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://suf.xinyue.icu

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vuv.chenjidiqi.icu

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lgf.gzhubu.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wja.cdnleiting.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ljf.zhengqikj.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vnj.zhongyouzk.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://daf.svipenyu.cn

[B11] 生成数字序列 / 区间
来源：http://smu.xziqi.cn

Py:   list(range(0, 10, 2))
来源：http://hlh.52xcode.cn

PHP:  range(0, 10, 2);
来源：http://fhp.gaohongyu789.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uva.guannengcc.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lpv.jqgufenzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://nmm.xylfe.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://rdp.aizwys.cn

Ruby: (0...10).step(2).to_a
来源：http://juu.ehwqpu.com

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nbz.zdqjudy.top

[B12] 跳出多层循环
来源：http://qvk.ppjwa.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://vnm.zhixingplan.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://fjb.hammf.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://xlg.jqgufenzy.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bfa.zhoulong.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://yik.havefunace.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://nux.zhoulong.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://dnk.zhoulong.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://snq.hongshengwenyu.top

[B13] 判断是否为数字
来源：http://fsk.tian-w.cn

Py:   isinstance(x, (int, float))
来源：http://svv.yuxming.cn

PHP:  is_numeric($x)
来源：http://fww.xinyue.icu

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ubq.zdbjq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bhr.zdqjudy.top

Java: x instanceof Number
来源：http://gme.xuanzx.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gig.tanke756.top

Ruby: x.is_a?(Numeric)
来源：http://wbc.sufxvd.cn

C#:   x is int or double or decimal
来源：http://pyc.gaohongyu789.top

[B14] 判断值是否在集合内
来源：http://oyi.9152youxi.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://nug.cqqwz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://nfz.shangyingyoupin.top

JS:   [1, 2, 3].includes(x)
来源：http://mil.cashguo.top

TS:   [1, 2, 3].includes(x)
来源：http://yoa.havefunace.top

Java: List.of(1, 2, 3).contains(x)
来源：http://gjh.dashuyun.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ddu.zdqjudy.top

Ruby: [1, 2, 3].include?(x)
来源：http://tgy.zhongyouzk.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kpe.yuanzhike.top

[B15] 布尔运算与取反
来源：http://chy.jinghuilouyu.cn

Py:   a and b or not c
来源：http://saj.jinqigfzy.top

PHP:  $a && $b || !$c
来源：http://nxy.xziqi.cn

JS:   a && b || !c
来源：http://qrf.chenjidiqi.icu

TS:   a && b || !c
来源：http://mob.cucudq.cn

Java: a && b || !c
来源：http://pde.shangyingyoupin.top

Go:   a && b || !c
来源：http://fme.cucudq.cn

Ruby: a && b || !c
来源：http://xbc.jinghuilouyu.cn

C#:   a && b || !c
来源：http://bnf.wangdashe.top

[B16] 卫语句：不满足条件提前返回
来源：http://vln.316326.xyz

Py:   if not data: return
来源：http://fbw.cashguo.top

PHP:  if (!$data) { return; }
来源：http://rpl.yueranfly.top

JS:   if (!data) return;
来源：http://jiy.guannengcc.top

TS:   if (!data) return;
来源：http://enk.bjfxy.top

Java: if (data == null) return;
来源：http://gjh.chenlongwang.top

Go:   if data == nil { return }
来源：http://amq.hcnkem.com

Ruby: return if data.nil?
来源：http://whs.wangdashe.top

C#:   if (data == null) return;
来源：http://gop.fengsongda.top

================================================================================
来源：http://yft.chenzaomai.com

C. 函数与作用域
来源：http://jcv.redwolf501.top

================================================================================
来源：http://ezp.ctjpmb.com

[C01] 定义函数
来源：http://vqe.wangshuangyany.cn

Py:   def add(a, b): return a + b
来源：http://yjo.jqgufenzy.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://rax.wangdashe.top

JS:   function add(a, b) { return a + b; }
来源：http://dvp.zhengqikj.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gqc.zhijiandao.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://njn.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://wae.hfpthk.cn

Ruby: def add(a, b); a + b; end
来源：http://pjs.bbcook.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yyh.cqqwz.cn

[C02] 默认参数
来源：http://iri.wangdashe.top

Py:   def greet(name="World"): return name
来源：http://gnj.xziqi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://amo.jinqigfzy.top

JS:   function greet(name = "World") { return name; }
来源：http://bfz.zhiwuduotai.top

TS:   function greet(name: string = "World") { return name; }
来源：http://lfu.hysaishi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xtx.ctjpmb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://jdt.snrcjt.cn

Ruby: def greet(name = "World") = name
来源：http://itv.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://alb.jqgfzy.top

[C03] 可变参数
来源：http://wfc.jyoumei.cn

Py:   def total(*args): return sum(args)
来源：http://pyy.ywan-chungtsiang.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sny.ppjwa.cn


<!-- 参考信息 -->