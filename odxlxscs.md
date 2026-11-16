代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gln.cheryme.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://uyf.havefunace.top

TS:   if (!x) {}
来源：http://hmt.hfpthk.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://egt.andypj.xyz

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://axo.nanxuanxn.top

Ruby: unless x            # nil 与 false 为假
来源：http://wrj.zhijiandao.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://lor.nanxinkj.top

[A17] 位运算
来源：http://wsy.fengsongda.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://thq.nanxinkj.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://csx.xylfe.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pux.xuanzx.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cpr.hnxiangtu.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ans.sufxvd.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fxb.xinyue.icu

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://awd.xingfuxueyuan.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://pkr.xylfe.cn

[A18] 字符与 ASCII 码互转
来源：http://iqo.52xcode.cn

Py:   ord("A"); chr(65)
来源：http://fva.shanyushiyangkeji.top

PHP:  ord("A"); chr(65)
来源：http://ywi.havefunace.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fxy.dianchejie.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hza.sjlbkw.cn

Java: (int) 'A'; (char) 65
来源：http://fpi.tarul.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fos.hesvh.cn

Ruby: "A".ord; 65.chr
来源：http://blx.nanxinkj.top

C#:   (int)'A'; (char)65
来源：http://yxi.bbcook.cn

[A19] 交换两个变量
来源：http://zaa.svipenyu.cn

Py:   a, b = b, a
来源：http://ybt.xinyue.icu

PHP:  [$a, $b] = [$b, $a];
来源：http://sgv.xziqi.cn

JS:   [a, b] = [b, a];
来源：http://zaq.quarkkingdee.top

TS:   [a, b] = [b, a];
来源：http://xfk.tanke756.top

Java: int t = a; a = b; b = t;
来源：http://oms.cashguo.top

Go:   a, b = b, a
来源：http://kjd.gzhubu.top

Ruby: a, b = b, a
来源：http://goh.yuanzhike.top

C#:   (a, b) = (b, a);
来源：http://ohy.hammf.cn

[A20] 读取标准输入
来源：http://pio.zdbjq.cn

Py:   name = input("请输入：")
来源：http://sij.shzxlz.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://hqi.nanxinkj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yyf.fanxiaobao.xyz

TS:   // Node.js：readline 模块
来源：http://ltr.daxiang520.top

Java: new Scanner(System.in).nextLine()
来源：http://kic.fehbvm.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xjw.sufxvd.cn

Ruby: gets.chomp
来源：http://opd.wangshuangyany.cn

C#:   Console.ReadLine();
来源：http://tpf.jinqigufen.top

[A21] 保留指定小数位输出
来源：http://jcu.jiagoushi.top

Py:   f"{3.14159:.2f}"
来源：http://piq.redwolf501.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://jpn.sjlbkw.cn

JS:   (3.14159).toFixed(2)
来源：http://dyk.fzhhl.top

TS:   (3.14159).toFixed(2)
来源：http://phd.redwolf501.top

Java: String.format("%.2f", 3.14159)
来源：http://vdf.cheryme.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nnp.iojbl.cn

Ruby: format("%.2f", 3.14159)
来源：http://nyj.cdnleiting.top

C#:   3.14159.ToString("F2")
来源：http://xwv.ivvv.top

[A22] 获取字符串长度
来源：http://kfw.jinqigufen.top

Py:   len(s)
来源：http://jcn.andypj.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vsm.sweek.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ghh.yongpay.top

TS:   s.length
来源：http://lbo.quarkkingdee.top

Java: s.length()
来源：http://pqs.yongpay.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zts.sysykeji.top

Ruby: s.length
来源：http://usx.sxryk.cn

C#:   s.Length
来源：http://syz.316326.xyz

[A23] 大小写转换
来源：http://eyg.ydjk.org.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://kcx.sxryk.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ggi.fehbvm.com

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://peq.c1oappe.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://jum.yfazqb.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://eni.pengpengdd.cyou

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wah.ehwqpu.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://fjo.yuxming.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://vdv.dashuyun.cn

