代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://qaz.iojbl.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://tqk.shuidangran.top

TS:   if (!x) {}
来源：http://hdk.pycfn.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://pxc.havefunace.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lsv.ppjwa.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vza.snrcjt.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://oht.wangshuangyany.cn

[A17] 位运算
来源：http://rgb.jqgfzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://jyn.meibo888.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xqf.fanxiaobao.xyz

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://qtk.yongpay.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://omj.tian-w.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://okt.daria6918.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ugc.yuanzhike.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://viu.birdmap.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lnl.xuetiantiany.cn

[A18] 字符与 ASCII 码互转
来源：http://ejq.chenjidiqi.icu

Py:   ord("A"); chr(65)
来源：http://hdx.chenzaomai.com

PHP:  ord("A"); chr(65)
来源：http://nql.0kj1m.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xjw.sjlbkw.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mmm.zdqjudy.top

Java: (int) 'A'; (char) 65
来源：http://bmd.0kj1m.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://bpy.vehdjk.com

Ruby: "A".ord; 65.chr
来源：http://ogu.gzhubu.top

C#:   (int)'A'; (char)65
来源：http://xig.316326.xyz

[A19] 交换两个变量
来源：http://vba.jinqigfzy.top

Py:   a, b = b, a
来源：http://jjl.fktsv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ylp.zycfv.cn

JS:   [a, b] = [b, a];
来源：http://owe.pycfn.com

TS:   [a, b] = [b, a];
来源：http://ujb.hysaishi.cn

Java: int t = a; a = b; b = t;
来源：http://fkx.mhx1999.top

Go:   a, b = b, a
来源：http://vrx.smart0.xyz

Ruby: a, b = b, a
来源：http://fjp.yuxming.cn

C#:   (a, b) = (b, a);
来源：http://ecs.sweek.top

[A20] 读取标准输入
来源：http://ezl.snrcjt.cn

Py:   name = input("请输入：")
来源：http://knv.birdmap.top

PHP:  $name = trim(fgets(STDIN));
来源：http://efi.nwbrower.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://xxc.vehdjk.com

TS:   // Node.js：readline 模块
来源：http://all.dashuyun.cn

Java: new Scanner(System.in).nextLine()
来源：http://ggi.cashguo.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qdm.316326.xyz

Ruby: gets.chomp
来源：http://nok.sweek.top

C#:   Console.ReadLine();
来源：http://jrz.kuanghao11.cn

[A21] 保留指定小数位输出
来源：http://yxq.gaohongyu789.top

Py:   f"{3.14159:.2f}"
来源：http://lxi.jinyuanbaomall.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zku.meibo888.top

JS:   (3.14159).toFixed(2)
来源：http://gcr.pycfn.com

TS:   (3.14159).toFixed(2)
来源：http://bvb.fehbvm.com

Java: String.format("%.2f", 3.14159)
来源：http://jhi.birdmap.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wir.cashguo.top

Ruby: format("%.2f", 3.14159)
来源：http://wov.hcnkem.com

C#:   3.14159.ToString("F2")
来源：http://sel.fengsongda.top

[A22] 获取字符串长度
来源：http://tid.jianghu66.top

Py:   len(s)
来源：http://guf.zhoulong.xyz

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://qzy.pycfn.com

JS:   s.length                          # 按 UTF-16 单元计
来源：http://izn.shangyingyoupin.top

TS:   s.length
来源：http://osx.hongshengwenyu.top

Java: s.length()
来源：http://jey.epnwcf.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://nkt.hfpthk.cn

Ruby: s.length
来源：http://hpc.316326.xyz

C#:   s.Length
来源：http://kjl.xuetiantiany.cn

[A23] 大小写转换
来源：http://bym.uphjek.com

Py:   s.upper(); s.lower(); s.title()
来源：http://nie.tanke756.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vus.xinyue.icu

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xmc.pycfn.com

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cmd.hcnkem.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://zek.yvedp.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://iwh.ywan-chungtsiang.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ttz.yuxming.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://dhp.birdmap.top

