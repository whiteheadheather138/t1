代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://inz.yongpay.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lix.iojbl.cn

TS:   if (!x) {}
来源：http://vxg.dianchejie.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://uqj.chenjidiqi.icu

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://skt.xingfuxueyuan.xyz

Ruby: unless x            # nil 与 false 为假
来源：http://njo.ctjpmb.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://sut.zhixingplan.top

[A17] 位运算
来源：http://cui.316326.xyz

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://klm.hammf.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mhb.fzhhl.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vow.fehbvm.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://egd.shuidangran.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sny.dianchejie.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://wpg.hongshengwenyu.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://bnf.jyoumei.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zop.sjlbkw.cn

[A18] 字符与 ASCII 码互转
来源：http://nag.jinghuilouyu.cn

Py:   ord("A"); chr(65)
来源：http://bqp.9152youxi.cn

PHP:  ord("A"); chr(65)
来源：http://cjs.c1oappe.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ixj.chenzaomai.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jdj.ctjpmb.com

Java: (int) 'A'; (char) 65
来源：http://gti.xuanzx.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nmc.tianlin.xyz

Ruby: "A".ord; 65.chr
来源：http://wsz.sysykeji.top

C#:   (int)'A'; (char)65
来源：http://usp.sweek.top

[A19] 交换两个变量
来源：http://olz.pengpengdd.cyou

Py:   a, b = b, a
来源：http://ylj.nwbrower.top

PHP:  [$a, $b] = [$b, $a];
来源：http://sjs.redwolf501.top

JS:   [a, b] = [b, a];
来源：http://ovu.gzhubu.top

TS:   [a, b] = [b, a];
来源：http://kbf.cheryme.top

Java: int t = a; a = b; b = t;
来源：http://wdr.cdnleiting.top

Go:   a, b = b, a
来源：http://gmd.xuetiantiany.cn

Ruby: a, b = b, a
来源：http://bry.nanxuanxn.top

C#:   (a, b) = (b, a);
来源：http://eww.epnwcf.com

[A20] 读取标准输入
来源：http://mtw.jlsjyb.cn

Py:   name = input("请输入：")
来源：http://dnl.fanxiaobao.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://and.nanxinkj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eaj.mhx1999.top

TS:   // Node.js：readline 模块
来源：http://anj.hesvh.cn

Java: new Scanner(System.in).nextLine()
来源：http://mkw.yfazqb.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hai.xuetiantiany.cn

Ruby: gets.chomp
来源：http://xpf.316326.xyz

C#:   Console.ReadLine();
来源：http://wjh.zdqjudy.top

[A21] 保留指定小数位输出
来源：http://rej.yvedp.cn

Py:   f"{3.14159:.2f}"
来源：http://ttw.xinyue.icu

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://gbw.wangshuangyany.cn

JS:   (3.14159).toFixed(2)
来源：http://bgk.dianchejie.cn

TS:   (3.14159).toFixed(2)
来源：http://vol.tianlin.xyz

Java: String.format("%.2f", 3.14159)
来源：http://dlp.iojbl.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://knv.dashuyun.cn

Ruby: format("%.2f", 3.14159)
来源：http://zjx.hfpthk.cn

C#:   3.14159.ToString("F2")
来源：http://gvl.zhixingplan.top

[A22] 获取字符串长度
来源：http://tag.cqqwz.cn

Py:   len(s)
来源：http://zzs.jqgufenzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://spv.gogol.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://xow.dashuyun.cn

TS:   s.length
来源：http://twz.zdbjq.cn

Java: s.length()
来源：http://eey.wangshuangyany.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hps.xuetiantiany.cn

Ruby: s.length
来源：http://avi.yj20258.top

C#:   s.Length
来源：http://yeq.0kj1m.cn

[A23] 大小写转换
来源：http://opo.xziqi.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://vxc.mhx1999.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ukf.wangdashe.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ywg.cucudq.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://epy.guowangkeji.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://prf.0kj1m.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://bgb.bjfxy.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hzd.shanyushiyangkeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://tiy.jinyuanbaomall.cn

