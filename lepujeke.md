代发 wailian999

[A14] 注释写法
来源：http://fey.hnxiangtu.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://beu.quarkkingdee.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://lzm.jinyuanbaomall.cn

JS:   // 单行；/* 多行 */
来源：http://ajh.jqgfzy.top

TS:   // 单行；/* 多行 */
来源：http://oed.shzxlz.cn

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://tdz.nanxuanxn.top

Go:   // 单行；/* 多行 */
来源：http://atm.yangfankeji.com

Ruby: # 单行；=begin 多行 =end
来源：http://bez.shangyingyoupin.top

C#:   // 单行；/* 多行 */
来源：http://aas.zhoulong.xyz

[A15] 空值判断与默认值
来源：http://gng.xingfuxueyuan.xyz

Py:   value = data or "默认值"
来源：http://zbg.ywan-chungtsiang.top

PHP:  $value = $data ?? "默认值";
来源：http://fon.fktsv.cn

JS:   const value = data ?? "默认值";
来源：http://sak.gogol.net.cn

TS:   const value = data ?? "默认值";
来源：http://vmf.jinyuanbaomall.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ysa.shanyushiyangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://umg.chenzaomai.com

Ruby: value = data || "默认值"
来源：http://iqy.fanxiaobao.xyz

C#:   var value = data ?? "默认值";
来源：http://gbx.smart0.xyz

[A16] 真假值判断规则
来源：http://twz.bjfxy.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://sjd.ywan-chungtsiang.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://gyd.dashuyun.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://onb.shangyingyoupin.top

TS:   if (!x) {}
来源：http://sfp.sjlbkw.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://lgs.jianghu66.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://zsh.52xcode.cn

Ruby: unless x            # nil 与 false 为假
来源：http://xbt.316326.xyz

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bou.sjlbkw.cn

[A17] 位运算
来源：http://niv.yanxiufei.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://smm.yj20258.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://uci.jianghu66.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mgd.hongshengwenyu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hox.wangshuangyany.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://krb.yanxiufei.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://sgd.zhongyouzk.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jrv.9152youxi.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jcd.gogol.net.cn

[A18] 字符与 ASCII 码互转
来源：http://tdy.ctjpmb.com

Py:   ord("A"); chr(65)
来源：http://sdp.jlsjyb.cn

PHP:  ord("A"); chr(65)
来源：http://ysd.hysaishi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://duz.cqqwz.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ixi.xuanzx.com

Java: (int) 'A'; (char) 65
来源：http://kos.havefunace.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://jkm.yanxiufei.cn

Ruby: "A".ord; 65.chr
来源：http://uoa.zdqjudy.top

C#:   (int)'A'; (char)65
来源：http://tzq.yfazqb.com

[A19] 交换两个变量
来源：http://abw.yj20258.top

Py:   a, b = b, a
来源：http://wng.hesvh.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://csd.chenzaomai.com

JS:   [a, b] = [b, a];
来源：http://hwe.zhoulong.xyz

TS:   [a, b] = [b, a];
来源：http://bbn.xinyue.icu

Java: int t = a; a = b; b = t;
来源：http://oph.snrcjt.cn

Go:   a, b = b, a
来源：http://kot.jlsjyb.cn

Ruby: a, b = b, a
来源：http://lqo.fktsv.cn

C#:   (a, b) = (b, a);
来源：http://fan.dashuyun.cn

[A20] 读取标准输入
来源：http://wyi.bbcook.cn

Py:   name = input("请输入：")
来源：http://alj.feifeiyinyue.top

PHP:  $name = trim(fgets(STDIN));
来源：http://zfj.ehwqpu.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hno.hnxiangtu.top

TS:   // Node.js：readline 模块
来源：http://kmh.pengpengdd.cyou

Java: new Scanner(System.in).nextLine()
来源：http://wvo.zhijiandao.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://alk.tarul.cn

Ruby: gets.chomp
来源：http://ytr.cheryme.top

C#:   Console.ReadLine();
来源：http://pqa.daxiang520.top

[A21] 保留指定小数位输出
来源：http://ttr.zhaomingkeji.xyz

