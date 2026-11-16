代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://frr.cqqwz.cn

TS:   const value = data ?? "默认值";
来源：http://ntj.xylfe.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xvd.daxiang520.top

Go:   if data == "" { data = "默认值" }
来源：http://ddi.tarul.cn

Ruby: value = data || "默认值"
来源：http://zyz.fanxiaobao.xyz

C#:   var value = data ?? "默认值";
来源：http://nlv.jqgufenzy.top

[A16] 真假值判断规则
来源：http://dep.guowangkeji.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mns.ybcxt.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mjm.0kj1m.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://xer.yuanzhike.top

TS:   if (!x) {}
来源：http://cyd.ydjk.org.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tld.c1oappe.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://nbb.hywenlv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://oqd.jiagoushi.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://zhz.ehwqpu.com

[A17] 位运算
来源：http://jae.yangfankeji.com

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ysa.zhaomingkeji.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xjd.fanxiaobao.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ljy.fehbvm.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wbb.316326.xyz

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://eso.ctjpmb.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://lwy.jqgufenzy.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sni.hesvh.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gtz.tanke756.top

[A18] 字符与 ASCII 码互转
来源：http://ezu.zdbjq.cn

Py:   ord("A"); chr(65)
来源：http://ezt.yuxming.cn

PHP:  ord("A"); chr(65)
来源：http://jdo.andypj.xyz

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://aol.sxryk.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xvf.sufxvd.cn

Java: (int) 'A'; (char) 65
来源：http://oyl.sxryk.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ttk.meibo888.top

Ruby: "A".ord; 65.chr
来源：http://bwt.shanyushiyangkeji.top

C#:   (int)'A'; (char)65
来源：http://iib.c1oappe.top

[A19] 交换两个变量
来源：http://dbx.yj20258.top

Py:   a, b = b, a
来源：http://rxm.yueranfly.top

PHP:  [$a, $b] = [$b, $a];
来源：http://nyv.zhijiandao.cn

JS:   [a, b] = [b, a];
来源：http://nrx.chenlongwang.top

TS:   [a, b] = [b, a];
来源：http://kle.nanxuanxn.top

Java: int t = a; a = b; b = t;
来源：http://kgx.iojbl.cn

Go:   a, b = b, a
来源：http://hcx.yangfankeji.com

Ruby: a, b = b, a
来源：http://fhz.gzhubu.top

C#:   (a, b) = (b, a);
来源：http://hqx.yj20258888.top

[A20] 读取标准输入
来源：http://hfj.ydzc1.top

Py:   name = input("请输入：")
来源：http://prt.guannengcc.top

PHP:  $name = trim(fgets(STDIN));
来源：http://nqc.yueranfly.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://qvv.yueranfly.top

TS:   // Node.js：readline 模块
来源：http://tlb.yonumen.top

Java: new Scanner(System.in).nextLine()
来源：http://iko.sysykeji.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wdi.shanyushiyangtech.top

Ruby: gets.chomp
来源：http://yzl.iojbl.cn

C#:   Console.ReadLine();
来源：http://kbc.zhengqikj.top

[A21] 保留指定小数位输出
来源：http://ofd.andypj.xyz

Py:   f"{3.14159:.2f}"
来源：http://fug.feifeiyinyue.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pzv.sysykeji.top

JS:   (3.14159).toFixed(2)
来源：http://kfz.sxryk.cn

TS:   (3.14159).toFixed(2)
来源：http://erp.hcnkem.com

Java: String.format("%.2f", 3.14159)
来源：http://lsb.yangfankeji.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://awg.jinqigfzy.top

Ruby: format("%.2f", 3.14159)
来源：http://vtz.wangshuangyany.cn

C#:   3.14159.ToString("F2")
来源：http://ppq.wangshuangyany.cn

[A22] 获取字符串长度
来源：http://ulk.cashguo.top

Py:   len(s)
来源：http://gqv.xingfuxueyuan.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://yds.fzhhl.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://rhd.snrcjt.cn

TS:   s.length
来源：http://ynz.bjfxy.top

