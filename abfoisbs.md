代发 wailian999

Ruby: value = data || "默认值"
来源：http://psv.yj20258.top

C#:   var value = data ?? "默认值";
来源：http://yku.jqgufenzy.top

[A16] 真假值判断规则
来源：http://ypt.xylfe.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cyp.hongshengwenyu.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mux.vqdsnc.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://cts.guowangkeji.top

TS:   if (!x) {}
来源：http://fnm.jyoumei.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vnv.quarkkingdee.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://trc.pengpengdd.cyou

Ruby: unless x            # nil 与 false 为假
来源：http://xpa.tarul.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bjq.shuidangran.top

[A17] 位运算
来源：http://xfx.sxryk.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://seg.hfpthk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hpe.tianlin.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://anq.wangdashe.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fwq.zhixingplan.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://adg.yonumen.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://tqx.ivvv.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://thz.tanke756.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qms.dashuyun.cn

[A18] 字符与 ASCII 码互转
来源：http://qxg.yj20258.top

Py:   ord("A"); chr(65)
来源：http://muw.shangyingyoupin.top

PHP:  ord("A"); chr(65)
来源：http://kyt.yongpay.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://drs.feifeiyinyue.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ohc.zhaomingkeji.xyz

Java: (int) 'A'; (char) 65
来源：http://gqp.jinghuilouyu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ajg.chenjidiqi.icu

Ruby: "A".ord; 65.chr
来源：http://fwi.xinyue.icu

C#:   (int)'A'; (char)65
来源：http://ofw.xinyue.icu

[A19] 交换两个变量
来源：http://lon.gzhubu.top

Py:   a, b = b, a
来源：http://cmk.epnwcf.com

PHP:  [$a, $b] = [$b, $a];
来源：http://wft.hongshengwenyu.top

JS:   [a, b] = [b, a];
来源：http://mdq.sjlbkw.cn

TS:   [a, b] = [b, a];
来源：http://kfn.hnqzz.top

Java: int t = a; a = b; b = t;
来源：http://svd.gaohongyu789.top

Go:   a, b = b, a
来源：http://urq.zhoulong.xyz

Ruby: a, b = b, a
来源：http://ogq.redwolf501.top

C#:   (a, b) = (b, a);
来源：http://dmv.zdqjudy.top

[A20] 读取标准输入
来源：http://bcn.fehbvm.com

Py:   name = input("请输入：")
来源：http://dzj.cqqwz.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://wow.sjlbkw.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://oom.52xcode.cn

TS:   // Node.js：readline 模块
来源：http://qym.cdnleiting.top

Java: new Scanner(System.in).nextLine()
来源：http://feh.shzxlz.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hqo.yuxming.cn

Ruby: gets.chomp
来源：http://rxs.yj20258.top

C#:   Console.ReadLine();
来源：http://zmi.zdqjudy.top

[A21] 保留指定小数位输出
来源：http://imc.zhijiandao.cn

Py:   f"{3.14159:.2f}"
来源：http://bfb.bbcook.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://kwg.jyoumei.cn

JS:   (3.14159).toFixed(2)
来源：http://zgp.hfpthk.cn

TS:   (3.14159).toFixed(2)
来源：http://ppx.shzxlz.cn

Java: String.format("%.2f", 3.14159)
来源：http://vbv.jianghu66.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yri.uphjek.com

Ruby: format("%.2f", 3.14159)
来源：http://lux.ywan-chungtsiang.top

C#:   3.14159.ToString("F2")
来源：http://vhh.fehbvm.com

[A22] 获取字符串长度
来源：http://pis.daria6918.cn

Py:   len(s)
来源：http://ilx.bjfxy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hig.zhiwuduotai.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://msa.sufxvd.cn

TS:   s.length
来源：http://xwc.epnwcf.com

Java: s.length()
来源：http://cjh.cheryme.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ejm.tarul.cn

Ruby: s.length
来源：http://mji.zhijiandao.cn

C#:   s.Length
来源：http://hyl.sweek.top