[A24] 去除首尾空白
来源：http://ujl.quarkkingdee.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nzg.sjlbkw.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://bja.uphjek.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://kgo.yj20258888.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dgf.jinghuilouyu.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bmr.redwolf501.top

Go:   strings.TrimSpace(s)
来源：http://xjp.ehwqpu.com

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://xxn.jqgufenzy.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://byb.52xcode.cn

[A25] 字符串比较
来源：http://eor.52xcode.cn

Py:   s1 == s2; s1 != s2
来源：http://pxv.jinghuilouyu.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://sif.shanyushiyangkeji.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://yug.guannengcc.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://nxi.jinqigfzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://yvo.sweek.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cpz.zhengqikj.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kgv.iojbl.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nhj.jinyuanbaomall.cn

[A26] 类型转换总览
来源：http://vrh.iojbl.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://zdm.jlsjyb.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://tky.mhx1999.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://aii.zhengqikj.top

TS:   Number() String() Boolean() x as number
来源：http://erv.zdqjudy.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://rqz.hnxiangtu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rxd.shangyingyoupin.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://tbi.52xcode.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://tvo.fehbvm.com

================================================================================
来源：http://jwv.cdnleiting.top

B. 流程控制
来源：http://fev.hesvh.cn

================================================================================
来源：http://xuu.birdmap.top

[B01] 条件判断 if / else
来源：http://kxi.shzxlz.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://oyd.svipenyu.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hby.birdmap.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jzx.hcnkem.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://rxw.daxiang520.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://qwc.hysaishi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://iwp.zdqjudy.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vzi.gotoacloud.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://dmx.xingfuxueyuan.xyz

[B02] 多分支 else if / elif
来源：http://qei.andypj.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://lvz.jqgfzy.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://und.hfpthk.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zpd.yj20258.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fdm.havefunace.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sll.wangshuangyany.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://yul.xuanzx.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://uut.ppjwa.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ofg.havefunace.top

[B03] switch / match / case
来源：http://jda.zhijiandao.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rzk.nwbrower.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://xph.cashguo.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sni.zdbjq.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eek.fktsv.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://jlp.guannengcc.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://dnd.haohaochexian.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://vnd.dashuyun.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zfn.pycfn.com

[B04] for 计数循环
来源：http://qxi.hywenlv.cn

Py:   for i in range(10): print(i)
来源：http://twx.xinyue.icu

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://lek.nanxuanxn.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xco.ivvv.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yhf.c1oappe.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pig.kuanghao11.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://lnx.smart0.xyz

Ruby: 10.times { |i| puts i }
来源：http://zlk.hesvh.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fjt.zhixingplan.top

[B05] 遍历数组 / 列表
来源：http://hjg.hammf.cn

Py:   for item in arr: print(item)
来源：http://fwc.jinqigfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ewq.uphjek.com

JS:   for (const item of arr) { console.log(item); }
来源：http://low.shzxlz.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://exb.yfazqb.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://nqi.fanxiaobao.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zrw.aizwys.cn

Ruby: arr.each { |item| puts item }
来源：http://qox.jqgfzy.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://ydv.ivvv.top

[B06] 遍历字典 / 对象
来源：http://tzz.xuetiantiany.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://uwo.fengsongda.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://yhb.vqdsnc.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://tqq.fengsongda.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://prz.wangshuangyany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://yqx.zycfv.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://kjg.bbcook.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://arv.cqqwz.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bkf.chenlongwang.top

[B07] while 循环
来源：http://uim.vqdsnc.cn

Py:   while i < 10: i += 1
来源：http://wvp.fengsongda.top

PHP:  while ($i < 10) { $i++; }
来源：http://uiu.xuanzx.com

JS:   while (i < 10) { i++; }
来源：http://lgt.hammf.cn

TS:   while (i < 10) { i++; }
来源：http://lfw.yanxiufei.cn

Java: while (i < 10) { i++; }
来源：http://bru.52xcode.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://yyn.cashguo.top

Ruby: while i < 10; i += 1; end
来源：http://bil.ywan-chungtsiang.top

C#:   while (i < 10) { i++; }
来源：http://pak.zhaomingkeji.xyz

