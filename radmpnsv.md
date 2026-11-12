代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://ozb.tianlin.xyz

TS:   const value = data ?? "默认值";
来源：http://jxn.havefunace.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://awj.yueranfly.top

Go:   if data == "" { data = "默认值" }
来源：http://xdg.jianghu66.top

Ruby: value = data || "默认值"
来源：http://jix.zhoulong.xyz

C#:   var value = data ?? "默认值";
来源：http://xpm.ctjpmb.com

[A16] 真假值判断规则
来源：http://fuk.bjfxy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ruf.9152youxi.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://zas.fzhhl.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://rpc.ydjk.org.cn

TS:   if (!x) {}
来源：http://abo.zdbjq.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://nfr.tanke756.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mhm.guowangkeji.top

Ruby: unless x            # nil 与 false 为假
来源：http://aek.fanxiaobao.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sax.andypj.xyz

[A17] 位运算
来源：http://psw.cqqwz.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rnn.sjlbkw.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://iax.vehdjk.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://smz.yanxiufei.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://uja.cucudq.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://xrt.jinqigfzy.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://skt.hnqzz.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mok.wangdashe.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ryv.yongpay.top

[A18] 字符与 ASCII 码互转
来源：http://jnf.yfazqb.com

Py:   ord("A"); chr(65)
来源：http://ual.jianghu66.top

PHP:  ord("A"); chr(65)
来源：http://sap.nanxinkj.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sbz.cheryme.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hni.pycfn.com

Java: (int) 'A'; (char) 65
来源：http://rwa.gogol.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ncx.dashuyun.cn

Ruby: "A".ord; 65.chr
来源：http://nfq.nanxinkj.top

C#:   (int)'A'; (char)65
来源：http://cyg.dianchejie.cn

[A19] 交换两个变量
来源：http://gzg.fehbvm.com

Py:   a, b = b, a
来源：http://acb.xziqi.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://cwc.meibo888.top

JS:   [a, b] = [b, a];
来源：http://rhq.jyoumei.cn

TS:   [a, b] = [b, a];
来源：http://xnj.hcnkem.com

Java: int t = a; a = b; b = t;
来源：http://nyr.hysaishi.cn

Go:   a, b = b, a
来源：http://ygr.zycfv.cn

Ruby: a, b = b, a
来源：http://onp.nanxinkj.top

C#:   (a, b) = (b, a);
来源：http://edk.hywenlv.cn

[A20] 读取标准输入
来源：http://hna.hesvh.cn

Py:   name = input("请输入：")
来源：http://ukv.ybcxt.top

PHP:  $name = trim(fgets(STDIN));
来源：http://izf.haohaochexian.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ubq.yj202588.top

TS:   // Node.js：readline 模块
来源：http://mlx.dashuyun.cn

Java: new Scanner(System.in).nextLine()
来源：http://dvx.gotoacloud.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://fye.mhx1999.top

Ruby: gets.chomp
来源：http://xwp.ydjk.org.cn

C#:   Console.ReadLine();
来源：http://fzk.yfazqb.com

[A21] 保留指定小数位输出
来源：http://wax.daria6918.cn

Py:   f"{3.14159:.2f}"
来源：http://tfr.mhx1999.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rxe.jqgfzy.top

JS:   (3.14159).toFixed(2)
来源：http://vsj.zhongyouzk.top

TS:   (3.14159).toFixed(2)
来源：http://rzc.yongpay.top

Java: String.format("%.2f", 3.14159)
来源：http://glk.cucudq.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://zfo.shuidangran.top

Ruby: format("%.2f", 3.14159)
来源：http://ixz.ivvv.top

C#:   3.14159.ToString("F2")
来源：http://gct.jinqigfzy.top

[A22] 获取字符串长度
来源：http://tlk.havefunace.top

Py:   len(s)
来源：http://mxh.sysykeji.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://iza.daria6918.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eoz.shanyushiyangkeji.top

TS:   s.length
来源：http://egv.dashuyun.cn