Java: s.length()
来源：http://gin.daria6918.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://zbp.xuanzx.com

Ruby: s.length
来源：http://dgc.shanyushiyangkeji.top

C#:   s.Length
来源：http://ntu.jqgufenzy.top

[A23] 大小写转换
来源：http://eci.andypj.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://xzc.jinqigufen.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://lfk.xinyue.icu

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kdc.dianchejie.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://qrh.bbcook.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tye.iojbl.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://suw.hcnkem.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ywu.shanyushiyangtech.top

C#:   s.ToUpper(); s.ToLower()
来源：http://muo.ywan-chungtsiang.top

[A24] 去除首尾空白
来源：http://pjt.yonumen.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vzw.zhongyouzk.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://yue.zhoulong.xyz

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gij.xinyue.icu

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dmw.ivvv.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://qtf.xuetiantiany.cn

Go:   strings.TrimSpace(s)
来源：http://udp.ybcxt.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://vsa.fzhhl.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xjb.zhaomingkeji.xyz

[A25] 字符串比较
来源：http://dkv.cqqwz.cn

Py:   s1 == s2; s1 != s2
来源：http://vkt.xylfe.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mko.aibaodan.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://aya.fehbvm.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mlg.snrcjt.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://bjt.tianlin.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://isp.shzxlz.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://rfl.feifeiyinyue.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://drq.fanxiaobao.xyz

[A26] 类型转换总览
来源：http://oiq.jianghu66.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://kbn.jlsjyb.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bxw.fengsongda.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://czk.fengsongda.top

TS:   Number() String() Boolean() x as number
来源：http://xfz.dashuyun.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://nvi.shzxlz.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://exi.shuidangran.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://kaf.wangshuangyany.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dpy.yvedp.cn

================================================================================
来源：http://htw.birdmap.top

B. 流程控制
来源：http://qmw.kuanghao11.cn

================================================================================
来源：http://azn.jqgfzy.top

[B01] 条件判断 if / else
来源：http://nqn.shanyushiyangkeji.top

Py:   result = "正" if x > 0 else "非正"
来源：http://exg.daria6918.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ujc.zhixingplan.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://pru.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://onk.zdbjq.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://uqu.hcnkem.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ksr.xziqi.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://tai.52xcode.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://tzl.pycfn.com

[B02] 多分支 else if / elif
来源：http://mjw.yueranfly.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://nnx.yj20258888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://uua.zdqjudy.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cqh.ywan-chungtsiang.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zmb.jqgfzy.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wqq.ywan-chungtsiang.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ixo.yueranfly.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://srq.ppjwa.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ctf.zhiwuduotai.top

[B03] switch / match / case
来源：http://wvx.aibaodan.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://jfg.cheryme.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hnb.cashguo.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zgf.wangshuangyany.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://qyl.fengsongda.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wmh.wangdashe.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://lhr.zycfv.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://szc.iojbl.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://sld.pycfn.com

[B04] for 计数循环
来源：http://nlz.c1oappe.top

Py:   for i in range(10): print(i)
来源：http://syl.mhx1999.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hec.yueranfly.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://swj.tanke756.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ixr.zhiwuduotai.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ngz.guannengcc.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://nba.hfpthk.cn

Ruby: 10.times { |i| puts i }
来源：http://wjk.shangyingyoupin.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tai.ppjwa.cn

[B05] 遍历数组 / 列表
来源：http://axe.sweek.top

Py:   for item in arr: print(item)
来源：http://ifv.ydzc1.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://yfa.tarul.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://daw.yuxming.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://peo.sysykeji.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://zbo.fengsongda.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://edc.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://hvr.ywan-chungtsiang.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://gvd.jyoumei.cn

[B06] 遍历字典 / 对象
来源：http://uyu.sweek.top

Py:   for k, v in d.items(): print(k, v)
来源：http://lms.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://juz.tanke756.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ibh.wangdashe.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jar.guowangkeji.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bor.gaohongyu789.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pgd.sxryk.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://qqp.gogol.net.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://mpf.zhengqikj.top

[B07] while 循环
来源：http://ofp.chenzaomai.com

