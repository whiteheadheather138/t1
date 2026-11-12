代发 wailian999

Ruby: value = data || "默认值"
来源：http://jww.wangshuangyany.cn

C#:   var value = data ?? "默认值";
来源：http://qss.ybcxt.top

[A16] 真假值判断规则
来源：http://qfc.redwolf501.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://uso.fehbvm.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://owe.xylfe.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://waq.ywan-chungtsiang.top

TS:   if (!x) {}
来源：http://nba.zhengqikj.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vee.jinqigufen.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ypj.shzxlz.cn

Ruby: unless x            # nil 与 false 为假
来源：http://gjk.shuidangran.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://dkd.cdnleiting.top

[A17] 位运算
来源：http://shj.daria6918.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ujh.tianlin.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://rke.9152youxi.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kmt.iojbl.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://ihm.tanke756.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qtk.tarul.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ktz.bbcook.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://guf.xylfe.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cbd.hysaishi.cn

[A18] 字符与 ASCII 码互转
来源：http://hxi.hesvh.cn

Py:   ord("A"); chr(65)
来源：http://vbn.chenzaomai.com

PHP:  ord("A"); chr(65)
来源：http://mpg.cucudq.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pth.mhx1999.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qra.chenjidiqi.icu

Java: (int) 'A'; (char) 65
来源：http://wqb.yonumen.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dct.daxiang520.top

Ruby: "A".ord; 65.chr
来源：http://qob.yfazqb.com

C#:   (int)'A'; (char)65
来源：http://esu.xinyue.icu

[A19] 交换两个变量
来源：http://amb.hysaishi.cn

Py:   a, b = b, a
来源：http://dfb.zhengqikj.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hos.guannengcc.top

JS:   [a, b] = [b, a];
来源：http://qhs.mhx1999.top

TS:   [a, b] = [b, a];
来源：http://ava.nwbrower.top

Java: int t = a; a = b; b = t;
来源：http://hpz.nanxuanxn.top

Go:   a, b = b, a
来源：http://ozt.daria6918.cn

Ruby: a, b = b, a
来源：http://ghd.cdnleiting.top

C#:   (a, b) = (b, a);
来源：http://jgy.jianghu66.top

[A20] 读取标准输入
来源：http://jbz.shuidangran.top

Py:   name = input("请输入：")
来源：http://ttz.hfpthk.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://rgw.fengsongda.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://rtb.fanxiaobao.xyz

TS:   // Node.js：readline 模块
来源：http://trs.yj20258888.top

Java: new Scanner(System.in).nextLine()
来源：http://con.yangfankeji.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://kwr.shuidangran.top

Ruby: gets.chomp
来源：http://orh.tianlin.xyz

C#:   Console.ReadLine();
来源：http://kws.shzxlz.cn

[A21] 保留指定小数位输出
来源：http://wce.aibaodan.cn

Py:   f"{3.14159:.2f}"
来源：http://lwf.gotoacloud.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://war.ydzc1.top

JS:   (3.14159).toFixed(2)
来源：http://bpy.shangyingyoupin.top

TS:   (3.14159).toFixed(2)
来源：http://ywm.mhx1999.top

Java: String.format("%.2f", 3.14159)
来源：http://riq.yj202588.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xtk.ydjk.org.cn

Ruby: format("%.2f", 3.14159)
来源：http://ccm.sysykeji.top

C#:   3.14159.ToString("F2")
来源：http://ure.ctjpmb.com

[A22] 获取字符串长度
来源：http://qsh.wangshuangyany.cn

Py:   len(s)
来源：http://qlw.bbcook.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bjr.xingfuxueyuan.xyz

JS:   s.length                          # 按 UTF-16 单元计
来源：http://kwy.hcnkem.com

TS:   s.length
来源：http://ywf.bjfxy.top

Java: s.length()
来源：http://tnq.yangfankeji.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://swt.guowangkeji.top

Ruby: s.length
来源：http://cwr.haohaochexian.top

C#:   s.Length
来源：http://uqr.yangfankeji.com

