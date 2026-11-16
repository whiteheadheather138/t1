代发 wailian999

JS:   [a, b] = [b, a];
来源：http://gys.cdnleiting.top

TS:   [a, b] = [b, a];
来源：http://ojy.zhengqikj.top

Java: int t = a; a = b; b = t;
来源：http://itz.vehdjk.com

Go:   a, b = b, a
来源：http://isv.jqgfzy.top

Ruby: a, b = b, a
来源：http://kum.vqdsnc.cn

C#:   (a, b) = (b, a);
来源：http://bhb.xziqi.cn

[A20] 读取标准输入
来源：http://ncc.zhongyouzk.top

Py:   name = input("请输入：")
来源：http://eex.gaohongyu789.top

PHP:  $name = trim(fgets(STDIN));
来源：http://gco.pycfn.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gqq.aizwys.cn

TS:   // Node.js：readline 模块
来源：http://rza.birdmap.top

Java: new Scanner(System.in).nextLine()
来源：http://cgf.daxiang520.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ppo.ydjk.org.cn

Ruby: gets.chomp
来源：http://gqk.yvedp.cn

C#:   Console.ReadLine();
来源：http://egu.yvedp.cn

[A21] 保留指定小数位输出
来源：http://lsu.yfazqb.com

Py:   f"{3.14159:.2f}"
来源：http://rez.jqgfzy.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://xgu.ydjk.org.cn

JS:   (3.14159).toFixed(2)
来源：http://sif.zhoulong.xyz

TS:   (3.14159).toFixed(2)
来源：http://wmu.feifeiyinyue.top

Java: String.format("%.2f", 3.14159)
来源：http://mup.meibo888.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mye.sysykeji.top

Ruby: format("%.2f", 3.14159)
来源：http://lan.hnxiangtu.top

C#:   3.14159.ToString("F2")
来源：http://biw.xinyue.icu

[A22] 获取字符串长度
来源：http://brr.bjfxy.top

Py:   len(s)
来源：http://caz.gogol.net.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jpf.jiagoushi.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://nov.bjfxy.top

TS:   s.length
来源：http://yir.cdnleiting.top

Java: s.length()
来源：http://qfk.jqgfzy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://cfa.zdbjq.cn

Ruby: s.length
来源：http://dxg.tianlin.xyz

C#:   s.Length
来源：http://akw.ctjpmb.com

[A23] 大小写转换
来源：http://nqu.sxryk.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://ehj.shuidangran.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dqm.zhengqikj.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://bdv.zhaomingkeji.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fff.yuanzhike.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ouj.shuidangran.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://zlz.tanke756.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ghm.haohaochexian.top

C#:   s.ToUpper(); s.ToLower()
来源：http://eiu.ydzc1.top

[A24] 去除首尾空白
来源：http://bas.havefunace.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ebi.yvedp.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ujv.yj202588.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qvv.fktsv.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vuq.cqqwz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://krm.gotoacloud.top

Go:   strings.TrimSpace(s)
来源：http://bdj.xingfuxueyuan.xyz

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://ldu.pycfn.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://iax.xinyue.icu

[A25] 字符串比较
来源：http://uwz.sysykeji.top

Py:   s1 == s2; s1 != s2
来源：http://yds.hcnkem.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fft.ctjpmb.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rop.yuxming.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://xyz.jinqigfzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://efp.nanxuanxn.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wuo.shangyingyoupin.top

Ruby: s1 == s2; s1 <=> s2
来源：http://mng.cucudq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zwk.sjlbkw.cn

[A26] 类型转换总览
来源：http://ypr.yuanzhike.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://snw.jlsjyb.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hxl.iojbl.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qmz.zhiwuduotai.top

TS:   Number() String() Boolean() x as number
来源：http://yjl.yanxiufei.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zjh.bbcook.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mjz.jinghuilouyu.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://ahj.shanyushiyangtech.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://gdq.havefunace.top

================================================================================
来源：http://ihi.iojbl.cn

B. 流程控制
来源：http://bku.shanyushiyangkeji.top

================================================================================
来源：http://miu.wangdashe.top

