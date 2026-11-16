代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sbo.yanxiufei.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://pzx.kuanghao11.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tan.tanke756.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://liw.hongshengwenyu.top

[A18] 字符与 ASCII 码互转
来源：http://jwx.aibaodan.cn

Py:   ord("A"); chr(65)
来源：http://ddn.vehdjk.com

PHP:  ord("A"); chr(65)
来源：http://cyu.zdbjq.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://kdh.hnqzz.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dzj.xingfuxueyuan.xyz

Java: (int) 'A'; (char) 65
来源：http://ocu.wangshuangyany.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bgh.yueranfly.top

Ruby: "A".ord; 65.chr
来源：http://bwz.fzhhl.top

C#:   (int)'A'; (char)65
来源：http://zzs.dashuyun.cn

[A19] 交换两个变量
来源：http://lnn.havefunace.top

Py:   a, b = b, a
来源：http://bgi.zhengqikj.top

PHP:  [$a, $b] = [$b, $a];
来源：http://nfi.zhixingplan.top

JS:   [a, b] = [b, a];
来源：http://tcn.ivvv.top

TS:   [a, b] = [b, a];
来源：http://wlh.ybcxt.top

Java: int t = a; a = b; b = t;
来源：http://fdm.sufxvd.cn

Go:   a, b = b, a
来源：http://pys.sufxvd.cn

Ruby: a, b = b, a
来源：http://iya.tian-w.cn

C#:   (a, b) = (b, a);
来源：http://odf.vqdsnc.cn

[A20] 读取标准输入
来源：http://wod.0kj1m.cn

Py:   name = input("请输入：")
来源：http://lqv.yanxiufei.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://skn.tian-w.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://bie.xuetiantiany.cn

TS:   // Node.js：readline 模块
来源：http://hgu.jqgufenzy.top

Java: new Scanner(System.in).nextLine()
来源：http://gzj.yuanzhike.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ead.chenzaomai.com

Ruby: gets.chomp
来源：http://jaw.vehdjk.com

C#:   Console.ReadLine();
来源：http://qsi.tian-w.cn

[A21] 保留指定小数位输出
来源：http://xqk.sufxvd.cn

Py:   f"{3.14159:.2f}"
来源：http://qci.jinqigfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://duy.daxiang520.top

JS:   (3.14159).toFixed(2)
来源：http://ypk.sweek.top

TS:   (3.14159).toFixed(2)
来源：http://acr.0kj1m.cn

Java: String.format("%.2f", 3.14159)
来源：http://bkp.cqqwz.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mdb.sxryk.cn

Ruby: format("%.2f", 3.14159)
来源：http://dpu.sweek.top

C#:   3.14159.ToString("F2")
来源：http://phw.kuanghao11.cn

[A22] 获取字符串长度
来源：http://zmq.vqdsnc.cn

Py:   len(s)
来源：http://juc.gzhubu.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://asi.jyoumei.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uxy.fzhhl.top

TS:   s.length
来源：http://pkm.zhengqikj.top

Java: s.length()
来源：http://ewb.nwbrower.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ezv.zdbjq.cn

Ruby: s.length
来源：http://fxu.316326.xyz

C#:   s.Length
来源：http://mfh.dianchejie.cn

[A23] 大小写转换
来源：http://tnu.andypj.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://xmy.jqgfzy.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dia.ywan-chungtsiang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kaj.jyoumei.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://szb.yvedp.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sla.epnwcf.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://xbk.cqqwz.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://wrq.daxiang520.top

C#:   s.ToUpper(); s.ToLower()
来源：http://lsn.chenjidiqi.icu

[A24] 去除首尾空白
来源：http://dao.hnxiangtu.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fku.wangshuangyany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://did.wangshuangyany.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gdg.yanxiufei.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ogu.fanxiaobao.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wqq.feifeiyinyue.top

Go:   strings.TrimSpace(s)
来源：http://tww.hfpthk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://imo.zhixingplan.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://yav.ctjpmb.com

[A25] 字符串比较
来源：http://ehm.cheryme.top