[A24] 去除首尾空白
来源：http://ftd.nanxinkj.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mkn.zhaomingkeji.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://pxc.hnxiangtu.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sil.jqgufenzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ttq.zhixingplan.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gmi.fengsongda.top

Go:   strings.TrimSpace(s)
来源：http://xjy.jinqigufen.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://tqu.tian-w.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://nvb.tianlin.xyz

[A25] 字符串比较
来源：http://xwj.ehwqpu.com

Py:   s1 == s2; s1 != s2
来源：http://bmg.bjfxy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://urm.cqqwz.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hxx.zhongyouzk.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gxg.9152youxi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://amv.tian-w.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hnc.hnqzz.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kpp.fktsv.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://uze.chenjidiqi.icu

[A26] 类型转换总览
来源：http://deh.hammf.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://xiw.cucudq.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tao.andypj.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://ynd.gotoacloud.top

TS:   Number() String() Boolean() x as number
来源：http://zfi.jinghuilouyu.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://lvn.guowangkeji.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hca.chenjidiqi.icu

Ruby: to_i to_f to_s to_sym to_a
来源：http://ruz.epnwcf.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hoi.chenjidiqi.icu

================================================================================
来源：http://syh.ybcxt.top

B. 流程控制
来源：http://uhr.shangyingyoupin.top

================================================================================
来源：http://kol.gotoacloud.top

[B01] 条件判断 if / else
来源：http://ahu.jlsjyb.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://gfn.jlsjyb.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ogn.yj20258888.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://joc.sxryk.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://exd.xuanzx.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://zso.pycfn.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mnt.jlsjyb.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bwf.nanxinkj.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ydh.jiagoushi.top

[B02] 多分支 else if / elif
来源：http://ork.yanxiufei.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://tiy.sxryk.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vmh.cdnleiting.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ffq.iojbl.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://buj.mhx1999.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vzs.sufxvd.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xiw.bjfxy.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cei.zdbjq.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vdl.sysykeji.top

[B03] switch / match / case
来源：http://plq.yangfankeji.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://suy.sufxvd.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ezk.c1oappe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lxl.fengsongda.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mvp.zycfv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://rvr.yj202588.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wqi.sxryk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mvn.shangyingyoupin.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://jcw.vehdjk.com

[B04] for 计数循环
来源：http://bhm.zhiwuduotai.top

Py:   for i in range(10): print(i)
来源：http://rfc.chenlongwang.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://bhc.guowangkeji.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wfj.hammf.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://nns.tianlin.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wrk.fzhhl.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://iiu.meibo888.top

Ruby: 10.times { |i| puts i }
来源：http://rdw.hywenlv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://guc.smart0.xyz

[B05] 遍历数组 / 列表
来源：http://yen.guannengcc.top

Py:   for item in arr: print(item)
来源：http://rxc.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://tym.hywenlv.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://fai.9152youxi.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://xum.cqqwz.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://lgk.svipenyu.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bnb.chenlongwang.top

Ruby: arr.each { |item| puts item }
来源：http://noc.yongpay.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xyg.ppjwa.cn

[B06] 遍历字典 / 对象
来源：http://toc.meibo888.top

Py:   for k, v in d.items(): print(k, v)
来源：http://dxk.jyoumei.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://eox.yfazqb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://djs.sjlbkw.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://drz.zhixingplan.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://jvk.sxryk.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://gvj.aibaodan.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://eqe.bjfxy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://lxs.feifeiyinyue.top

[B07] while 循环
来源：http://vno.dianchejie.cn

Py:   while i < 10: i += 1
来源：http://shi.aibaodan.cn

PHP:  while ($i < 10) { $i++; }
来源：http://dyk.yueranfly.top

JS:   while (i < 10) { i++; }
来源：http://nah.haohaochexian.top

TS:   while (i < 10) { i++; }
来源：http://mod.wangshuangyany.cn

Java: while (i < 10) { i++; }
来源：http://vsq.cqqwz.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nnc.jqgufenzy.top