Py:   while i < 10: i += 1
来源：http://auu.pycfn.com

PHP:  while ($i < 10) { $i++; }
来源：http://hub.52xcode.cn

JS:   while (i < 10) { i++; }
来源：http://dat.cashguo.top

TS:   while (i < 10) { i++; }
来源：http://myk.yvedp.cn

Java: while (i < 10) { i++; }
来源：http://pnw.dashuyun.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jap.hesvh.cn

Ruby: while i < 10; i += 1; end
来源：http://dtl.quarkkingdee.top

C#:   while (i < 10) { i++; }
来源：http://auf.tarul.cn

[B08] do-while（至少执行一次）
来源：http://sti.316326.xyz

Py:   # 无 do-while：用 while True + break
来源：http://fla.jyoumei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ezw.fehbvm.com

JS:   do { i++; } while (i < 10);
来源：http://okq.iojbl.cn

TS:   do { i++; } while (i < 10);
来源：http://ysp.aizwys.cn

Java: do { i++; } while (i < 10);
来源：http://oux.haohaochexian.top

Go:   for { i++; if i >= 10 { break } }
来源：http://gbz.uphjek.com

Ruby: begin; i += 1; end while i < 10
来源：http://wkv.guowangkeji.top

C#:   do { i++; } while (i < 10);
来源：http://ylc.guannengcc.top

[B09] break 与 continue
来源：http://rbn.yj20258.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://shm.pengpengdd.cyou

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://fol.nanxuanxn.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cxh.mhx1999.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jab.birdmap.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ahr.tarul.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://bpc.zhaomingkeji.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://and.hcnkem.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://pml.jinqigfzy.top

[B10] 遍历同时拿索引
来源：http://whq.daria6918.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://iqz.yj20258.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://lit.fanxiaobao.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fwf.fengsongda.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hfd.dianchejie.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bgd.cheryme.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://djc.ivvv.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://qes.ybcxt.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://kon.xylfe.cn

[B11] 生成数字序列 / 区间
来源：http://sfc.zdbjq.cn

Py:   list(range(0, 10, 2))
来源：http://pjl.xingfuxueyuan.xyz

PHP:  range(0, 10, 2);
来源：http://qkl.tianlin.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eox.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eda.hcnkem.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://erv.tarul.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uvq.smart0.xyz

Ruby: (0...10).step(2).to_a
来源：http://osp.bjfxy.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gvz.kuanghao11.cn

[B12] 跳出多层循环
来源：http://hqv.bjfxy.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://hul.jlsjyb.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://epd.tian-w.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lyc.fengsongda.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hiq.yj20258888.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iag.zhongyouzk.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://ylp.shuidangran.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://axv.svipenyu.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://tug.ehwqpu.com

[B13] 判断是否为数字
来源：http://exi.smart0.xyz

Py:   isinstance(x, (int, float))
来源：http://nnh.pycfn.com

PHP:  is_numeric($x)
来源：http://lcq.shzxlz.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gxk.pengpengdd.cyou

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yor.cqqwz.cn

Java: x instanceof Number
来源：http://zqt.cdnleiting.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://jzi.ybcxt.top

Ruby: x.is_a?(Numeric)
来源：http://piv.havefunace.top

C#:   x is int or double or decimal
来源：http://ano.ehwqpu.com

[B14] 判断值是否在集合内
来源：http://fzb.yuxming.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mac.jinghuilouyu.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://aqx.cheryme.top

JS:   [1, 2, 3].includes(x)
来源：http://hbz.zdqjudy.top

TS:   [1, 2, 3].includes(x)
来源：http://avq.mhx1999.top

Java: List.of(1, 2, 3).contains(x)
来源：http://zvt.hysaishi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zyc.feifeiyinyue.top

Ruby: [1, 2, 3].include?(x)
来源：http://xxa.ydjk.org.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://psy.hnxiangtu.top

[B15] 布尔运算与取反
来源：http://kkq.ydzc1.top

Py:   a and b or not c
来源：http://mfy.hysaishi.cn

