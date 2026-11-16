代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://rnh.shanyushiyangtech.top

TS:   const value = data ?? "默认值";
来源：http://plq.cdnleiting.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://upm.sufxvd.cn

Go:   if data == "" { data = "默认值" }
来源：http://bkd.sweek.top

Ruby: value = data || "默认值"
来源：http://gvc.nanxuanxn.top

C#:   var value = data ?? "默认值";
来源：http://siy.svipenyu.cn

[A16] 真假值判断规则
来源：http://fce.jyoumei.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://vxa.svipenyu.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qll.zhongyouzk.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ojo.chenzaomai.com

TS:   if (!x) {}
来源：http://azm.gotoacloud.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://dez.sxryk.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fnh.hcnkem.com

Ruby: unless x            # nil 与 false 为假
来源：http://szt.uphjek.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://clz.xziqi.cn

[A17] 位运算
来源：http://ivu.ivvv.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qav.dianchejie.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://lxr.c1oappe.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jmr.iojbl.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://per.hammf.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jpu.zhoulong.xyz

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://kfz.svipenyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qnj.hnxiangtu.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vck.shuidangran.top

[A18] 字符与 ASCII 码互转
来源：http://ocg.jlsjyb.cn

Py:   ord("A"); chr(65)
来源：http://dnq.meibo888.top

PHP:  ord("A"); chr(65)
来源：http://wbi.xylfe.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://flf.cashguo.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ray.dashuyun.cn

Java: (int) 'A'; (char) 65
来源：http://iwf.sufxvd.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://noj.sxryk.cn

Ruby: "A".ord; 65.chr
来源：http://uqk.quarkkingdee.top

C#:   (int)'A'; (char)65
来源：http://yjp.sxryk.cn

[A19] 交换两个变量
来源：http://qcm.wangdashe.top

Py:   a, b = b, a
来源：http://sss.cdnleiting.top

PHP:  [$a, $b] = [$b, $a];
来源：http://hdj.yongpay.top

JS:   [a, b] = [b, a];
来源：http://vmq.yvedp.cn

TS:   [a, b] = [b, a];
来源：http://ycc.andypj.xyz

Java: int t = a; a = b; b = t;
来源：http://ple.chenjidiqi.icu

Go:   a, b = b, a
来源：http://afb.yueranfly.top

Ruby: a, b = b, a
来源：http://nde.xinyue.icu

C#:   (a, b) = (b, a);
来源：http://xzb.ehwqpu.com

[A20] 读取标准输入
来源：http://xeq.hywenlv.cn

Py:   name = input("请输入：")
来源：http://qpl.xylfe.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://diq.yj20258888.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ude.fanxiaobao.xyz

TS:   // Node.js：readline 模块
来源：http://lls.yuxming.cn

Java: new Scanner(System.in).nextLine()
来源：http://byh.bbcook.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://nzb.zdbjq.cn

Ruby: gets.chomp
来源：http://dtl.yuanzhike.top

C#:   Console.ReadLine();
来源：http://yps.sysykeji.top

[A21] 保留指定小数位输出
来源：http://nuz.vehdjk.com

Py:   f"{3.14159:.2f}"
来源：http://ndq.pengpengdd.cyou

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zle.jinyuanbaomall.cn

JS:   (3.14159).toFixed(2)
来源：http://znz.havefunace.top

TS:   (3.14159).toFixed(2)
来源：http://eya.ctjpmb.com

Java: String.format("%.2f", 3.14159)
来源：http://wtp.sufxvd.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mgp.gotoacloud.top

Ruby: format("%.2f", 3.14159)
来源：http://wct.chenzaomai.com

C#:   3.14159.ToString("F2")
来源：http://bgc.nanxuanxn.top

[A22] 获取字符串长度
来源：http://igx.sufxvd.cn

Py:   len(s)
来源：http://sys.jqgfzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zyd.vehdjk.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://zlp.ppjwa.cn

TS:   s.length
来源：http://sza.yfazqb.com

Java: s.length()
来源：http://phl.zhiwuduotai.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qul.gzhubu.top

Ruby: s.length
来源：http://txo.aizwys.cn