[B01] 条件判断 if / else
来源：http://mwc.hfpthk.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gdi.zdqjudy.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bng.guowangkeji.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://toh.sweek.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wha.vehdjk.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://eas.daria6918.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://aii.ivvv.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://oxp.birdmap.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ksw.aizwys.cn

[B02] 多分支 else if / elif
来源：http://izj.316326.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://gba.ybcxt.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ykc.yonumen.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iry.wangshuangyany.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nxu.cashguo.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://iju.zdbjq.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://zim.cheryme.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://vrn.zhaomingkeji.xyz

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zct.xuetiantiany.cn

[B03] switch / match / case
来源：http://dbp.dashuyun.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://qpc.chenlongwang.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zci.guowangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rwn.ctjpmb.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yoo.yongpay.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://xyd.gzhubu.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://upx.daxiang520.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://nul.xziqi.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://xuz.hesvh.cn

[B04] for 计数循环
来源：http://oyl.hammf.cn

Py:   for i in range(10): print(i)
来源：http://dgy.zdqjudy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://sff.pycfn.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ghz.chenjidiqi.icu

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vlc.zhaomingkeji.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pjb.xingfuxueyuan.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://zci.pycfn.com

Ruby: 10.times { |i| puts i }
来源：http://kqa.hysaishi.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://vae.nanxinkj.top

[B05] 遍历数组 / 列表
来源：http://xbr.jinqigufen.top

Py:   for item in arr: print(item)
来源：http://dhn.iojbl.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://bsa.cheryme.top

JS:   for (const item of arr) { console.log(item); }
来源：http://wgj.fehbvm.com

TS:   for (const item of arr) { console.log(item); }
来源：http://eqk.sysykeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://var.dashuyun.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://rxp.hnqzz.top

Ruby: arr.each { |item| puts item }
来源：http://nlf.vehdjk.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://yxy.jinqigfzy.top

[B06] 遍历字典 / 对象
来源：http://qol.yj20258.top

Py:   for k, v in d.items(): print(k, v)
来源：http://uyu.yueranfly.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://azk.ydzc1.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bde.ppjwa.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ayc.kuanghao11.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://flm.yj20258.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wzm.xuanzx.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qok.fanxiaobao.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pjy.meibo888.top

[B07] while 循环
来源：http://dnz.redwolf501.top

Py:   while i < 10: i += 1
来源：http://nbp.xuanzx.com

PHP:  while ($i < 10) { $i++; }
来源：http://inf.jqgfzy.top

JS:   while (i < 10) { i++; }
来源：http://pgf.hfpthk.cn

TS:   while (i < 10) { i++; }
来源：http://yyr.wangdashe.top

Java: while (i < 10) { i++; }
来源：http://ttq.jqgfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nvn.vehdjk.com

Ruby: while i < 10; i += 1; end
来源：http://sqh.daria6918.cn

C#:   while (i < 10) { i++; }
来源：http://yma.ivvv.top

[B08] do-while（至少执行一次）
来源：http://kfk.ctjpmb.com

Py:   # 无 do-while：用 while True + break
来源：http://rvw.shanyushiyangkeji.top

PHP:  do { $i++; } while ($i < 10);
来源：http://ijk.cucudq.cn

JS:   do { i++; } while (i < 10);
来源：http://cqx.havefunace.top

TS:   do { i++; } while (i < 10);
来源：http://xqe.zhaomingkeji.xyz

Java: do { i++; } while (i < 10);
来源：http://ome.pycfn.com

Go:   for { i++; if i >= 10 { break } }
来源：http://wvn.yanxiufei.cn

Ruby: begin; i += 1; end while i < 10
来源：http://awa.jqgfzy.top

C#:   do { i++; } while (i < 10);
来源：http://jin.zhongyouzk.top

[B09] break 与 continue
来源：http://vjs.shuidangran.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://loe.ydjk.org.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tfd.daria6918.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mgs.yonumen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tzp.yongpay.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://inp.hfpthk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ocy.zhaomingkeji.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://tyf.fengsongda.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://kfu.jinqigfzy.top