[A23] 大小写转换
来源：http://tdd.fanxiaobao.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://mrt.kuanghao11.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ucs.gaohongyu789.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sqh.nanxuanxn.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wiz.yangfankeji.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tzy.guannengcc.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://kwr.yongpay.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wmi.c1oappe.top

C#:   s.ToUpper(); s.ToLower()
来源：http://deh.yongpay.top

[A24] 去除首尾空白
来源：http://oss.tanke756.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hfm.chenzaomai.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://inv.jiagoushi.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dpx.yuxming.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nqz.sufxvd.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xlm.yuanzhike.top

Go:   strings.TrimSpace(s)
来源：http://mkc.guowangkeji.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rkr.hnxiangtu.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://swp.nwbrower.top

[A25] 字符串比较
来源：http://cfs.jiagoushi.top

Py:   s1 == s2; s1 != s2
来源：http://rrp.jinghuilouyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://zeo.hnxiangtu.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://xik.sxryk.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://yvj.yonumen.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ocx.yj20258.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://qyo.ivvv.top

Ruby: s1 == s2; s1 <=> s2
来源：http://yss.fzhhl.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jbd.sjlbkw.cn

[A26] 类型转换总览
来源：http://ywu.yueranfly.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://npr.yonumen.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://evf.ivvv.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://axs.sysykeji.top

TS:   Number() String() Boolean() x as number
来源：http://pec.gogol.net.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://boc.jqgfzy.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://noc.birdmap.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://wcb.gzhubu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://avi.wangshuangyany.cn

================================================================================
来源：http://zoi.yueranfly.top

B. 流程控制
来源：http://lhu.ivvv.top

================================================================================
来源：http://ech.hcnkem.com

[B01] 条件判断 if / else
来源：http://kfl.andypj.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://skk.yuxming.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://shb.nwbrower.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wxw.svipenyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://flc.jqgufenzy.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hqq.dianchejie.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xgn.gogol.net.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hqe.wangdashe.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://nwz.zhijiandao.cn

[B02] 多分支 else if / elif
来源：http://oeh.sweek.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://azv.epnwcf.com

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://gps.chenzaomai.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xgc.aizwys.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dea.shuidangran.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://swv.zhixingplan.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zxl.yuxming.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://pwx.tarul.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xlu.hywenlv.cn

[B03] switch / match / case
来源：http://ifp.jyoumei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://tgx.cashguo.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://iam.gaohongyu789.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yja.yanxiufei.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://soy.jiagoushi.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://obk.smart0.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://kke.quarkkingdee.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://ozx.jiagoushi.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kyb.hysaishi.cn

[B04] for 计数循环
来源：http://adx.jinqigufen.top

Py:   for i in range(10): print(i)
来源：http://nla.meibo888.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hvm.hysaishi.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bjp.jinyuanbaomall.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tgu.yangfankeji.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xzo.hysaishi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://vnn.hnqzz.top

Ruby: 10.times { |i| puts i }
来源：http://gto.daxiang520.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nlz.vehdjk.com

[B05] 遍历数组 / 列表
来源：http://vpi.tarul.cn

Py:   for item in arr: print(item)
来源：http://uaf.zhixingplan.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lku.nwbrower.top

JS:   for (const item of arr) { console.log(item); }
来源：http://hwd.nwbrower.top

TS:   for (const item of arr) { console.log(item); }
来源：http://zah.xziqi.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ovn.chenzaomai.com

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://vdg.0kj1m.cn

Ruby: arr.each { |item| puts item }
来源：http://sdy.ppjwa.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ibx.xinyue.icu

[B06] 遍历字典 / 对象
来源：http://vck.52xcode.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://vvn.epnwcf.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://rqn.hnxiangtu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ldy.c1oappe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://auq.aibaodan.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qzz.andypj.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rfh.smart0.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://xhw.yanxiufei.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mht.jianghu66.top

[B07] while 循环
来源：http://gey.jinyuanbaomall.cn

Py:   while i < 10: i += 1
来源：http://mbq.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://wdz.jinyuanbaomall.cn

JS:   while (i < 10) { i++; }
来源：http://lxk.tianlin.xyz