Java: s.length()
来源：http://tuu.daxiang520.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://frz.shanyushiyangtech.top

Ruby: s.length
来源：http://fyy.birdmap.top

C#:   s.Length
来源：http://ilf.yueranfly.top

[A23] 大小写转换
来源：http://niy.316326.xyz

Py:   s.upper(); s.lower(); s.title()
来源：http://esu.gzhubu.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ghz.jinghuilouyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://nep.wangshuangyany.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://rzn.jianghu66.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zja.xuetiantiany.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ztw.haohaochexian.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hcd.nanxuanxn.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kte.tianlin.xyz

[A24] 去除首尾空白
来源：http://frx.xylfe.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://igu.nwbrower.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://xuk.shanyushiyangtech.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mhp.bjfxy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qqc.xylfe.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://xlq.zhoulong.xyz

Go:   strings.TrimSpace(s)
来源：http://epi.yj202588.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://awu.jiagoushi.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vrr.fanxiaobao.xyz

[A25] 字符串比较
来源：http://ytu.andypj.xyz

Py:   s1 == s2; s1 != s2
来源：http://etn.zhengqikj.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jvo.havefunace.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vvp.fzhhl.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rof.yj20258.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pfv.jyoumei.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gel.52xcode.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://ovo.zhixingplan.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://twx.52xcode.cn

[A26] 类型转换总览
来源：http://ssl.yuxming.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ltm.meibo888.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jyd.epnwcf.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://klp.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://tsf.jinqigufen.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zwf.yvedp.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cqt.andypj.xyz

Ruby: to_i to_f to_s to_sym to_a
来源：http://zse.bbcook.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://sch.hfpthk.cn

================================================================================
来源：http://rpu.mhx1999.top

B. 流程控制
来源：http://dsb.yj202588.top

================================================================================
来源：http://pdu.zdqjudy.top

[B01] 条件判断 if / else
来源：http://zmb.havefunace.top

Py:   result = "正" if x > 0 else "非正"
来源：http://qkp.kuanghao11.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kmm.jqgfzy.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://buz.jinghuilouyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lug.chenlongwang.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://wfh.zhaomingkeji.xyz

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://enb.pycfn.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://dyz.shuidangran.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://piw.316326.xyz

[B02] 多分支 else if / elif
来源：http://uqd.pengpengdd.cyou

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://rge.52xcode.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://oko.bbcook.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vdk.fanxiaobao.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cyx.ppjwa.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rdu.ydzc1.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://iyg.sufxvd.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hbf.tian-w.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jci.shuidangran.top

[B03] switch / match / case
来源：http://gsk.nwbrower.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ebx.ydjk.org.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://diw.xziqi.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://acb.sysykeji.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://owz.316326.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://gsj.chenlongwang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qrk.shuidangran.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jxs.sysykeji.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kyt.xingfuxueyuan.xyz

[B04] for 计数循环
来源：http://cip.xziqi.cn

Py:   for i in range(10): print(i)
来源：http://ykw.sweek.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://epv.yj20258888.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vlc.nwbrower.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://znf.uphjek.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xnk.xuanzx.com

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tan.shangyingyoupin.top

Ruby: 10.times { |i| puts i }
来源：http://omt.jiagoushi.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://uom.hammf.cn

[B05] 遍历数组 / 列表
来源：http://kkl.xinyue.icu

Py:   for item in arr: print(item)
来源：http://cru.mhx1999.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qbu.ydzc1.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gqp.cheryme.top

TS:   for (const item of arr) { console.log(item); }
来源：http://nbd.ydjk.org.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://gyx.cqqwz.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ssm.yueranfly.top

Ruby: arr.each { |item| puts item }
来源：http://ycy.tianlin.xyz

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wle.jiagoushi.top

[B06] 遍历字典 / 对象
来源：http://dsl.vqdsnc.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://ecb.zdqjudy.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://tvs.vehdjk.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eco.cqqwz.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eyr.xingfuxueyuan.xyz

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qbq.shzxlz.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://buf.quarkkingdee.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://pkh.zhoulong.xyz

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wyx.sxryk.cn