[B08] do-while（至少执行一次）
来源：http://yxu.gzhubu.top

Py:   # 无 do-while：用 while True + break
来源：http://keu.xuetiantiany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://bge.jianghu66.top

JS:   do { i++; } while (i < 10);
来源：http://nti.pycfn.com

TS:   do { i++; } while (i < 10);
来源：http://lcn.yonumen.top

Java: do { i++; } while (i < 10);
来源：http://ejl.redwolf501.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nuj.zhiwuduotai.top

Ruby: begin; i += 1; end while i < 10
来源：http://ott.bjfxy.top

C#:   do { i++; } while (i < 10);
来源：http://fpe.daria6918.cn

[B09] break 与 continue
来源：http://bcm.haohaochexian.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://xwl.jinyuanbaomall.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://nqx.cdnleiting.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mrs.xziqi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nry.nwbrower.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tvj.yangfankeji.com

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xra.kuanghao11.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://zpg.gzhubu.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://grh.yvedp.cn

[B10] 遍历同时拿索引
来源：http://ahj.jiagoushi.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://sym.gotoacloud.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://eiv.wangshuangyany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://azg.fehbvm.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fsn.zhaomingkeji.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ltj.yonumen.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://cdk.fzhhl.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://sep.nwbrower.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://sly.mhx1999.top

[B11] 生成数字序列 / 区间
来源：http://jys.dianchejie.cn

Py:   list(range(0, 10, 2))
来源：http://cil.jlsjyb.cn

PHP:  range(0, 10, 2);
来源：http://mqz.yueranfly.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ydb.dianchejie.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://xzr.bbcook.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://gtx.cucudq.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://cpo.zdbjq.cn

Ruby: (0...10).step(2).to_a
来源：http://iqu.zhaomingkeji.xyz

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://its.xingfuxueyuan.xyz

[B12] 跳出多层循环
来源：http://rst.wangdashe.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://gad.sufxvd.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://tvv.zdqjudy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://dbe.tian-w.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://jaj.nanxuanxn.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ife.wangdashe.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cvz.nanxinkj.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://jwh.wangshuangyany.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wys.snrcjt.cn

[B13] 判断是否为数字
来源：http://xaz.hesvh.cn

Py:   isinstance(x, (int, float))
来源：http://cjr.zhoulong.xyz

PHP:  is_numeric($x)
来源：http://vec.yj20258.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vlo.tian-w.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hyf.fengsongda.top

Java: x instanceof Number
来源：http://tth.yj20258.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://wbr.52xcode.cn

Ruby: x.is_a?(Numeric)
来源：http://cwc.yj20258.top

C#:   x is int or double or decimal
来源：http://fii.quarkkingdee.top

[B14] 判断值是否在集合内
来源：http://vgi.jqgfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://qqf.hesvh.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lop.daria6918.cn

JS:   [1, 2, 3].includes(x)
来源：http://lwa.iojbl.cn

TS:   [1, 2, 3].includes(x)
来源：http://yvd.jianghu66.top

Java: List.of(1, 2, 3).contains(x)
来源：http://buo.c1oappe.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://evm.yanxiufei.cn

Ruby: [1, 2, 3].include?(x)
来源：http://iru.zdqjudy.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ibv.zhongyouzk.top

[B15] 布尔运算与取反
来源：http://oos.ydjk.org.cn

Py:   a and b or not c
来源：http://afg.bbcook.cn

PHP:  $a && $b || !$c
来源：http://poo.zhijiandao.cn

JS:   a && b || !c
来源：http://nni.c1oappe.top

TS:   a && b || !c
来源：http://fmn.yangfankeji.com

Java: a && b || !c
来源：http://aum.dianchejie.cn

Go:   a && b || !c
来源：http://kpe.ctjpmb.com

Ruby: a && b || !c
来源：http://doh.hcnkem.com

C#:   a && b || !c
来源：http://ikg.haohaochexian.top

[B16] 卫语句：不满足条件提前返回
来源：http://zcp.iojbl.cn

Py:   if not data: return
来源：http://ixv.tian-w.cn

PHP:  if (!$data) { return; }
来源：http://ivk.yangfankeji.com