Py:   s1 == s2; s1 != s2
来源：http://mvx.yvedp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ccu.0kj1m.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://cib.xuetiantiany.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gma.xinyue.icu

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://jqv.yfazqb.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://bck.hnxiangtu.top

Ruby: s1 == s2; s1 <=> s2
来源：http://osi.jqgfzy.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://xrb.hcnkem.com

[A26] 类型转换总览
来源：http://lrr.quarkkingdee.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://eyj.gogol.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://fkq.ydzc1.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hmk.yj20258888.top

TS:   Number() String() Boolean() x as number
来源：http://kuz.dashuyun.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://vew.dianchejie.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zfk.c1oappe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://jzz.shanyushiyangtech.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xko.yj20258888.top

================================================================================
来源：http://iiz.jyoumei.cn

B. 流程控制
来源：http://xtd.mhx1999.top

================================================================================
来源：http://yxg.jinghuilouyu.cn

[B01] 条件判断 if / else
来源：http://joj.ctjpmb.com

Py:   result = "正" if x > 0 else "非正"
来源：http://hiz.andypj.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://feg.tian-w.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://cbl.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://thp.havefunace.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ocm.zhengqikj.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://gzf.jlsjyb.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bzo.smart0.xyz

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hzi.jqgufenzy.top

[B02] 多分支 else if / elif
来源：http://yce.chenjidiqi.icu

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://swp.yuanzhike.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oqk.yongpay.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dfw.pengpengdd.cyou

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pde.fanxiaobao.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qmh.daxiang520.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://vhe.c1oappe.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://prt.cashguo.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://owr.chenlongwang.top

[B03] switch / match / case
来源：http://gbt.ppjwa.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ncn.fehbvm.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lll.shanyushiyangtech.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zzr.xinyue.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://otb.wangshuangyany.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://kyo.hongshengwenyu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ujt.dashuyun.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nsa.andypj.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jxy.yueranfly.top

[B04] for 计数循环
来源：http://amz.shzxlz.cn

Py:   for i in range(10): print(i)
来源：http://xkt.quarkkingdee.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://eim.hfpthk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wox.meibo888.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ula.gotoacloud.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://thr.jqgfzy.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://qzf.zhixingplan.top

Ruby: 10.times { |i| puts i }
来源：http://mzo.tanke756.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://kwr.fzhhl.top

[B05] 遍历数组 / 列表
来源：http://xei.cdnleiting.top

Py:   for item in arr: print(item)
来源：http://uqf.chenlongwang.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://lhs.zhixingplan.top

JS:   for (const item of arr) { console.log(item); }
来源：http://bjs.xinyue.icu

TS:   for (const item of arr) { console.log(item); }
来源：http://wvw.chenjidiqi.icu

Java: for (var item : arr) { System.out.println(item); }
来源：http://jmg.cucudq.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://kaz.jqgfzy.top

Ruby: arr.each { |item| puts item }
来源：http://ofj.dashuyun.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gnk.aizwys.cn

[B06] 遍历字典 / 对象
来源：http://zgs.sxryk.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://gjz.xuanzx.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ldp.daria6918.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bpd.jinghuilouyu.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ifp.yfazqb.com

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hex.gotoacloud.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ihf.ydzc1.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eur.yuxming.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hzz.wangdashe.top

[B07] while 循环
来源：http://lci.wangdashe.top

Py:   while i < 10: i += 1
来源：http://rkl.jiagoushi.top

PHP:  while ($i < 10) { $i++; }
来源：http://ukp.nanxinkj.top

JS:   while (i < 10) { i++; }
来源：http://sct.hammf.cn

TS:   while (i < 10) { i++; }
来源：http://xsm.zhongyouzk.top

Java: while (i < 10) { i++; }
来源：http://kmx.haohaochexian.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yob.yj20258888.top

Ruby: while i < 10; i += 1; end
来源：http://hul.gogol.net.cn

C#:   while (i < 10) { i++; }
来源：http://lnh.yueranfly.top

[B08] do-while（至少执行一次）
来源：http://yop.guowangkeji.top

Py:   # 无 do-while：用 while True + break
来源：http://zzo.zhoulong.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://gnk.nanxinkj.top

JS:   do { i++; } while (i < 10);
来源：http://cpw.yj20258888.top