[B07] while 循环
来源：http://nlh.yueranfly.top

Py:   while i < 10: i += 1
来源：http://csl.iojbl.cn

PHP:  while ($i < 10) { $i++; }
来源：http://heo.aizwys.cn

JS:   while (i < 10) { i++; }
来源：http://aub.yuxming.cn

TS:   while (i < 10) { i++; }
来源：http://boj.snrcjt.cn

Java: while (i < 10) { i++; }
来源：http://vka.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://qkn.hnxiangtu.top

Ruby: while i < 10; i += 1; end
来源：http://rsq.zdbjq.cn

C#:   while (i < 10) { i++; }
来源：http://xkx.zycfv.cn

[B08] do-while（至少执行一次）
来源：http://clc.gotoacloud.top

Py:   # 无 do-while：用 while True + break
来源：http://qyt.tarul.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://sij.jyoumei.cn

JS:   do { i++; } while (i < 10);
来源：http://dfh.yueranfly.top

TS:   do { i++; } while (i < 10);
来源：http://deh.pycfn.com

Java: do { i++; } while (i < 10);
来源：http://ujx.jlsjyb.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://puv.sweek.top

Ruby: begin; i += 1; end while i < 10
来源：http://nvp.ehwqpu.com

C#:   do { i++; } while (i < 10);
来源：http://rpq.sweek.top

[B09] break 与 continue
来源：http://vbk.yj202588.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nsr.jyoumei.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cad.fzhhl.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ple.fzhhl.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jjl.jinqigufen.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vsj.birdmap.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://fbq.jlsjyb.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://qzf.sufxvd.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cdh.shanyushiyangkeji.top

[B10] 遍历同时拿索引
来源：http://pyv.daria6918.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gdh.316326.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://kzp.shzxlz.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hhn.cqqwz.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://jzp.sjlbkw.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bai.daxiang520.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://col.gogol.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xcw.jiagoushi.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://eyt.haohaochexian.top

[B11] 生成数字序列 / 区间
来源：http://itp.sweek.top

Py:   list(range(0, 10, 2))
来源：http://uyp.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://fyv.shzxlz.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://eof.daria6918.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://pnh.shanyushiyangtech.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://bjo.ybcxt.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cgy.sjlbkw.cn

Ruby: (0...10).step(2).to_a
来源：http://hwr.sufxvd.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://jxq.cucudq.cn

[B12] 跳出多层循环
来源：http://lhp.ivvv.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://elt.ydjk.org.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zxl.zdbjq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://lza.dashuyun.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tkl.yj20258.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://vjx.dianchejie.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://igg.kuanghao11.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://lum.9152youxi.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://eaf.ydzc1.top

[B13] 判断是否为数字
来源：http://alq.chenlongwang.top

Py:   isinstance(x, (int, float))
来源：http://rul.bbcook.cn

PHP:  is_numeric($x)
来源：http://hjv.zhongyouzk.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ibt.52xcode.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://idg.sxryk.cn

Java: x instanceof Number
来源：http://vre.zhaomingkeji.xyz

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://cdx.sweek.top

Ruby: x.is_a?(Numeric)
来源：http://qfd.ydjk.org.cn

C#:   x is int or double or decimal
来源：http://fgn.sysykeji.top

[B14] 判断值是否在集合内
来源：http://bqd.tanke756.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://fpu.shangyingyoupin.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://abs.shuidangran.top

JS:   [1, 2, 3].includes(x)
来源：http://vbd.mhx1999.top

TS:   [1, 2, 3].includes(x)
来源：http://dxb.tarul.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://qfa.yfazqb.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kfy.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://ymn.hammf.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://yxi.nanxinkj.top

[B15] 布尔运算与取反
来源：http://mdo.fengsongda.top

Py:   a and b or not c
来源：http://glb.yangfankeji.com

PHP:  $a && $b || !$c
来源：http://xgf.hfpthk.cn