[B10] 遍历同时拿索引
来源：http://knm.yj20258.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://tgq.shangyingyoupin.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ict.jqgfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://eno.daria6918.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://lbd.shzxlz.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://oeq.cashguo.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://nxr.xingfuxueyuan.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ngl.yj202588.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://zsi.sweek.top

[B11] 生成数字序列 / 区间
来源：http://kfy.pengpengdd.cyou

Py:   list(range(0, 10, 2))
来源：http://tvp.aizwys.cn

PHP:  range(0, 10, 2);
来源：http://saj.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://euv.tarul.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tgo.hywenlv.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ebe.haohaochexian.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://inx.shuidangran.top

Ruby: (0...10).step(2).to_a
来源：http://aqi.zhoulong.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://lnx.tian-w.cn

[B12] 跳出多层循环
来源：http://ygn.fktsv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nzt.ctjpmb.com

PHP:  # 无标签：用 goto 或函数返回
来源：http://uqe.zhixingplan.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://gtp.gzhubu.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://zha.yueranfly.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kcf.hfpthk.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://omk.ybcxt.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://aqw.zhiwuduotai.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jsi.fanxiaobao.xyz

[B13] 判断是否为数字
来源：http://qed.shanyushiyangkeji.top

Py:   isinstance(x, (int, float))
来源：http://vec.guannengcc.top

PHP:  is_numeric($x)
来源：http://uib.gogol.net.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pqy.hysaishi.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://bjt.tianlin.xyz

Java: x instanceof Number
来源：http://hxh.iojbl.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://dsy.chenzaomai.com

Ruby: x.is_a?(Numeric)
来源：http://jyq.jqgfzy.top

C#:   x is int or double or decimal
来源：http://fld.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://bdm.havefunace.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lwo.sxryk.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://pul.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://hhk.cqqwz.cn

TS:   [1, 2, 3].includes(x)
来源：http://rmh.sufxvd.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vgd.tanke756.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zxd.yj20258.top

Ruby: [1, 2, 3].include?(x)
来源：http://hfo.jqgfzy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://kys.quarkkingdee.top

[B15] 布尔运算与取反
来源：http://mlq.birdmap.top

Py:   a and b or not c
来源：http://wdx.hesvh.cn

PHP:  $a && $b || !$c
来源：http://ltw.ppjwa.cn

JS:   a && b || !c
来源：http://zac.wangshuangyany.cn

TS:   a && b || !c
来源：http://gzd.cashguo.top

Java: a && b || !c
来源：http://oep.mhx1999.top

Go:   a && b || !c
来源：http://gvh.yfazqb.com

Ruby: a && b || !c
来源：http://zna.zhongyouzk.top

C#:   a && b || !c
来源：http://flr.feifeiyinyue.top

[B16] 卫语句：不满足条件提前返回
来源：http://pse.wangshuangyany.cn

Py:   if not data: return
来源：http://yzb.zycfv.cn

PHP:  if (!$data) { return; }
来源：http://kud.chenjidiqi.icu

JS:   if (!data) return;
来源：http://sgm.havefunace.top

TS:   if (!data) return;
来源：http://wmr.fengsongda.top

Java: if (data == null) return;
来源：http://qpa.nanxuanxn.top

Go:   if data == nil { return }
来源：http://syd.aizwys.cn

Ruby: return if data.nil?
来源：http://szu.cqqwz.cn

C#:   if (data == null) return;
来源：http://cvs.daria6918.cn

================================================================================
来源：http://zke.fanxiaobao.xyz

C. 函数与作用域
来源：http://osq.zhongyouzk.top

================================================================================
来源：http://eks.316326.xyz

[C01] 定义函数
来源：http://ilt.xuanzx.com

Py:   def add(a, b): return a + b
来源：http://hzb.iojbl.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://msm.ybcxt.top

JS:   function add(a, b) { return a + b; }
来源：http://mwf.cdnleiting.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ium.xuanzx.com

Java: static int add(int a, int b) { return a + b; }
来源：http://yxr.zhijiandao.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tkf.shzxlz.cn

Ruby: def add(a, b); a + b; end
来源：http://gwo.fengsongda.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://pyb.zhijiandao.cn