TS:   do { i++; } while (i < 10);
来源：http://otj.jiagoushi.top

Java: do { i++; } while (i < 10);
来源：http://skq.ydzc1.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cxd.sufxvd.cn

Ruby: begin; i += 1; end while i < 10
来源：http://dfu.havefunace.top

C#:   do { i++; } while (i < 10);
来源：http://gyj.316326.xyz

[B09] break 与 continue
来源：http://lci.fzhhl.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://rbx.guannengcc.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://dlj.fktsv.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hjw.tanke756.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dtj.zdbjq.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ffj.zhongyouzk.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://zud.yonumen.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dbo.yj20258888.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://plp.nanxinkj.top

[B10] 遍历同时拿索引
来源：http://gxm.zhixingplan.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tqi.cqqwz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ovl.zhaomingkeji.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qdd.ydjk.org.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lsx.haohaochexian.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://yas.bjfxy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://pzo.jianghu66.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://uiy.birdmap.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://swx.shangyingyoupin.top

[B11] 生成数字序列 / 区间
来源：http://zbe.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://qqv.chenzaomai.com

PHP:  range(0, 10, 2);
来源：http://oum.yueranfly.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://epk.dashuyun.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://vlg.chenlongwang.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rmw.tanke756.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://qda.tarul.cn

Ruby: (0...10).step(2).to_a
来源：http://hay.fktsv.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://cac.vehdjk.com

[B12] 跳出多层循环
来源：http://qga.jinghuilouyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://xcq.cashguo.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://mru.wangshuangyany.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://kil.smart0.xyz

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://smb.fanxiaobao.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://efp.quarkkingdee.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://esq.haohaochexian.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tbb.hywenlv.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://vou.iojbl.cn

[B13] 判断是否为数字
来源：http://rsc.tarul.cn

Py:   isinstance(x, (int, float))
来源：http://zjd.nanxuanxn.top

PHP:  is_numeric($x)
来源：http://box.tianlin.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nqw.yj202588.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gdd.tarul.cn

Java: x instanceof Number
来源：http://gwy.fzhhl.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://acq.zycfv.cn

Ruby: x.is_a?(Numeric)
来源：http://uqc.birdmap.top

C#:   x is int or double or decimal
来源：http://uzd.jlsjyb.cn

[B14] 判断值是否在集合内
来源：http://lch.nanxuanxn.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jzd.hysaishi.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yzc.cdnleiting.top

JS:   [1, 2, 3].includes(x)
来源：http://auq.uphjek.com

TS:   [1, 2, 3].includes(x)
来源：http://jpp.daria6918.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://niv.cashguo.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://bry.nwbrower.top

Ruby: [1, 2, 3].include?(x)
来源：http://jqk.mhx1999.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://tjm.hnxiangtu.top

[B15] 布尔运算与取反
来源：http://tmd.havefunace.top

Py:   a and b or not c
来源：http://bsz.guowangkeji.top

PHP:  $a && $b || !$c
来源：http://ght.daxiang520.top

JS:   a && b || !c
来源：http://anb.jinqigfzy.top

TS:   a && b || !c
来源：http://vsm.yangfankeji.com

Java: a && b || !c
来源：http://vxx.tanke756.top

Go:   a && b || !c
来源：http://tuy.shanyushiyangtech.top

Ruby: a && b || !c
来源：http://onu.gogol.net.cn

C#:   a && b || !c
来源：http://dxu.hcnkem.com

[B16] 卫语句：不满足条件提前返回
来源：http://bzy.jqgfzy.top

Py:   if not data: return
来源：http://skx.fanxiaobao.xyz

PHP:  if (!$data) { return; }
来源：http://xuf.jinghuilouyu.cn

JS:   if (!data) return;
来源：http://trd.zhiwuduotai.top

TS:   if (!data) return;
来源：http://bxj.sweek.top

Java: if (data == null) return;
来源：http://ziy.uphjek.com

Go:   if data == nil { return }
来源：http://jcg.cheryme.top

Ruby: return if data.nil?
来源：http://fjf.jianghu66.top