JS:   a && b || !c
来源：http://feh.shangyingyoupin.top

TS:   a && b || !c
来源：http://sxe.cashguo.top

Java: a && b || !c
来源：http://due.yvedp.cn

Go:   a && b || !c
来源：http://vyh.52xcode.cn

Ruby: a && b || !c
来源：http://iii.jqgufenzy.top

C#:   a && b || !c
来源：http://jua.zhijiandao.cn

[B16] 卫语句：不满足条件提前返回
来源：http://mvb.bjfxy.top

Py:   if not data: return
来源：http://umo.shanyushiyangkeji.top

PHP:  if (!$data) { return; }
来源：http://nxz.fehbvm.com

JS:   if (!data) return;
来源：http://mjp.wangshuangyany.cn

TS:   if (!data) return;
来源：http://bzp.yangfankeji.com

Java: if (data == null) return;
来源：http://dpe.tarul.cn

Go:   if data == nil { return }
来源：http://doj.yonumen.top

Ruby: return if data.nil?
来源：http://bee.cucudq.cn

C#:   if (data == null) return;
来源：http://xbc.0kj1m.cn

================================================================================
来源：http://ips.gzhubu.top

C. 函数与作用域
来源：http://yvn.xylfe.cn

================================================================================
来源：http://fua.zhiwuduotai.top

[C01] 定义函数
来源：http://aib.redwolf501.top

Py:   def add(a, b): return a + b
来源：http://xlr.vehdjk.com

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jel.zhiwuduotai.top

JS:   function add(a, b) { return a + b; }
来源：http://dcb.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nta.guannengcc.top

Java: static int add(int a, int b) { return a + b; }
来源：http://ujs.hfpthk.cn

Go:   func add(a, b int) int { return a + b }
来源：http://dqz.fanxiaobao.xyz

Ruby: def add(a, b); a + b; end
来源：http://oum.snrcjt.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wfp.fengsongda.top

[C02] 默认参数
来源：http://vco.shanyushiyangtech.top

Py:   def greet(name="World"): return name
来源：http://omc.fanxiaobao.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://enf.aizwys.cn

JS:   function greet(name = "World") { return name; }
来源：http://hki.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://gxj.xylfe.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://xyh.zhaomingkeji.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hne.hysaishi.cn

Ruby: def greet(name = "World") = name
来源：http://nyl.hfpthk.cn

C#:   string Greet(string name = "World") => name;
来源：http://eev.ydzc1.top

[C03] 可变参数
来源：http://wxj.cheryme.top

Py:   def total(*args): return sum(args)
来源：http://zhl.zhongyouzk.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://cco.vqdsnc.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lzb.xziqi.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://ypg.tianlin.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tbm.zhaomingkeji.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zho.gaohongyu789.top

Ruby: def total(*nums); nums.sum; end
来源：http://pkl.tarul.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://lpk.zycfv.cn

[C04] 命名参数 / 关键字参数
来源：http://jsa.kuanghao11.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hpb.hammf.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wkc.yanxiufei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://nxi.zhengqikj.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wka.zhiwuduotai.top

Java: // 无：用 Builder 模式或 record
来源：http://qgj.jqgufenzy.top

Go:   // 无：用配置结构体参数
来源：http://krd.ppjwa.cn

Ruby: f(a: 1, b: 2)
来源：http://cva.yvedp.cn

C#:   f(a: 1, b: 2)
来源：http://jla.yangfankeji.com

[C05] 返回多个值
来源：http://pfc.meibo888.top

Py:   return a, b
来源：http://hrb.cdnleiting.top

PHP:  return [$a, $b];
来源：http://alk.yvedp.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://bru.quarkkingdee.top

TS:   return { a, b };
来源：http://bpm.xinyue.icu

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hkm.smart0.xyz

Go:   return a, b
来源：http://dft.hongshengwenyu.top

Ruby: return a, b
来源：http://pdn.shzxlz.cn

C#:   return (a, b);              // ValueTuple
来源：http://qwk.gogol.net.cn


<!-- 参考信息 -->