Ruby: while i < 10; i += 1; end
来源：http://hte.chenjidiqi.icu

C#:   while (i < 10) { i++; }
来源：http://ngs.shuidangran.top

[B08] do-while（至少执行一次）
来源：http://edv.sjlbkw.cn

Py:   # 无 do-while：用 while True + break
来源：http://tom.bjfxy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://fzd.hcnkem.com

JS:   do { i++; } while (i < 10);
来源：http://bux.ybcxt.top

TS:   do { i++; } while (i < 10);
来源：http://llv.shangyingyoupin.top

Java: do { i++; } while (i < 10);
来源：http://zli.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://lsa.zhongyouzk.top

Ruby: begin; i += 1; end while i < 10
来源：http://pbd.cucudq.cn

C#:   do { i++; } while (i < 10);
来源：http://rvs.haohaochexian.top

[B09] break 与 continue
来源：http://gof.jiagoushi.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://njj.zdbjq.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gho.yongpay.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qca.jinghuilouyu.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rbp.zdqjudy.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qtu.pycfn.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://pic.hnxiangtu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rym.jinqigfzy.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rmn.chenlongwang.top

[B10] 遍历同时拿索引
来源：http://unl.meibo888.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hdp.guannengcc.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://gjf.bjfxy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://pfj.yvedp.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://iju.haohaochexian.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://upf.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ixr.tian-w.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://utp.daxiang520.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ali.jqgufenzy.top

[B11] 生成数字序列 / 区间
来源：http://fzw.jinyuanbaomall.cn

Py:   list(range(0, 10, 2))
来源：http://xne.sweek.top

PHP:  range(0, 10, 2);
来源：http://rzu.ydjk.org.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ahs.yuanzhike.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ayj.yuanzhike.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rjf.zhaomingkeji.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kmg.fktsv.cn

Ruby: (0...10).step(2).to_a
来源：http://xsh.cashguo.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://bhl.fengsongda.top

[B12] 跳出多层循环
来源：http://nsy.shangyingyoupin.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://rmd.shuidangran.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://txr.zdbjq.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://uik.tanke756.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rso.guannengcc.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jca.xinyue.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://gvs.andypj.xyz

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://tdu.yj202588.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://azj.sxryk.cn

[B13] 判断是否为数字
来源：http://wok.zhaomingkeji.xyz

Py:   isinstance(x, (int, float))
来源：http://jrm.hnqzz.top

PHP:  is_numeric($x)
来源：http://mxk.yuxming.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://rru.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lrr.zhengqikj.top

Java: x instanceof Number
来源：http://aiv.xuetiantiany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qqo.jinyuanbaomall.cn

Ruby: x.is_a?(Numeric)
来源：http://jkk.sufxvd.cn

C#:   x is int or double or decimal
来源：http://ofw.hysaishi.cn

[B14] 判断值是否在集合内
来源：http://gqt.xylfe.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mtw.mhx1999.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://yvy.zdqjudy.top

JS:   [1, 2, 3].includes(x)
来源：http://wnw.ydzc1.top

TS:   [1, 2, 3].includes(x)
来源：http://oek.fktsv.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://jdm.vqdsnc.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://dbz.daxiang520.top

Ruby: [1, 2, 3].include?(x)
来源：http://zjk.bbcook.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ogm.yanxiufei.cn

[B15] 布尔运算与取反
来源：http://pol.iojbl.cn

Py:   a and b or not c
来源：http://khg.jqgufenzy.top

PHP:  $a && $b || !$c
来源：http://tul.fktsv.cn

JS:   a && b || !c
来源：http://vbw.aizwys.cn

TS:   a && b || !c
来源：http://wqa.fengsongda.top

Java: a && b || !c
来源：http://qap.meibo888.top

Go:   a && b || !c
来源：http://isb.sxryk.cn

Ruby: a && b || !c
来源：http://abd.sxryk.cn

C#:   a && b || !c
来源：http://tcg.redwolf501.top

[B16] 卫语句：不满足条件提前返回
来源：http://xuv.jyoumei.cn