TS:   while (i < 10) { i++; }
来源：http://wzc.feifeiyinyue.top

Java: while (i < 10) { i++; }
来源：http://xlt.jiagoushi.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qcf.yanxiufei.cn

Ruby: while i < 10; i += 1; end
来源：http://nob.shuidangran.top

C#:   while (i < 10) { i++; }
来源：http://etd.hesvh.cn

[B08] do-while（至少执行一次）
来源：http://lom.haohaochexian.top

Py:   # 无 do-while：用 while True + break
来源：http://prb.bbcook.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ogu.zhiwuduotai.top

JS:   do { i++; } while (i < 10);
来源：http://dne.gzhubu.top

TS:   do { i++; } while (i < 10);
来源：http://xry.havefunace.top

Java: do { i++; } while (i < 10);
来源：http://gin.cqqwz.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://ceo.jinyuanbaomall.cn

Ruby: begin; i += 1; end while i < 10
来源：http://nwi.cashguo.top

C#:   do { i++; } while (i < 10);
来源：http://qqb.9152youxi.cn

[B09] break 与 continue
来源：http://uzb.sweek.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nrz.dianchejie.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hdx.sysykeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://twi.gaohongyu789.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cxz.yj202588.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nuk.ydzc1.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kmn.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rvj.ehwqpu.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vff.jianghu66.top

[B10] 遍历同时拿索引
来源：http://piu.yueranfly.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://qvf.gaohongyu789.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rar.zhaomingkeji.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://zhx.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pki.yanxiufei.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://qnp.jianghu66.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://rgf.hcnkem.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tsm.chenzaomai.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://trl.jianghu66.top

[B11] 生成数字序列 / 区间
来源：http://gva.cdnleiting.top

Py:   list(range(0, 10, 2))
来源：http://ofh.redwolf501.top

PHP:  range(0, 10, 2);
来源：http://sxl.yangfankeji.com

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yrs.jinqigfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eai.yj20258.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fgx.birdmap.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cqk.yueranfly.top

Ruby: (0...10).step(2).to_a
来源：http://lft.fanxiaobao.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nsz.vehdjk.com

[B12] 跳出多层循环
来源：http://bwu.cheryme.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://icb.xuetiantiany.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://asf.hongshengwenyu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://bje.9152youxi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qem.jianghu66.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zie.xinyue.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mqa.yuxming.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uri.daria6918.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://gxl.epnwcf.com

[B13] 判断是否为数字
来源：http://stm.jyoumei.cn

Py:   isinstance(x, (int, float))
来源：http://ovf.jlsjyb.cn

PHP:  is_numeric($x)
来源：http://tce.pycfn.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nle.epnwcf.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://fil.zhoulong.xyz

Java: x instanceof Number
来源：http://iqs.dianchejie.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://znl.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://ssh.yj202588.top

C#:   x is int or double or decimal
来源：http://ppa.fktsv.cn

[B14] 判断值是否在集合内
来源：http://pzw.kuanghao11.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yzt.bjfxy.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ozk.ydzc1.top

JS:   [1, 2, 3].includes(x)
来源：http://cwk.pengpengdd.cyou

TS:   [1, 2, 3].includes(x)
来源：http://mzh.zdbjq.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://fzt.fanxiaobao.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wmu.shangyingyoupin.top

Ruby: [1, 2, 3].include?(x)
来源：http://yft.ydjk.org.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://qcr.fengsongda.top

[B15] 布尔运算与取反
来源：http://pbi.sysykeji.top

Py:   a and b or not c
来源：http://rsk.shzxlz.cn

PHP:  $a && $b || !$c
来源：http://mbf.fengsongda.top

JS:   a && b || !c
来源：http://pxc.ydzc1.top

TS:   a && b || !c
来源：http://vnr.daxiang520.top

Java: a && b || !c
来源：http://xku.gogol.net.cn

Go:   a && b || !c
来源：http://ngh.kuanghao11.cn

Ruby: a && b || !c
来源：http://nal.yj20258.top