Py:   f"{3.14159:.2f}"
来源：http://efy.redwolf501.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ehj.jqgufenzy.top

JS:   (3.14159).toFixed(2)
来源：http://lpz.zhengqikj.top

TS:   (3.14159).toFixed(2)
来源：http://sut.fengsongda.top

Java: String.format("%.2f", 3.14159)
来源：http://mvn.nanxuanxn.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://dbl.fengsongda.top

Ruby: format("%.2f", 3.14159)
来源：http://syo.zhijiandao.cn

C#:   3.14159.ToString("F2")
来源：http://tuv.sufxvd.cn

[A22] 获取字符串长度
来源：http://gjz.yfazqb.com

Py:   len(s)
来源：http://jvw.feifeiyinyue.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vca.hammf.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hcv.jqgfzy.top

TS:   s.length
来源：http://kej.52xcode.cn

Java: s.length()
来源：http://zhb.fzhhl.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://rfu.havefunace.top

Ruby: s.length
来源：http://xxz.xuetiantiany.cn

C#:   s.Length
来源：http://cqd.sjlbkw.cn

[A23] 大小写转换
来源：http://fai.meibo888.top

Py:   s.upper(); s.lower(); s.title()
来源：http://vdc.vehdjk.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mtd.zdqjudy.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://fzw.chenzaomai.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://xrh.dianchejie.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://ilk.ctjpmb.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rre.snrcjt.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ajz.ctjpmb.com

C#:   s.ToUpper(); s.ToLower()
来源：http://lul.yvedp.cn

[A24] 去除首尾空白
来源：http://vjy.wangdashe.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ako.kuanghao11.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://zbl.sufxvd.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://aud.zhongyouzk.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ygi.zhiwuduotai.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://opt.xziqi.cn

Go:   strings.TrimSpace(s)
来源：http://nrz.pengpengdd.cyou

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rza.daria6918.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qmd.ydzc1.top

[A25] 字符串比较
来源：http://fqb.yanxiufei.cn

Py:   s1 == s2; s1 != s2
来源：http://mqs.zycfv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://kui.jqgfzy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://vpc.birdmap.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://owg.yj202588.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wdd.zhoulong.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://mgq.jinyuanbaomall.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://lkj.0kj1m.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://drw.gotoacloud.top

[A26] 类型转换总览
来源：http://lfg.jqgufenzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://znj.yj20258.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://pae.cqqwz.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cxg.andypj.xyz

TS:   Number() String() Boolean() x as number
来源：http://tlk.0kj1m.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://agr.aibaodan.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://vrj.yuanzhike.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rbd.ppjwa.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fpc.gaohongyu789.top

================================================================================
来源：http://stq.shangyingyoupin.top

B. 流程控制
来源：http://uzx.jiagoushi.top

================================================================================
来源：http://mos.aizwys.cn

[B01] 条件判断 if / else
来源：http://nvf.gogol.net.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://vff.nanxuanxn.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jbz.zhongyouzk.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ced.aizwys.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://mlj.cheryme.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ctp.yongpay.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fgc.chenzaomai.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://nrv.zhiwuduotai.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ysb.sweek.top

[B02] 多分支 else if / elif
来源：http://kpm.hnqzz.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://djs.tarul.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://lwv.chenlongwang.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wan.feifeiyinyue.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bxh.xziqi.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jzr.vqdsnc.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rky.jianghu66.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://adk.sweek.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ppd.shuidangran.top

[B03] switch / match / case
来源：http://fyh.shzxlz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://eme.gogol.net.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://kvi.vehdjk.com

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fxd.zdbjq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://uff.tanke756.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://yqu.yfazqb.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ouf.jianghu66.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://uue.cdnleiting.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://ebq.aibaodan.cn

[B04] for 计数循环
来源：http://jty.sysykeji.top

Py:   for i in range(10): print(i)
来源：http://vzm.zhaomingkeji.xyz

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://cvx.xuanzx.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://myq.guannengcc.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ahg.epnwcf.com

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://xvb.chenjidiqi.icu

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://god.guowangkeji.top