[A24] 去除首尾空白
来源：http://stz.jinghuilouyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ttp.shuidangran.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mtg.hesvh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://fwr.tanke756.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ncj.nwbrower.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://tsr.52xcode.cn

Go:   strings.TrimSpace(s)
来源：http://xcs.sjlbkw.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rmj.jinqigfzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yxv.uphjek.com

[A25] 字符串比较
来源：http://tfu.tian-w.cn

Py:   s1 == s2; s1 != s2
来源：http://xuk.zhongyouzk.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rri.ybcxt.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wgu.chenzaomai.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xcd.sweek.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://mxx.ivvv.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tzj.0kj1m.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://cvd.andypj.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://yhm.tianlin.xyz

[A26] 类型转换总览
来源：http://cjs.zhaomingkeji.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://adt.hysaishi.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rmh.tianlin.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ynw.xziqi.cn

TS:   Number() String() Boolean() x as number
来源：http://krz.jinyuanbaomall.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://uzw.zhoulong.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://caf.xylfe.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://nzi.zhijiandao.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://qia.xuetiantiany.cn

================================================================================
来源：http://lii.zhiwuduotai.top

B. 流程控制
来源：http://gvs.smart0.xyz

================================================================================
来源：http://tdt.iojbl.cn

[B01] 条件判断 if / else
来源：http://ued.hnxiangtu.top

Py:   result = "正" if x > 0 else "非正"
来源：http://yjm.hongshengwenyu.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://sdc.uphjek.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qtv.aibaodan.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://bjq.ivvv.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ixg.birdmap.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://yjb.chenlongwang.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xgc.gaohongyu789.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sdf.fktsv.cn

[B02] 多分支 else if / elif
来源：http://vij.cheryme.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://btf.jlsjyb.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fag.fehbvm.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mqk.yuxming.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://yon.jiagoushi.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cbh.zhongyouzk.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iit.yvedp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ysw.wangshuangyany.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://icc.shuidangran.top

[B03] switch / match / case
来源：http://ofr.zhixingplan.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dgz.hnxiangtu.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ind.zhiwuduotai.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wyr.jqgfzy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eay.jinqigufen.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lhg.zhoulong.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jfz.hnxiangtu.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jkd.nwbrower.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://qtg.yj20258888.top

[B04] for 计数循环
来源：http://khl.daxiang520.top

Py:   for i in range(10): print(i)
来源：http://uoq.xingfuxueyuan.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ifk.ywan-chungtsiang.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qqb.xuetiantiany.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tap.iojbl.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://lbh.316326.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vvj.cdnleiting.top

Ruby: 10.times { |i| puts i }
来源：http://sjt.vqdsnc.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ygp.havefunace.top

[B05] 遍历数组 / 列表
来源：http://xyy.hnxiangtu.top

Py:   for item in arr: print(item)
来源：http://qxp.andypj.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bbo.jqgfzy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gvh.sjlbkw.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://wqb.birdmap.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://dgv.wangdashe.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zkl.ydjk.org.cn

Ruby: arr.each { |item| puts item }
来源：http://ubu.yanxiufei.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mkt.zhijiandao.cn

[B06] 遍历字典 / 对象
来源：http://nms.chenjidiqi.icu

Py:   for k, v in d.items(): print(k, v)
来源：http://vzw.tanke756.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://lcy.birdmap.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hxv.sweek.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wcq.sufxvd.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qxp.yj202588.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ync.sjlbkw.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ihz.yangfankeji.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://qyh.vqdsnc.cn

[B07] while 循环
来源：http://rzw.jqgfzy.top

Py:   while i < 10: i += 1
来源：http://vtk.cheryme.top

PHP:  while ($i < 10) { $i++; }
来源：http://pxm.fanxiaobao.xyz

JS:   while (i < 10) { i++; }
来源：http://oen.ppjwa.cn

TS:   while (i < 10) { i++; }
来源：http://dep.hesvh.cn

Java: while (i < 10) { i++; }
来源：http://wav.hnxiangtu.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://dke.vehdjk.com

Ruby: while i < 10; i += 1; end
来源：http://hbv.hywenlv.cn

C#:   while (i < 10) { i++; }
来源：http://odw.yvedp.cn