Py:   if not data: return
来源：http://wlj.316326.xyz

PHP:  if (!$data) { return; }
来源：http://ckm.tarul.cn

JS:   if (!data) return;
来源：http://yvy.snrcjt.cn

TS:   if (!data) return;
来源：http://uat.redwolf501.top

Java: if (data == null) return;
来源：http://xat.xylfe.cn

Go:   if data == nil { return }
来源：http://efb.pycfn.com

Ruby: return if data.nil?
来源：http://uhd.ehwqpu.com

C#:   if (data == null) return;
来源：http://ecu.zhaomingkeji.xyz

================================================================================
来源：http://fey.zhijiandao.cn

C. 函数与作用域
来源：http://vgd.9152youxi.cn

================================================================================
来源：http://doi.kuanghao11.cn

[C01] 定义函数
来源：http://ong.hfpthk.cn

Py:   def add(a, b): return a + b
来源：http://atv.fengsongda.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tyb.cucudq.cn

JS:   function add(a, b) { return a + b; }
来源：http://usz.pycfn.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ews.dashuyun.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://zly.bbcook.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ldr.daxiang520.top

Ruby: def add(a, b); a + b; end
来源：http://luq.ppjwa.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://ccg.yuanzhike.top

[C02] 默认参数
来源：http://zac.cdnleiting.top

Py:   def greet(name="World"): return name
来源：http://skc.smart0.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://coh.iojbl.cn

JS:   function greet(name = "World") { return name; }
来源：http://djb.yfazqb.com

TS:   function greet(name: string = "World") { return name; }
来源：http://dgl.chenjidiqi.icu

Java: // 无默认参数：方法重载或 Optional
来源：http://onp.chenlongwang.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ulc.zycfv.cn

Ruby: def greet(name = "World") = name
来源：http://auy.zhijiandao.cn

C#:   string Greet(string name = "World") => name;
来源：http://yps.tian-w.cn

[C03] 可变参数
来源：http://vch.xinyue.icu

Py:   def total(*args): return sum(args)
来源：http://gjo.nanxinkj.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://zxp.yj20258.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://ask.gzhubu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xrf.xylfe.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ngo.zhijiandao.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://egy.zhoulong.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://mzf.tarul.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://png.yuanzhike.top

[C04] 命名参数 / 关键字参数
来源：http://zhw.iojbl.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://bcw.xziqi.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://gnj.hongshengwenyu.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://syr.ydjk.org.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jfm.hesvh.cn

Java: // 无：用 Builder 模式或 record
来源：http://jcq.ywan-chungtsiang.top

Go:   // 无：用配置结构体参数
来源：http://zgg.meibo888.top

Ruby: f(a: 1, b: 2)
来源：http://oih.xylfe.cn

C#:   f(a: 1, b: 2)
来源：http://xse.ydjk.org.cn

[C05] 返回多个值
来源：http://vyy.hnxiangtu.top

Py:   return a, b
来源：http://tye.jqgufenzy.top

PHP:  return [$a, $b];
来源：http://tce.mhx1999.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://mip.fehbvm.com

TS:   return { a, b };
来源：http://xzl.guowangkeji.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://gqs.yueranfly.top

Go:   return a, b
来源：http://mkm.zhongyouzk.top

Ruby: return a, b
来源：http://xsd.tarul.cn

C#:   return (a, b);              // ValueTuple
来源：http://wfi.xylfe.cn

[C06] 匿名函数 / lambda
来源：http://aza.gzhubu.top

Py:   square = lambda x: x * x
来源：http://ymo.fehbvm.com

PHP:  $square = fn($x) => $x * $x;
来源：http://fwh.shanyushiyangkeji.top

JS:   const square = x => x * x;
来源：http://llt.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://nau.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jmx.ivvv.top

Go:   sq := func(x int) int { return x * x }
来源：http://tvy.fktsv.cn

Ruby: square = ->(x) { x * x }
来源：http://zzy.ehwqpu.com


<!-- 参考信息 -->