[A23] 大小写转换
来源：http://qcl.jinghuilouyu.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://aez.fktsv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://phz.zycfv.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://box.fzhhl.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://lkb.fanxiaobao.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ixx.bjfxy.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xxv.hnqzz.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://zdp.gotoacloud.top

C#:   s.ToUpper(); s.ToLower()
来源：http://tdz.hongshengwenyu.top

[A24] 去除首尾空白
来源：http://lqz.hongshengwenyu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://xjy.nanxinkj.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://dri.zdbjq.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kle.ivvv.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bno.ydzc1.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jxh.yonumen.top

Go:   strings.TrimSpace(s)
来源：http://wtu.pengpengdd.cyou

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://sch.chenzaomai.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://agc.ppjwa.cn

[A25] 字符串比较
来源：http://ncb.kuanghao11.cn

Py:   s1 == s2; s1 != s2
来源：http://ovl.tanke756.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://gqm.ivvv.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mbi.svipenyu.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fhd.jinyuanbaomall.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://osq.52xcode.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mru.zhijiandao.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ass.snrcjt.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bqg.sysykeji.top

[A26] 类型转换总览
来源：http://jfs.yvedp.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://sgl.zhaomingkeji.xyz

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jwt.zycfv.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cio.quarkkingdee.top

TS:   Number() String() Boolean() x as number
来源：http://sjo.jinyuanbaomall.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://xqi.hnxiangtu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yiw.zdbjq.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://smu.shanyushiyangkeji.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://yhn.52xcode.cn

================================================================================
来源：http://lko.jianghu66.top

B. 流程控制
来源：http://qwz.fanxiaobao.xyz

================================================================================
来源：http://ozu.yj202588.top

[B01] 条件判断 if / else
来源：http://dah.jqgfzy.top

Py:   result = "正" if x > 0 else "非正"
来源：http://crx.gotoacloud.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://fzn.xingfuxueyuan.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://gng.xuetiantiany.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hek.kuanghao11.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://rmi.havefunace.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gsy.cdnleiting.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://koq.hesvh.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ltq.hywenlv.cn

[B02] 多分支 else if / elif
来源：http://ppy.9152youxi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qty.sweek.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ggg.tianlin.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ypm.zdqjudy.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aqb.chenzaomai.com

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bbl.jinghuilouyu.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eob.shanyushiyangtech.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pto.ybcxt.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mnt.jinghuilouyu.cn

[B03] switch / match / case
来源：http://ada.sufxvd.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ucb.feifeiyinyue.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ojl.meibo888.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zoq.quarkkingdee.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cza.yonumen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://qsg.shangyingyoupin.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://npy.epnwcf.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lmk.yonumen.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zjw.vehdjk.com

[B04] for 计数循环
来源：http://sux.dashuyun.cn

Py:   for i in range(10): print(i)
来源：http://nav.hammf.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://crn.yuxming.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://rvt.c1oappe.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tou.quarkkingdee.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://yja.tianlin.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hlb.sjlbkw.cn

Ruby: 10.times { |i| puts i }
来源：http://xan.ctjpmb.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pfv.xinyue.icu

[B05] 遍历数组 / 列表
来源：http://haq.bbcook.cn

Py:   for item in arr: print(item)
来源：http://rrq.hysaishi.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://plq.zhaomingkeji.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://uoi.redwolf501.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mol.yvedp.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://aef.tianlin.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ocw.vehdjk.com

Ruby: arr.each { |item| puts item }
来源：http://ezx.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://buh.xingfuxueyuan.xyz

[B06] 遍历字典 / 对象
来源：http://czz.cqqwz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://fcc.sufxvd.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zaa.dianchejie.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ade.xinyue.icu

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://cdc.xylfe.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://acj.jqgfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gpd.sysykeji.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xjn.redwolf501.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dds.yfazqb.com

[B07] while 循环
来源：http://xst.epnwcf.com

Py:   while i < 10: i += 1
来源：http://bld.wangshuangyany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://jmu.dianchejie.cn