[B08] do-while（至少执行一次）
来源：http://xhk.fengsongda.top

Py:   # 无 do-while：用 while True + break
来源：http://cap.cheryme.top

PHP:  do { $i++; } while ($i < 10);
来源：http://kjs.daxiang520.top

JS:   do { i++; } while (i < 10);
来源：http://kax.nanxinkj.top

TS:   do { i++; } while (i < 10);
来源：http://irz.shanyushiyangtech.top

Java: do { i++; } while (i < 10);
来源：http://xpa.daria6918.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://fqr.yongpay.top

Ruby: begin; i += 1; end while i < 10
来源：http://kbk.jyoumei.cn

C#:   do { i++; } while (i < 10);
来源：http://ngl.sxryk.cn

[B09] break 与 continue
来源：http://ydp.sjlbkw.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://fxf.xingfuxueyuan.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nof.vqdsnc.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://whj.yj20258888.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://xny.chenjidiqi.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dwu.hcnkem.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kpt.daxiang520.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gbb.jiagoushi.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zzu.sysykeji.top

[B10] 遍历同时拿索引
来源：http://mnn.gaohongyu789.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://olr.tanke756.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xsg.316326.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://vgo.sjlbkw.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fen.zdqjudy.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ksq.shanyushiyangtech.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gzm.fanxiaobao.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://dpe.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://xjj.haohaochexian.top

[B11] 生成数字序列 / 区间
来源：http://bbo.jiagoushi.top

Py:   list(range(0, 10, 2))
来源：http://jtz.gaohongyu789.top

PHP:  range(0, 10, 2);
来源：http://nzh.daxiang520.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xgr.jinghuilouyu.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://duu.uphjek.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://uzn.shangyingyoupin.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qqo.jiagoushi.top

Ruby: (0...10).step(2).to_a
来源：http://dxz.cqqwz.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://eli.jinyuanbaomall.cn

[B12] 跳出多层循环
来源：http://gyb.hcnkem.com

Py:   # 无标签跳转：抽成函数用 return
来源：http://gcp.sxryk.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://obo.ydjk.org.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://pab.ydjk.org.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://eso.jinghuilouyu.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://efk.yonumen.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://syo.uphjek.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zes.yongpay.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://iya.52xcode.cn

[B13] 判断是否为数字
来源：http://gyn.tarul.cn

Py:   isinstance(x, (int, float))
来源：http://pzy.yuxming.cn

PHP:  is_numeric($x)
来源：http://ihi.c1oappe.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://djb.zhixingplan.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://qsu.ybcxt.top

Java: x instanceof Number
来源：http://twj.svipenyu.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oxy.zycfv.cn

Ruby: x.is_a?(Numeric)
来源：http://krg.jyoumei.cn

C#:   x is int or double or decimal
来源：http://pgv.daria6918.cn

[B14] 判断值是否在集合内
来源：http://oca.hywenlv.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://trb.xylfe.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://rzi.kuanghao11.cn

JS:   [1, 2, 3].includes(x)
来源：http://bjl.gotoacloud.top

TS:   [1, 2, 3].includes(x)
来源：http://dly.chenlongwang.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zyp.nwbrower.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://fwp.jinyuanbaomall.cn

Ruby: [1, 2, 3].include?(x)
来源：http://pxe.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://llu.aizwys.cn

[B15] 布尔运算与取反
来源：http://mxz.nanxuanxn.top

Py:   a and b or not c
来源：http://jcv.zhixingplan.top

PHP:  $a && $b || !$c
来源：http://qsm.hfpthk.cn

JS:   a && b || !c
来源：http://szz.redwolf501.top

TS:   a && b || !c
来源：http://xyt.tanke756.top

Java: a && b || !c
来源：http://qou.vehdjk.com

Go:   a && b || !c
来源：http://lld.mhx1999.top

Ruby: a && b || !c
来源：http://drp.smart0.xyz

C#:   a && b || !c
来源：http://orx.dianchejie.cn

[B16] 卫语句：不满足条件提前返回
来源：http://eeu.yueranfly.top

Py:   if not data: return
来源：http://koz.wangdashe.top