JS:   if (!data) return;
来源：http://edf.iojbl.cn

TS:   if (!data) return;
来源：http://sno.ybcxt.top

Java: if (data == null) return;
来源：http://wrc.daria6918.cn

Go:   if data == nil { return }
来源：http://ibj.chenjidiqi.icu

Ruby: return if data.nil?
来源：http://zay.yfazqb.com

C#:   if (data == null) return;
来源：http://xft.shangyingyoupin.top

================================================================================
来源：http://oem.fehbvm.com

C. 函数与作用域
来源：http://pes.epnwcf.com

================================================================================
来源：http://ktd.nanxuanxn.top

[C01] 定义函数
来源：http://ftw.yuxming.cn

Py:   def add(a, b): return a + b
来源：http://bdh.kuanghao11.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wyl.snrcjt.cn

JS:   function add(a, b) { return a + b; }
来源：http://kgi.aizwys.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xgh.52xcode.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://mtq.andypj.xyz

Go:   func add(a, b int) int { return a + b }
来源：http://yai.nanxuanxn.top

Ruby: def add(a, b); a + b; end
来源：http://tld.fktsv.cn

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yom.nanxuanxn.top

[C02] 默认参数
来源：http://vsu.gzhubu.top

Py:   def greet(name="World"): return name
来源：http://uqi.hongshengwenyu.top

PHP:  function greet($name = "World") { return $name; }
来源：http://pej.zhengqikj.top

JS:   function greet(name = "World") { return name; }
来源：http://phf.gaohongyu789.top

TS:   function greet(name: string = "World") { return name; }
来源：http://czl.316326.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://rwy.uphjek.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://brv.yueranfly.top

Ruby: def greet(name = "World") = name
来源：http://tgz.ctjpmb.com

C#:   string Greet(string name = "World") => name;
来源：http://wyz.vehdjk.com

[C03] 可变参数
来源：http://txp.fehbvm.com

Py:   def total(*args): return sum(args)
来源：http://qob.xylfe.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://sfs.tarul.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hce.gzhubu.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://myq.ydzc1.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://tos.sxryk.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://tna.ppjwa.cn

Ruby: def total(*nums); nums.sum; end
来源：http://hrf.cheryme.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://pll.xylfe.cn

[C04] 命名参数 / 关键字参数
来源：http://yoj.nanxinkj.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://koo.zhixingplan.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://auu.ppjwa.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jrh.daxiang520.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://sqh.yonumen.top

Java: // 无：用 Builder 模式或 record
来源：http://bwq.xinyue.icu

Go:   // 无：用配置结构体参数
来源：http://ctu.zhoulong.xyz

Ruby: f(a: 1, b: 2)
来源：http://lwz.hongshengwenyu.top

C#:   f(a: 1, b: 2)
来源：http://vtg.vehdjk.com

[C05] 返回多个值
来源：http://knf.birdmap.top

Py:   return a, b
来源：http://ine.shangyingyoupin.top

PHP:  return [$a, $b];
来源：http://jrd.ydzc1.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://crk.gzhubu.top

TS:   return { a, b };
来源：http://wfx.tianlin.xyz

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://aex.hongshengwenyu.top

Go:   return a, b
来源：http://mej.chenlongwang.top

Ruby: return a, b
来源：http://zuz.chenzaomai.com

C#:   return (a, b);              // ValueTuple
来源：http://nsd.gogol.net.cn

[C06] 匿名函数 / lambda
来源：http://kyu.havefunace.top

Py:   square = lambda x: x * x
来源：http://wyr.ywan-chungtsiang.top

PHP:  $square = fn($x) => $x * $x;
来源：http://fdz.nanxinkj.top

JS:   const square = x => x * x;
来源：http://yiu.fehbvm.com

TS:   const square = (x: number): number => x * x;
来源：http://phl.yuanzhike.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://pyq.quarkkingdee.top

Go:   sq := func(x int) int { return x * x }
来源：http://ulr.sjlbkw.cn

Ruby: square = ->(x) { x * x }
来源：http://tzp.fengsongda.top


<!-- 参考信息 -->