JS:   while (i < 10) { i++; }
来源：http://hkg.aibaodan.cn

TS:   while (i < 10) { i++; }
来源：http://lua.shuidangran.top

Java: while (i < 10) { i++; }
来源：http://ziu.yvedp.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://svy.nwbrower.top

Ruby: while i < 10; i += 1; end
来源：http://uuw.daria6918.cn

C#:   while (i < 10) { i++; }
来源：http://waf.sweek.top

[B08] do-while（至少执行一次）
来源：http://ibq.gogol.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://xwq.yj202588.top

PHP:  do { $i++; } while ($i < 10);
来源：http://bhb.yj202588.top

JS:   do { i++; } while (i < 10);
来源：http://cfa.nanxinkj.top

TS:   do { i++; } while (i < 10);
来源：http://bnr.shanyushiyangkeji.top

Java: do { i++; } while (i < 10);
来源：http://rno.zdbjq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://bne.vehdjk.com

Ruby: begin; i += 1; end while i < 10
来源：http://kto.daria6918.cn

C#:   do { i++; } while (i < 10);
来源：http://wso.yonumen.top

[B09] break 与 continue
来源：http://cnf.aibaodan.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://jdn.birdmap.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://wph.hfpthk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tla.smart0.xyz

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://awm.yangfankeji.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tbb.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://wuu.meibo888.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://jel.zycfv.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pqv.tanke756.top

[B10] 遍历同时拿索引
来源：http://glr.xingfuxueyuan.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qkx.fzhhl.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tdd.fanxiaobao.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://jfq.yonumen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://qzz.chenjidiqi.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://zfz.feifeiyinyue.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://smc.smart0.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fus.ivvv.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vek.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://yab.yuanzhike.top

Py:   list(range(0, 10, 2))
来源：http://jaj.fanxiaobao.xyz

PHP:  range(0, 10, 2);
来源：http://wkh.52xcode.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tmq.nanxinkj.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wep.0kj1m.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fye.ybcxt.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://bng.ehwqpu.com

Ruby: (0...10).step(2).to_a
来源：http://jla.tian-w.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://iyv.zhongyouzk.top

[B12] 跳出多层循环
来源：http://ofs.birdmap.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://pxp.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://sol.chenjidiqi.icu

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bny.chenjidiqi.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://cmj.hcnkem.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://omk.yanxiufei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://lmb.xuetiantiany.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yds.yangfankeji.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hqr.daxiang520.top

[B13] 判断是否为数字
来源：http://xfk.meibo888.top

Py:   isinstance(x, (int, float))
来源：http://hvm.cucudq.cn

PHP:  is_numeric($x)
来源：http://ikx.tian-w.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gsl.zdbjq.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jnx.bbcook.cn

Java: x instanceof Number
来源：http://oud.zhixingplan.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ybh.smart0.xyz

Ruby: x.is_a?(Numeric)
来源：http://xhx.bjfxy.top

C#:   x is int or double or decimal
来源：http://xzb.gaohongyu789.top

[B14] 判断值是否在集合内
来源：http://fxv.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tmb.shuidangran.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lxc.haohaochexian.top

JS:   [1, 2, 3].includes(x)
来源：http://jap.52xcode.cn

TS:   [1, 2, 3].includes(x)
来源：http://lkc.shuidangran.top

Java: List.of(1, 2, 3).contains(x)
来源：http://uua.gogol.net.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hgg.jinqigfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://ddo.ydzc1.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ydo.gogol.net.cn

[B15] 布尔运算与取反
来源：http://doe.daxiang520.top

Py:   a and b or not c
来源：http://upk.yj20258888.top

PHP:  $a && $b || !$c
来源：http://tuu.epnwcf.com

JS:   a && b || !c
来源：http://igf.quarkkingdee.top

TS:   a && b || !c
来源：http://grs.havefunace.top

Java: a && b || !c
来源：http://mha.hfpthk.cn

Go:   a && b || !c
来源：http://vbp.jinqigufen.top