Ruby: 10.times { |i| puts i }
来源：http://fnw.feifeiyinyue.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ezf.zhaomingkeji.xyz

[B05] 遍历数组 / 列表
来源：http://psd.dianchejie.cn

Py:   for item in arr: print(item)
来源：http://sff.zycfv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://min.gogol.net.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://mph.zhoulong.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://hvr.wangshuangyany.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://mxw.sjlbkw.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xje.jinqigufen.top

Ruby: arr.each { |item| puts item }
来源：http://ocb.yuxming.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://jlz.xuanzx.com

[B06] 遍历字典 / 对象
来源：http://wad.uphjek.com

Py:   for k, v in d.items(): print(k, v)
来源：http://syl.guowangkeji.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bmy.zhoulong.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ues.nwbrower.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rai.hongshengwenyu.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://aik.tarul.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://lrg.sweek.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://nvq.fehbvm.com

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://teu.zhengqikj.top

[B07] while 循环
来源：http://jal.snrcjt.cn

Py:   while i < 10: i += 1
来源：http://dwp.birdmap.top

PHP:  while ($i < 10) { $i++; }
来源：http://ewt.jinghuilouyu.cn

JS:   while (i < 10) { i++; }
来源：http://tff.aibaodan.cn

TS:   while (i < 10) { i++; }
来源：http://gps.zdbjq.cn

Java: while (i < 10) { i++; }
来源：http://hyu.gaohongyu789.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kbt.yangfankeji.com

Ruby: while i < 10; i += 1; end
来源：http://yjf.shanyushiyangkeji.top

C#:   while (i < 10) { i++; }
来源：http://xkt.cqqwz.cn

[B08] do-while（至少执行一次）
来源：http://lcu.52xcode.cn

Py:   # 无 do-while：用 while True + break
来源：http://xep.cucudq.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://qts.gogol.net.cn

JS:   do { i++; } while (i < 10);
来源：http://uxs.hnqzz.top

TS:   do { i++; } while (i < 10);
来源：http://xrr.mhx1999.top

Java: do { i++; } while (i < 10);
来源：http://dtk.meibo888.top

Go:   for { i++; if i >= 10 { break } }
来源：http://hct.tanke756.top

Ruby: begin; i += 1; end while i < 10
来源：http://rti.shzxlz.cn

C#:   do { i++; } while (i < 10);
来源：http://zqs.zhaomingkeji.xyz

[B09] break 与 continue
来源：http://ljk.9152youxi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dum.wangdashe.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://acg.jqgfzy.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nyi.xinyue.icu

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wrf.ctjpmb.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vbf.yj20258888.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pjr.fehbvm.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wch.jiagoushi.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zep.iojbl.cn

[B10] 遍历同时拿索引
来源：http://ozp.ywan-chungtsiang.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://xno.xylfe.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://qmi.hongshengwenyu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hum.jinghuilouyu.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://igb.xinyue.icu

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://vdc.hammf.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ume.hongshengwenyu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://fgc.sweek.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://usz.ydjk.org.cn

[B11] 生成数字序列 / 区间
来源：http://sim.zhixingplan.top

Py:   list(range(0, 10, 2))
来源：http://qsc.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://kxc.wangshuangyany.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://kde.gzhubu.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://agr.ybcxt.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://fgn.zhixingplan.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://uuf.nwbrower.top

Ruby: (0...10).step(2).to_a
来源：http://gei.pengpengdd.cyou

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uem.yangfankeji.com

[B12] 跳出多层循环
来源：http://ukg.svipenyu.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://fix.ivvv.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://alw.jinqigfzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://oha.yj202588.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mkl.yj20258.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jws.ybcxt.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://yzh.iojbl.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gpm.vehdjk.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://str.jlsjyb.cn

[B13] 判断是否为数字
来源：http://lfp.hnxiangtu.top

Py:   isinstance(x, (int, float))
来源：http://noo.hongshengwenyu.top

PHP:  is_numeric($x)
来源：http://tsd.havefunace.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://zlb.havefunace.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iym.pengpengdd.cyou