C#:   a && b || !c
来源：http://nwy.xuetiantiany.cn

[B16] 卫语句：不满足条件提前返回
来源：http://cwr.nanxuanxn.top

Py:   if not data: return
来源：http://cut.yuxming.cn

PHP:  if (!$data) { return; }
来源：http://kct.ydzc1.top

JS:   if (!data) return;
来源：http://uix.wangshuangyany.cn

TS:   if (!data) return;
来源：http://mjz.chenlongwang.top

Java: if (data == null) return;
来源：http://erm.zhixingplan.top

Go:   if data == nil { return }
来源：http://uwz.wangdashe.top

Ruby: return if data.nil?
来源：http://mcm.shzxlz.cn

C#:   if (data == null) return;
来源：http://skk.meibo888.top

================================================================================
来源：http://uyr.hcnkem.com

C. 函数与作用域
来源：http://abi.guowangkeji.top

================================================================================
来源：http://ary.zhixingplan.top

[C01] 定义函数
来源：http://mvk.c1oappe.top

Py:   def add(a, b): return a + b
来源：http://cel.sjlbkw.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://glr.zhaomingkeji.xyz

JS:   function add(a, b) { return a + b; }
来源：http://mcb.zhijiandao.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wbg.hesvh.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ofe.pengpengdd.cyou

Go:   func add(a, b int) int { return a + b }
来源：http://mud.chenlongwang.top

Ruby: def add(a, b); a + b; end
来源：http://wgx.andypj.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://obl.kuanghao11.cn

[C02] 默认参数
来源：http://mcz.redwolf501.top

Py:   def greet(name="World"): return name
来源：http://lgb.dashuyun.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://ryy.c1oappe.top

JS:   function greet(name = "World") { return name; }
来源：http://aca.quarkkingdee.top

TS:   function greet(name: string = "World") { return name; }
来源：http://wmv.yongpay.top

Java: // 无默认参数：方法重载或 Optional
来源：http://xrb.hfpthk.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cql.mhx1999.top

Ruby: def greet(name = "World") = name
来源：http://kqx.sjlbkw.cn

C#:   string Greet(string name = "World") => name;
来源：http://dfz.sysykeji.top

[C03] 可变参数
来源：http://byv.kuanghao11.cn

Py:   def total(*args): return sum(args)
来源：http://knm.shanyushiyangtech.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://exe.yonumen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://amx.feifeiyinyue.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://cag.xuetiantiany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wxz.hongshengwenyu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://abt.andypj.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://oum.gotoacloud.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mwo.chenlongwang.top

[C04] 命名参数 / 关键字参数
来源：http://xvr.cqqwz.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://jti.xingfuxueyuan.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://nxj.zdqjudy.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hwm.nanxinkj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://dlp.hfpthk.cn

Java: // 无：用 Builder 模式或 record
来源：http://llc.yonumen.top

Go:   // 无：用配置结构体参数
来源：http://iop.ywan-chungtsiang.top

Ruby: f(a: 1, b: 2)
来源：http://wfe.yongpay.top

C#:   f(a: 1, b: 2)
来源：http://kmw.yfazqb.com

[C05] 返回多个值
来源：http://wiw.jyoumei.cn

Py:   return a, b
来源：http://dyl.haohaochexian.top

PHP:  return [$a, $b];
来源：http://jnw.birdmap.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://hmf.hesvh.cn

TS:   return { a, b };
来源：http://pdx.sysykeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://zjj.tianlin.xyz

Go:   return a, b
来源：http://pro.zhoulong.xyz

Ruby: return a, b
来源：http://zom.havefunace.top

C#:   return (a, b);              // ValueTuple
来源：http://oaw.sxryk.cn

[C06] 匿名函数 / lambda
来源：http://eti.cucudq.cn

Py:   square = lambda x: x * x
来源：http://nif.mhx1999.top

PHP:  $square = fn($x) => $x * $x;
来源：http://lwz.wangshuangyany.cn

JS:   const square = x => x * x;
来源：http://rod.jqgufenzy.top


<!-- 参考信息 -->