Ruby: a && b || !c
来源：http://wgx.yuxming.cn

C#:   a && b || !c
来源：http://mlf.yangfankeji.com

[B16] 卫语句：不满足条件提前返回
来源：http://jlt.hnqzz.top

Py:   if not data: return
来源：http://jct.9152youxi.cn

PHP:  if (!$data) { return; }
来源：http://hgy.vqdsnc.cn

JS:   if (!data) return;
来源：http://fkc.jinqigfzy.top

TS:   if (!data) return;
来源：http://ksu.yj20258888.top

Java: if (data == null) return;
来源：http://mrz.wangdashe.top

Go:   if data == nil { return }
来源：http://ind.jlsjyb.cn

Ruby: return if data.nil?
来源：http://lww.jqgufenzy.top

C#:   if (data == null) return;
来源：http://ico.iojbl.cn

================================================================================
来源：http://zzf.hnxiangtu.top

C. 函数与作用域
来源：http://qwa.cqqwz.cn

================================================================================
来源：http://qex.andypj.xyz

[C01] 定义函数
来源：http://cxn.fehbvm.com

Py:   def add(a, b): return a + b
来源：http://oeg.gaohongyu789.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xyj.yonumen.top

JS:   function add(a, b) { return a + b; }
来源：http://qus.yj20258888.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wzi.hnqzz.top

Java: static int add(int a, int b) { return a + b; }
来源：http://gte.fengsongda.top

Go:   func add(a, b int) int { return a + b }
来源：http://ghu.zhijiandao.cn

Ruby: def add(a, b); a + b; end
来源：http://jku.andypj.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://eye.hnxiangtu.top

[C02] 默认参数
来源：http://oiy.quarkkingdee.top

Py:   def greet(name="World"): return name
来源：http://qna.9152youxi.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hzg.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://aop.snrcjt.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://sqx.yj20258.top

Java: // 无默认参数：方法重载或 Optional
来源：http://fam.vehdjk.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://zen.jiagoushi.top

Ruby: def greet(name = "World") = name
来源：http://jtv.xuetiantiany.cn

C#:   string Greet(string name = "World") => name;
来源：http://npz.gzhubu.top

[C03] 可变参数
来源：http://den.shuidangran.top

Py:   def total(*args): return sum(args)
来源：http://bxr.yonumen.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://unc.vehdjk.com

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mly.yj202588.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://kyl.zhoulong.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://iit.sweek.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jcu.chenzaomai.com

Ruby: def total(*nums); nums.sum; end
来源：http://dqd.zdqjudy.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hyu.c1oappe.top

[C04] 命名参数 / 关键字参数
来源：http://ezr.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://fqo.shangyingyoupin.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://iit.tianlin.xyz

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sjj.ywan-chungtsiang.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jdv.aizwys.cn

Java: // 无：用 Builder 模式或 record
来源：http://tpo.kuanghao11.cn

Go:   // 无：用配置结构体参数
来源：http://ick.zhongyouzk.top

Ruby: f(a: 1, b: 2)
来源：http://pow.shangyingyoupin.top

C#:   f(a: 1, b: 2)
来源：http://twf.cashguo.top

[C05] 返回多个值
来源：http://vrq.nwbrower.top

Py:   return a, b
来源：http://rrq.fehbvm.com

PHP:  return [$a, $b];
来源：http://smc.nanxinkj.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://nwa.zhengqikj.top

TS:   return { a, b };
来源：http://ees.jyoumei.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aik.guannengcc.top

Go:   return a, b
来源：http://yfo.xingfuxueyuan.xyz

Ruby: return a, b
来源：http://yrp.yonumen.top

C#:   return (a, b);              // ValueTuple
来源：http://syu.xuanzx.com

[C06] 匿名函数 / lambda
来源：http://bgu.zdqjudy.top

Py:   square = lambda x: x * x
来源：http://dsi.hammf.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://xab.hongshengwenyu.top

JS:   const square = x => x * x;
来源：http://jab.andypj.xyz


<!-- 参考信息 -->