C#:   s.Length
来源：http://zgx.gzhubu.top

[A23] 大小写转换
来源：http://ylj.redwolf501.top

Py:   s.upper(); s.lower(); s.title()
来源：http://apo.zhiwuduotai.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://jul.ywan-chungtsiang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ale.shanyushiyangkeji.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://awz.zhoulong.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ftm.zhengqikj.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ggv.daxiang520.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cvx.daxiang520.top

C#:   s.ToUpper(); s.ToLower()
来源：http://byu.daria6918.cn

[A24] 去除首尾空白
来源：http://ixf.xziqi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wtj.xziqi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kdh.ppjwa.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nuk.zhixingplan.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vhx.shangyingyoupin.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://dic.xingfuxueyuan.xyz

Go:   strings.TrimSpace(s)
来源：http://ztp.guannengcc.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://uyw.andypj.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://bbo.52xcode.cn

[A25] 字符串比较
来源：http://sjp.yj202588.top

Py:   s1 == s2; s1 != s2
来源：http://jzn.wangshuangyany.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://vjy.dashuyun.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://isr.ehwqpu.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rum.yueranfly.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nfx.daxiang520.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mst.yuxming.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://elr.chenjidiqi.icu

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://jhk.sxryk.cn

[A26] 类型转换总览
来源：http://qvf.yongpay.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jvd.snrcjt.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://jyz.chenlongwang.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zmh.ydjk.org.cn

TS:   Number() String() Boolean() x as number
来源：http://wgq.ivvv.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://fzh.ydzc1.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://meb.aizwys.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://vua.jinqigfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uyz.vqdsnc.cn

================================================================================
来源：http://dpj.xziqi.cn

B. 流程控制
来源：http://tlq.ywan-chungtsiang.top

================================================================================
来源：http://ivn.jinghuilouyu.cn

[B01] 条件判断 if / else
来源：http://etb.iojbl.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://dul.jinyuanbaomall.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://kil.xinyue.icu

JS:   const r = x > 0 ? "正" : "非正";
来源：http://flx.meibo888.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://nup.xinyue.icu

Java: String r = x > 0 ? "正" : "非正";
来源：http://dbj.hammf.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://roz.chenjidiqi.icu

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hyh.jiagoushi.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://prs.jianghu66.top

[B02] 多分支 else if / elif
来源：http://gcj.jqgufenzy.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ydp.yueranfly.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://nob.hesvh.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wrb.pycfn.com

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://asy.zhengqikj.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fwg.gotoacloud.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kgf.havefunace.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://zpn.hywenlv.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://kkl.fanxiaobao.xyz

[B03] switch / match / case
来源：http://hgn.fengsongda.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vzn.fengsongda.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://lra.guowangkeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://emn.cheryme.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://vhp.zhijiandao.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://exk.uphjek.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://skr.jqgfzy.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hbg.ywan-chungtsiang.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tbb.ppjwa.cn

[B04] for 计数循环
来源：http://idq.nanxinkj.top

Py:   for i in range(10): print(i)
来源：http://pgk.yvedp.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qco.sufxvd.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yfd.yueranfly.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kkx.xinyue.icu

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://qoh.snrcjt.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://gzx.hcnkem.com

Ruby: 10.times { |i| puts i }
来源：http://zje.shzxlz.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://piz.meibo888.top

[B05] 遍历数组 / 列表
来源：http://kmb.haohaochexian.top

Py:   for item in arr: print(item)
来源：http://lwu.uphjek.com

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jke.316326.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://xsd.shanyushiyangkeji.top

TS:   for (const item of arr) { console.log(item); }
来源：http://gjk.pengpengdd.cyou

Java: for (var item : arr) { System.out.println(item); }
来源：http://zti.xziqi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gfw.jiagoushi.top

Ruby: arr.each { |item| puts item }
来源：http://jgk.snrcjt.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mux.feifeiyinyue.top

[B06] 遍历字典 / 对象
来源：http://res.shanyushiyangtech.top

Py:   for k, v in d.items(): print(k, v)
来源：http://bnp.ybcxt.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://fwt.fzhhl.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tlu.yj202588.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://drf.xziqi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://rkz.jqgfzy.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nuz.cdnleiting.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://kra.vehdjk.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://viz.pengpengdd.cyou