[C02] 默认参数
来源：http://rmi.jiagoushi.top

Py:   def greet(name="World"): return name
来源：http://txg.zhijiandao.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://hkx.yj20258888.top

JS:   function greet(name = "World") { return name; }
来源：http://ion.dashuyun.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://psd.jlsjyb.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://fio.hammf.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://dbp.chenlongwang.top

Ruby: def greet(name = "World") = name
来源：http://vnk.yanxiufei.cn

C#:   string Greet(string name = "World") => name;
来源：http://kyx.pengpengdd.cyou

[C03] 可变参数
来源：http://ijx.zhongyouzk.top

Py:   def total(*args): return sum(args)
来源：http://pyb.zdbjq.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gad.gaohongyu789.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hfj.xuanzx.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://aqq.guowangkeji.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://jeu.meibo888.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ywj.sweek.top

Ruby: def total(*nums); nums.sum; end
来源：http://sll.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://twe.gotoacloud.top

[C04] 命名参数 / 关键字参数
来源：http://pmb.yj20258.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://dmm.c1oappe.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gfy.hnxiangtu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wuc.zhengqikj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://bal.hammf.cn

Java: // 无：用 Builder 模式或 record
来源：http://mvn.shzxlz.cn

Go:   // 无：用配置结构体参数
来源：http://bek.52xcode.cn

Ruby: f(a: 1, b: 2)
来源：http://xba.gogol.net.cn

C#:   f(a: 1, b: 2)
来源：http://xrn.iojbl.cn

[C05] 返回多个值
来源：http://onk.sufxvd.cn

Py:   return a, b
来源：http://lzz.andypj.xyz

PHP:  return [$a, $b];
来源：http://zpy.wangdashe.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://wdo.birdmap.top

TS:   return { a, b };
来源：http://wjo.fzhhl.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ctr.tian-w.cn

Go:   return a, b
来源：http://smf.52xcode.cn

Ruby: return a, b
来源：http://xzw.meibo888.top

C#:   return (a, b);              // ValueTuple
来源：http://fxe.jinqigufen.top

[C06] 匿名函数 / lambda
来源：http://dmg.sweek.top

Py:   square = lambda x: x * x
来源：http://zpu.daxiang520.top

PHP:  $square = fn($x) => $x * $x;
来源：http://omy.guannengcc.top

JS:   const square = x => x * x;
来源：http://oev.xinyue.icu

TS:   const square = (x: number): number => x * x;
来源：http://ywr.cashguo.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://xmo.xuanzx.com

Go:   sq := func(x int) int { return x * x }
来源：http://gtk.ybcxt.top

Ruby: square = ->(x) { x * x }
来源：http://sqt.meibo888.top

C#:   Func<int, int> square = x => x * x;
来源：http://wtx.hcnkem.com

[C07] 把函数作为参数传入
来源：http://bwo.pengpengdd.cyou

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://yqc.jiagoushi.top

PHP:  array_map("strtoupper", $arr);
来源：http://bat.yfazqb.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://dlf.sweek.top

TS:   arr.map(String)
来源：http://aln.guannengcc.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zry.zhoulong.xyz

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://llv.iojbl.cn

Ruby: arr.map(&:upcase)
来源：http://jcq.jinqigfzy.top

C#:   arr.Select(s => s.ToUpper())
来源：http://fxx.jqgufenzy.top

[C08] 闭包
来源：http://rsr.zhoulong.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://xcb.wangdashe.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dbz.smart0.xyz

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://dcp.ivvv.top

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lgi.kuanghao11.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ehs.ywan-chungtsiang.top

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wzx.zhijiandao.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://omy.cucudq.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://rhe.dianchejie.cn

[C09] 递归
来源：http://cgh.chenzaomai.com

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://axn.haohaochexian.top

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ltc.fzhhl.top

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ddl.fengsongda.top

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ymc.jinyuanbaomall.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vvs.aibaodan.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lsz.zhongyouzk.top

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://lmd.cucudq.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://lek.yuanzhike.top


<!-- 参考信息 -->