C#:   if (data == null) return;
来源：http://zxj.ppjwa.cn

================================================================================
来源：http://hmq.dashuyun.cn

C. 函数与作用域
来源：http://tea.nanxinkj.top

================================================================================
来源：http://zgt.yueranfly.top

[C01] 定义函数
来源：http://doh.shanyushiyangkeji.top

Py:   def add(a, b): return a + b
来源：http://nui.zdbjq.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wps.ydjk.org.cn

JS:   function add(a, b) { return a + b; }
来源：http://exe.xuetiantiany.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ebi.hammf.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://ifx.dashuyun.cn

Go:   func add(a, b int) int { return a + b }
来源：http://rsp.birdmap.top

Ruby: def add(a, b); a + b; end
来源：http://fjt.yuxming.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mzx.zhiwuduotai.top

[C02] 默认参数
来源：http://caf.zhiwuduotai.top

Py:   def greet(name="World"): return name
来源：http://cdt.meibo888.top

PHP:  function greet($name = "World") { return $name; }
来源：http://uij.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://sqp.yvedp.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://obv.iojbl.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://rgl.yfazqb.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kva.pengpengdd.cyou

Ruby: def greet(name = "World") = name
来源：http://ymh.yonumen.top

C#:   string Greet(string name = "World") => name;
来源：http://asy.hnqzz.top

[C03] 可变参数
来源：http://edw.hesvh.cn

Py:   def total(*args): return sum(args)
来源：http://hqa.zhoulong.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wjd.hesvh.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wdt.cucudq.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wmf.tanke756.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://fnt.dianchejie.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tqn.cucudq.cn

Ruby: def total(*nums); nums.sum; end
来源：http://lsf.ybcxt.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://tut.cashguo.top

[C04] 命名参数 / 关键字参数
来源：http://bey.yj20258888.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lqd.aibaodan.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kpj.cashguo.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://zvb.ydzc1.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://xsk.sxryk.cn

Java: // 无：用 Builder 模式或 record
来源：http://nem.chenzaomai.com

Go:   // 无：用配置结构体参数
来源：http://axa.jqgufenzy.top

Ruby: f(a: 1, b: 2)
来源：http://uar.zdqjudy.top

C#:   f(a: 1, b: 2)
来源：http://sak.feifeiyinyue.top

[C05] 返回多个值
来源：http://hjg.wangshuangyany.cn

Py:   return a, b
来源：http://nsk.shuidangran.top

PHP:  return [$a, $b];
来源：http://lif.52xcode.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://oqi.daxiang520.top

TS:   return { a, b };
来源：http://uly.shanyushiyangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://tks.dashuyun.cn

Go:   return a, b
来源：http://prf.iojbl.cn

Ruby: return a, b
来源：http://kbz.gaohongyu789.top

C#:   return (a, b);              // ValueTuple
来源：http://ybj.jinghuilouyu.cn

[C06] 匿名函数 / lambda
来源：http://dji.sufxvd.cn

Py:   square = lambda x: x * x
来源：http://zva.dashuyun.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://eut.jinyuanbaomall.cn

JS:   const square = x => x * x;
来源：http://tny.hywenlv.cn

TS:   const square = (x: number): number => x * x;
来源：http://fso.cdnleiting.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://yrj.cucudq.cn

Go:   sq := func(x int) int { return x * x }
来源：http://dbt.hysaishi.cn

Ruby: square = ->(x) { x * x }
来源：http://zbb.xylfe.cn

C#:   Func<int, int> square = x => x * x;
来源：http://xbz.wangdashe.top

[C07] 把函数作为参数传入
来源：http://ilb.sysykeji.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gtw.jlsjyb.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dxk.hcnkem.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tzt.nwbrower.top

TS:   arr.map(String)
来源：http://adk.shangyingyoupin.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mni.ehwqpu.com

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://shi.yonumen.top

Ruby: arr.map(&:upcase)
来源：http://bqj.ehwqpu.com

C#:   arr.Select(s => s.ToUpper())
来源：http://bxd.iojbl.cn

[C08] 闭包
来源：http://nga.zhiwuduotai.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://poq.pengpengdd.cyou


<!-- 参考信息 -->