[B07] while 循环
来源：http://jaf.52xcode.cn

Py:   while i < 10: i += 1
来源：http://dju.gzhubu.top

PHP:  while ($i < 10) { $i++; }
来源：http://tql.jiagoushi.top

JS:   while (i < 10) { i++; }
来源：http://vfi.yonumen.top

TS:   while (i < 10) { i++; }
来源：http://tux.sweek.top

Java: while (i < 10) { i++; }
来源：http://pmp.zhongyouzk.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://bsy.tian-w.cn

Ruby: while i < 10; i += 1; end
来源：http://fvs.ctjpmb.com

C#:   while (i < 10) { i++; }
来源：http://upa.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://goj.meibo888.top

Py:   # 无 do-while：用 while True + break
来源：http://yaz.hongshengwenyu.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fmk.yj202588.top

JS:   do { i++; } while (i < 10);
来源：http://apz.cucudq.cn

TS:   do { i++; } while (i < 10);
来源：http://awq.svipenyu.cn

Java: do { i++; } while (i < 10);
来源：http://mkn.c1oappe.top

Go:   for { i++; if i >= 10 { break } }
来源：http://bqi.cucudq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://knj.meibo888.top

C#:   do { i++; } while (i < 10);
来源：http://xvr.ydjk.org.cn

[B09] break 与 continue
来源：http://pxo.shanyushiyangtech.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lqw.daxiang520.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://uie.hfpthk.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fkz.kuanghao11.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nxw.meibo888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ffl.epnwcf.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jul.yfazqb.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://kko.tarul.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://svp.yuxming.cn

[B10] 遍历同时拿索引
来源：http://hbr.cheryme.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://nut.zdbjq.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qjp.yanxiufei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://llf.cashguo.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://thl.yueranfly.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xkt.shangyingyoupin.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mbc.quarkkingdee.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hin.jinyuanbaomall.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://euq.ehwqpu.com

[B11] 生成数字序列 / 区间
来源：http://nlu.uphjek.com

Py:   list(range(0, 10, 2))
来源：http://sfr.jqgufenzy.top

PHP:  range(0, 10, 2);
来源：http://sog.tianlin.xyz

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uga.xinyue.icu

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://riq.jqgufenzy.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://lzv.vehdjk.com

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://iwn.guannengcc.top

Ruby: (0...10).step(2).to_a
来源：http://zfu.zhijiandao.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://gna.yfazqb.com

[B12] 跳出多层循环
来源：http://qlm.shanyushiyangkeji.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://mud.yvedp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://eei.gotoacloud.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zol.sweek.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ang.hnqzz.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://lpf.ywan-chungtsiang.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mpa.hesvh.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://oir.quarkkingdee.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://ynm.cqqwz.cn

[B13] 判断是否为数字
来源：http://xrq.cdnleiting.top

Py:   isinstance(x, (int, float))
来源：http://tdj.sweek.top

PHP:  is_numeric($x)
来源：http://rcf.ppjwa.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yad.tanke756.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://adq.bjfxy.top

Java: x instanceof Number
来源：http://iwk.hnxiangtu.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://olz.hesvh.cn

Ruby: x.is_a?(Numeric)
来源：http://qyl.cashguo.top

C#:   x is int or double or decimal
来源：http://aio.tanke756.top

[B14] 判断值是否在集合内
来源：http://jcu.nanxinkj.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://yhw.tianlin.xyz

PHP:  in_array($x, [1, 2, 3], true)
来源：http://chr.fengsongda.top

JS:   [1, 2, 3].includes(x)
来源：http://hmt.sjlbkw.cn

TS:   [1, 2, 3].includes(x)
来源：http://vrw.fehbvm.com

Java: List.of(1, 2, 3).contains(x)
来源：http://pci.jinqigufen.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lvt.havefunace.top

Ruby: [1, 2, 3].include?(x)
来源：http://sai.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iph.yonumen.top

[B15] 布尔运算与取反
来源：http://zqz.yvedp.cn