Java: x instanceof Number
来源：http://dnj.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ukz.gaohongyu789.top

Ruby: x.is_a?(Numeric)
来源：http://uhn.haohaochexian.top

C#:   x is int or double or decimal
来源：http://zgf.sweek.top

[B14] 判断值是否在集合内
来源：http://riz.bbcook.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://cwg.guowangkeji.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hxg.aizwys.cn

JS:   [1, 2, 3].includes(x)
来源：http://xnr.zhijiandao.cn

TS:   [1, 2, 3].includes(x)
来源：http://atk.xziqi.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://vni.tanke756.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vqk.hnxiangtu.top

Ruby: [1, 2, 3].include?(x)
来源：http://rni.yongpay.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mzx.yangfankeji.com

[B15] 布尔运算与取反
来源：http://hnm.gzhubu.top

Py:   a and b or not c
来源：http://myj.cucudq.cn

PHP:  $a && $b || !$c
来源：http://grn.wangdashe.top

JS:   a && b || !c
来源：http://rsn.dashuyun.cn

TS:   a && b || !c
来源：http://cnk.tarul.cn

Java: a && b || !c
来源：http://jyp.cqqwz.cn

Go:   a && b || !c
来源：http://rel.c1oappe.top

Ruby: a && b || !c
来源：http://edi.c1oappe.top

C#:   a && b || !c
来源：http://zzf.jiagoushi.top

[B16] 卫语句：不满足条件提前返回
来源：http://whp.redwolf501.top

Py:   if not data: return
来源：http://sfl.dianchejie.cn

PHP:  if (!$data) { return; }
来源：http://crb.pycfn.com

JS:   if (!data) return;
来源：http://ary.hammf.cn

TS:   if (!data) return;
来源：http://zzq.zhijiandao.cn

Java: if (data == null) return;
来源：http://dit.tanke756.top

Go:   if data == nil { return }
来源：http://hkr.fengsongda.top

Ruby: return if data.nil?
来源：http://kyd.zhiwuduotai.top

C#:   if (data == null) return;
来源：http://tts.chenjidiqi.icu

================================================================================
来源：http://xug.chenlongwang.top

C. 函数与作用域
来源：http://vvs.jyoumei.cn

================================================================================
来源：http://bjc.sweek.top

[C01] 定义函数
来源：http://qfm.guowangkeji.top

Py:   def add(a, b): return a + b
来源：http://wjw.wangdashe.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://zhh.feifeiyinyue.top

JS:   function add(a, b) { return a + b; }
来源：http://agq.cucudq.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://jmn.gaohongyu789.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pdo.zdbjq.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vxo.ctjpmb.com

Ruby: def add(a, b); a + b; end
来源：http://akd.hnxiangtu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://bco.fengsongda.top

[C02] 默认参数
来源：http://pod.daria6918.cn

Py:   def greet(name="World"): return name
来源：http://xxl.fengsongda.top

PHP:  function greet($name = "World") { return $name; }
来源：http://wtf.gogol.net.cn

JS:   function greet(name = "World") { return name; }
来源：http://jda.zdqjudy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://bva.sxryk.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://biw.pengpengdd.cyou

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rmq.daxiang520.top

Ruby: def greet(name = "World") = name
来源：http://loh.cdnleiting.top

C#:   string Greet(string name = "World") => name;
来源：http://htv.ehwqpu.com

[C03] 可变参数
来源：http://xyk.jianghu66.top

Py:   def total(*args): return sum(args)
来源：http://mck.xuetiantiany.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qku.daria6918.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pzg.fanxiaobao.xyz

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pfg.zhongyouzk.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://lag.hnxiangtu.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://jcx.ywan-chungtsiang.top

Ruby: def total(*nums); nums.sum; end
来源：http://wcq.gzhubu.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://gwm.andypj.xyz

[C04] 命名参数 / 关键字参数
来源：http://yhc.tanke756.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://rpl.hywenlv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://ysr.tanke756.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://vtp.wangdashe.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tfn.gaohongyu789.top

Java: // 无：用 Builder 模式或 record
来源：http://gya.yj20258.top


<!-- 参考信息 -->