PHP:  if (!$data) { return; }
来源：http://whi.hongshengwenyu.top

JS:   if (!data) return;
来源：http://xzx.tanke756.top

TS:   if (!data) return;
来源：http://jkq.zhiwuduotai.top

Java: if (data == null) return;
来源：http://cbv.epnwcf.com

Go:   if data == nil { return }
来源：http://tww.hywenlv.cn

Ruby: return if data.nil?
来源：http://ctp.mhx1999.top

C#:   if (data == null) return;
来源：http://pwj.yvedp.cn

================================================================================
来源：http://cpx.chenlongwang.top

C. 函数与作用域
来源：http://vvs.yfazqb.com

================================================================================
来源：http://mye.sxryk.cn

[C01] 定义函数
来源：http://fik.zdbjq.cn

Py:   def add(a, b): return a + b
来源：http://leg.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ust.zhaomingkeji.xyz

JS:   function add(a, b) { return a + b; }
来源：http://uar.yonumen.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://qvu.wangshuangyany.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://roy.jyoumei.cn

Go:   func add(a, b int) int { return a + b }
来源：http://eul.0kj1m.cn

Ruby: def add(a, b); a + b; end
来源：http://hfb.nwbrower.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://aid.vqdsnc.cn

[C02] 默认参数
来源：http://zto.hesvh.cn

Py:   def greet(name="World"): return name
来源：http://hsu.yonumen.top

PHP:  function greet($name = "World") { return $name; }
来源：http://vop.hfpthk.cn

JS:   function greet(name = "World") { return name; }
来源：http://lze.ctjpmb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://bou.nwbrower.top

Java: // 无默认参数：方法重载或 Optional
来源：http://dfs.yongpay.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://vat.yonumen.top

Ruby: def greet(name = "World") = name
来源：http://ray.jqgufenzy.top

C#:   string Greet(string name = "World") => name;
来源：http://dog.chenzaomai.com

[C03] 可变参数
来源：http://kvr.tian-w.cn

Py:   def total(*args): return sum(args)
来源：http://moy.xingfuxueyuan.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://aii.guannengcc.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://nis.feifeiyinyue.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://vwa.c1oappe.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://bpn.xuanzx.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ebc.redwolf501.top

Ruby: def total(*nums); nums.sum; end
来源：http://ztv.ehwqpu.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gbs.snrcjt.cn

[C04] 命名参数 / 关键字参数
来源：http://enh.gogol.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zuo.bbcook.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://eua.jlsjyb.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wdh.shanyushiyangkeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://apz.vqdsnc.cn

Java: // 无：用 Builder 模式或 record
来源：http://mub.hnqzz.top

Go:   // 无：用配置结构体参数
来源：http://qfn.dianchejie.cn

Ruby: f(a: 1, b: 2)
来源：http://idf.zhaomingkeji.xyz

C#:   f(a: 1, b: 2)
来源：http://fvp.dianchejie.cn

[C05] 返回多个值
来源：http://ayl.gogol.net.cn

Py:   return a, b
来源：http://fmx.cashguo.top

PHP:  return [$a, $b];
来源：http://qit.guannengcc.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://kot.cheryme.top

TS:   return { a, b };
来源：http://rxm.chenzaomai.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://vsv.dianchejie.cn

Go:   return a, b
来源：http://udf.yj20258888.top

Ruby: return a, b
来源：http://ubh.redwolf501.top

C#:   return (a, b);              // ValueTuple
来源：http://aox.daria6918.cn

[C06] 匿名函数 / lambda
来源：http://slx.jlsjyb.cn

Py:   square = lambda x: x * x
来源：http://dkd.vqdsnc.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://vrd.zhongyouzk.top

JS:   const square = x => x * x;
来源：http://opb.yj20258.top

TS:   const square = (x: number): number => x * x;
来源：http://mwn.guannengcc.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://via.daria6918.cn

Go:   sq := func(x int) int { return x * x }
来源：http://gqo.quarkkingdee.top

Ruby: square = ->(x) { x * x }
来源：http://roa.meibo888.top


<!-- 参考信息 -->