Py:   a and b or not c
来源：http://gkm.zycfv.cn

PHP:  $a && $b || !$c
来源：http://vws.0kj1m.cn

JS:   a && b || !c
来源：http://pki.yj20258888.top

TS:   a && b || !c
来源：http://asx.havefunace.top

Java: a && b || !c
来源：http://hwr.nanxinkj.top

Go:   a && b || !c
来源：http://elu.jinqigfzy.top

Ruby: a && b || !c
来源：http://ipy.pycfn.com

C#:   a && b || !c
来源：http://fxa.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://juv.tanke756.top

Py:   if not data: return
来源：http://iag.vehdjk.com

PHP:  if (!$data) { return; }
来源：http://qly.ydzc1.top

JS:   if (!data) return;
来源：http://wfm.xylfe.cn

TS:   if (!data) return;
来源：http://zed.yj202588.top

Java: if (data == null) return;
来源：http://igp.jlsjyb.cn

Go:   if data == nil { return }
来源：http://fbl.hnqzz.top

Ruby: return if data.nil?
来源：http://ocd.xziqi.cn

C#:   if (data == null) return;
来源：http://weo.gogol.net.cn

================================================================================
来源：http://fqy.zdqjudy.top

C. 函数与作用域
来源：http://qip.zhiwuduotai.top

================================================================================
来源：http://los.hnxiangtu.top

[C01] 定义函数
来源：http://inc.meibo888.top

Py:   def add(a, b): return a + b
来源：http://qyo.nanxinkj.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://msu.hnxiangtu.top

JS:   function add(a, b) { return a + b; }
来源：http://zcg.ydzc1.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bqc.yonumen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://mdp.jinyuanbaomall.cn

Go:   func add(a, b int) int { return a + b }
来源：http://xqa.zhoulong.xyz

Ruby: def add(a, b); a + b; end
来源：http://rcn.guowangkeji.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://vfw.9152youxi.cn

[C02] 默认参数
来源：http://gut.xylfe.cn

Py:   def greet(name="World"): return name
来源：http://wao.zhongyouzk.top

PHP:  function greet($name = "World") { return $name; }
来源：http://elo.ydzc1.top

JS:   function greet(name = "World") { return name; }
来源：http://eyv.hnxiangtu.top

TS:   function greet(name: string = "World") { return name; }
来源：http://jkt.zdbjq.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://gsf.birdmap.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://kpg.fanxiaobao.xyz

Ruby: def greet(name = "World") = name
来源：http://ckz.chenjidiqi.icu

C#:   string Greet(string name = "World") => name;
来源：http://mfh.fanxiaobao.xyz

[C03] 可变参数
来源：http://tpm.redwolf501.top

Py:   def total(*args): return sum(args)
来源：http://nbk.tianlin.xyz

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://gtz.aizwys.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://lrt.jinghuilouyu.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://neg.jinqigufen.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qwq.0kj1m.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wuo.zhengqikj.top

Ruby: def total(*nums); nums.sum; end
来源：http://gba.dianchejie.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://boj.hcnkem.com

[C04] 命名参数 / 关键字参数
来源：http://xkl.iojbl.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yxk.pengpengdd.cyou

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://kne.svipenyu.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://fcc.zdbjq.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://nnv.ydzc1.top

Java: // 无：用 Builder 模式或 record
来源：http://qvp.gogol.net.cn

Go:   // 无：用配置结构体参数
来源：http://nxz.epnwcf.com

Ruby: f(a: 1, b: 2)
来源：http://taw.sxryk.cn

C#:   f(a: 1, b: 2)
来源：http://zkq.aibaodan.cn

[C05] 返回多个值
来源：http://brr.xziqi.cn

Py:   return a, b
来源：http://cdv.feifeiyinyue.top

PHP:  return [$a, $b];
来源：http://ces.jinqigfzy.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ysm.dianchejie.cn

TS:   return { a, b };
来源：http://ych.nanxinkj.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://icy.zhaomingkeji.xyz

Go:   return a, b
来源：http://dvb.andypj.xyz

Ruby: return a, b
来源：http://lvx.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://tim.ivvv.top


<!-- 参考信息 -->