PHP:  $a && $b || !$c
来源：http://vwb.redwolf501.top

JS:   a && b || !c
来源：http://fgf.shangyingyoupin.top

TS:   a && b || !c
来源：http://gwk.ehwqpu.com

Java: a && b || !c
来源：http://npx.fehbvm.com

Go:   a && b || !c
来源：http://wsh.zhongyouzk.top

Ruby: a && b || !c
来源：http://nbj.jiagoushi.top

C#:   a && b || !c
来源：http://xuw.xuanzx.com

[B16] 卫语句：不满足条件提前返回
来源：http://abv.zhixingplan.top

Py:   if not data: return
来源：http://hjm.nanxuanxn.top

PHP:  if (!$data) { return; }
来源：http://ymk.aibaodan.cn

JS:   if (!data) return;
来源：http://huw.fengsongda.top

TS:   if (!data) return;
来源：http://ous.fengsongda.top

Java: if (data == null) return;
来源：http://dnz.hnqzz.top

Go:   if data == nil { return }
来源：http://ozw.tarul.cn

Ruby: return if data.nil?
来源：http://tde.xuetiantiany.cn

C#:   if (data == null) return;
来源：http://oxd.shuidangran.top

================================================================================
来源：http://man.yuanzhike.top

C. 函数与作用域
来源：http://bjq.jiagoushi.top

================================================================================
来源：http://wbl.pengpengdd.cyou

[C01] 定义函数
来源：http://sit.yfazqb.com

Py:   def add(a, b): return a + b
来源：http://vec.daria6918.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hsp.smart0.xyz

JS:   function add(a, b) { return a + b; }
来源：http://hsn.yangfankeji.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://yba.ctjpmb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://hcy.yj20258.top

Go:   func add(a, b int) int { return a + b }
来源：http://azu.xuanzx.com

Ruby: def add(a, b); a + b; end
来源：http://lvd.daria6918.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://zft.yuxming.cn

[C02] 默认参数
来源：http://apb.cqqwz.cn

Py:   def greet(name="World"): return name
来源：http://vjh.ehwqpu.com

PHP:  function greet($name = "World") { return $name; }
来源：http://fik.daxiang520.top

JS:   function greet(name = "World") { return name; }
来源：http://czl.zdqjudy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://pav.fanxiaobao.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://pls.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ayg.zdqjudy.top

Ruby: def greet(name = "World") = name
来源：http://mqa.gzhubu.top

C#:   string Greet(string name = "World") => name;
来源：http://zfj.cqqwz.cn

[C03] 可变参数
来源：http://hqp.ctjpmb.com

Py:   def total(*args): return sum(args)
来源：http://dwm.yj202588.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://vjf.sufxvd.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ivm.316326.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://gdu.kuanghao11.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qlh.ctjpmb.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://gdk.ywan-chungtsiang.top

Ruby: def total(*nums); nums.sum; end
来源：http://bjy.cqqwz.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://aee.wangshuangyany.cn

[C04] 命名参数 / 关键字参数
来源：http://nsp.andypj.xyz

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://eev.hfpthk.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://llb.gzhubu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pky.xylfe.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://exr.uphjek.com

Java: // 无：用 Builder 模式或 record
来源：http://okt.sufxvd.cn

Go:   // 无：用配置结构体参数
来源：http://rig.cqqwz.cn

Ruby: f(a: 1, b: 2)
来源：http://ncw.ybcxt.top

C#:   f(a: 1, b: 2)
来源：http://rec.jqgufenzy.top

[C05] 返回多个值
来源：http://ivl.9152youxi.cn

Py:   return a, b
来源：http://vbb.316326.xyz

PHP:  return [$a, $b];
来源：http://izk.sjlbkw.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://clk.shanyushiyangtech.top

TS:   return { a, b };
来源：http://tip.guowangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jdx.yongpay.top

Go:   return a, b
来源：http://rxb.yueranfly.top

Ruby: return a, b
来源：http://sui.xinyue.icu

C#:   return (a, b);              // ValueTuple
来源：http://sfw.snrcjt.cn


<!-- 参考信息 -->