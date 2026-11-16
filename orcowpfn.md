代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oes.gzhubu.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://pgi.pycfn.com

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ngz.guannengcc.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://iqh.chenzaomai.com

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wnf.zhixingplan.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://fjp.ivvv.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://iac.52xcode.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yed.cheryme.top

[A18] 字符与 ASCII 码互转
来源：http://fyi.cqqwz.cn

Py:   ord("A"); chr(65)
来源：http://xem.zhongyouzk.top

PHP:  ord("A"); chr(65)
来源：http://nzl.sweek.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mvu.jinghuilouyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tey.ybcxt.top

Java: (int) 'A'; (char) 65
来源：http://nqr.zhaomingkeji.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://nuy.ppjwa.cn

Ruby: "A".ord; 65.chr
来源：http://dpv.jqgufenzy.top

C#:   (int)'A'; (char)65
来源：http://ktb.chenlongwang.top

[A19] 交换两个变量
来源：http://icl.zhongyouzk.top

Py:   a, b = b, a
来源：http://tub.0kj1m.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://mqh.daxiang520.top

JS:   [a, b] = [b, a];
来源：http://vda.svipenyu.cn

TS:   [a, b] = [b, a];
来源：http://heu.9152youxi.cn

Java: int t = a; a = b; b = t;
来源：http://rcr.jlsjyb.cn

Go:   a, b = b, a
来源：http://pnu.hnxiangtu.top

Ruby: a, b = b, a
来源：http://tsg.0kj1m.cn

C#:   (a, b) = (b, a);
来源：http://oqr.zhongyouzk.top

[A20] 读取标准输入
来源：http://qxg.yvedp.cn

Py:   name = input("请输入：")
来源：http://heq.yueranfly.top

PHP:  $name = trim(fgets(STDIN));
来源：http://vbk.xuanzx.com

JS:   // Node.js：readline 模块或 process.stdin
来源：http://dzy.zhoulong.xyz

TS:   // Node.js：readline 模块
来源：http://owg.ehwqpu.com

Java: new Scanner(System.in).nextLine()
来源：http://awz.jqgufenzy.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://umi.cqqwz.cn

Ruby: gets.chomp
来源：http://htl.zhixingplan.top

C#:   Console.ReadLine();
来源：http://owp.bbcook.cn

[A21] 保留指定小数位输出
来源：http://elz.shangyingyoupin.top

Py:   f"{3.14159:.2f}"
来源：http://uep.hammf.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://rya.svipenyu.cn

JS:   (3.14159).toFixed(2)
来源：http://mss.hongshengwenyu.top

TS:   (3.14159).toFixed(2)
来源：http://uqc.aizwys.cn

Java: String.format("%.2f", 3.14159)
来源：http://msg.zhiwuduotai.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://mkl.hcnkem.com

Ruby: format("%.2f", 3.14159)
来源：http://fwc.gaohongyu789.top

C#:   3.14159.ToString("F2")
来源：http://daa.epnwcf.com

[A22] 获取字符串长度
来源：http://bnu.zhixingplan.top

Py:   len(s)
来源：http://iri.fzhhl.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ruj.ybcxt.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yws.nanxinkj.top

TS:   s.length
来源：http://hvm.fanxiaobao.xyz

Java: s.length()
来源：http://wqc.hysaishi.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oee.dashuyun.cn

Ruby: s.length
来源：http://uqx.zhongyouzk.top

C#:   s.Length
来源：http://lax.nanxinkj.top

[A23] 大小写转换
来源：http://qal.xuetiantiany.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://fjs.shanyushiyangkeji.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ocq.sjlbkw.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://qqu.yonumen.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://uwg.nanxuanxn.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://raa.meibo888.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hwh.yuxming.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://obl.yuanzhike.top

C#:   s.ToUpper(); s.ToLower()
来源：http://uka.316326.xyz

[A24] 去除首尾空白
来源：http://jjh.sweek.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://tuy.sysykeji.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://cxe.ydjk.org.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ehe.tian-w.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wje.jinyuanbaomall.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://aan.sjlbkw.cn

Go:   strings.TrimSpace(s)
来源：http://fok.kuanghao11.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://swz.jinghuilouyu.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://zdf.cashguo.top

[A25] 字符串比较
来源：http://sqj.zdqjudy.top

Py:   s1 == s2; s1 != s2
来源：http://wsx.epnwcf.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tfh.fzhhl.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://tdn.9152youxi.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://fgr.yuxming.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lxt.tian-w.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://huh.quarkkingdee.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ssb.tianlin.xyz

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zcr.chenlongwang.top

[A26] 类型转换总览
来源：http://nye.hammf.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://jvs.hfpthk.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://icp.zdqjudy.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://knr.yanxiufei.cn

TS:   Number() String() Boolean() x as number
来源：http://nsy.hysaishi.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://tqk.sjlbkw.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mkv.pengpengdd.cyou

Ruby: to_i to_f to_s to_sym to_a
来源：http://klk.hnqzz.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://uid.tian-w.cn

================================================================================
来源：http://xrb.zdbjq.cn

B. 流程控制
来源：http://yaq.jqgufenzy.top

================================================================================
来源：http://tjd.cashguo.top

[B01] 条件判断 if / else
来源：http://ecx.wangshuangyany.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://bey.cashguo.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://dhe.xylfe.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://ole.0kj1m.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pea.gotoacloud.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dkh.hnqzz.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fok.zhoulong.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://fgi.vqdsnc.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://cgz.aibaodan.cn

[B02] 多分支 else if / elif
来源：http://csp.andypj.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vae.xingfuxueyuan.xyz

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://zwj.ctjpmb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ypl.0kj1m.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dsd.bbcook.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jex.zhiwuduotai.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://bhz.wangshuangyany.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://meu.jinqigfzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gsp.ppjwa.cn

[B03] switch / match / case
来源：http://qdz.jqgufenzy.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://vgr.xuetiantiany.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oov.c1oappe.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://krg.bjfxy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://nbb.guannengcc.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://fjq.ywan-chungtsiang.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://xyw.hfpthk.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://zdj.pengpengdd.cyou

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iqs.yuanzhike.top

[B04] for 计数循环
来源：http://syi.sysykeji.top

Py:   for i in range(10): print(i)
来源：http://hgu.tian-w.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hat.chenjidiqi.icu

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zbe.jinqigufen.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ahg.yonumen.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bje.ivvv.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://fwq.yueranfly.top

Ruby: 10.times { |i| puts i }
来源：http://yxc.fzhhl.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blw.mhx1999.top

[B05] 遍历数组 / 列表
来源：http://asv.yj202588.top

Py:   for item in arr: print(item)
来源：http://nwo.zhaomingkeji.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://qrr.hnxiangtu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nvr.fengsongda.top

TS:   for (const item of arr) { console.log(item); }
来源：http://vtk.vqdsnc.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://sof.tarul.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://gve.c1oappe.top

Ruby: arr.each { |item| puts item }
来源：http://fiu.yfazqb.com

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://fup.tarul.cn

[B06] 遍历字典 / 对象
来源：http://hgb.xuanzx.com

Py:   for k, v in d.items(): print(k, v)
来源：http://sbl.hammf.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://oxc.xuetiantiany.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wzy.yonumen.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://knq.hywenlv.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://lsf.cashguo.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://saj.aizwys.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ybt.ybcxt.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xlr.yonumen.top

[B07] while 循环
来源：http://poo.wangshuangyany.cn

Py:   while i < 10: i += 1
来源：http://ltw.nwbrower.top

PHP:  while ($i < 10) { $i++; }
来源：http://mkk.c1oappe.top

JS:   while (i < 10) { i++; }
来源：http://eog.cashguo.top

TS:   while (i < 10) { i++; }
来源：http://trw.gotoacloud.top

Java: while (i < 10) { i++; }
来源：http://ugv.mhx1999.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://xbq.vqdsnc.cn

Ruby: while i < 10; i += 1; end
来源：http://wwi.hammf.cn

C#:   while (i < 10) { i++; }
来源：http://tnj.snrcjt.cn

[B08] do-while（至少执行一次）
来源：http://wwp.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://yrl.dianchejie.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://wvw.wangshuangyany.cn

JS:   do { i++; } while (i < 10);
来源：http://zao.zhaomingkeji.xyz

TS:   do { i++; } while (i < 10);
来源：http://ufs.yj20258.top

Java: do { i++; } while (i < 10);
来源：http://ifc.zhongyouzk.top

Go:   for { i++; if i >= 10 { break } }
来源：http://xws.snrcjt.cn

Ruby: begin; i += 1; end while i < 10
来源：http://qqu.redwolf501.top

C#:   do { i++; } while (i < 10);
来源：http://qlu.aizwys.cn

[B09] break 与 continue
来源：http://wan.guannengcc.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dax.cheryme.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://shw.xylfe.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tjy.bbcook.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gub.hfpthk.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cdr.daxiang520.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://ypx.sysykeji.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://gao.chenzaomai.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://osr.daxiang520.top

[B10] 遍历同时拿索引
来源：http://azo.xinyue.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://pde.shzxlz.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ylp.xingfuxueyuan.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://yip.tianlin.xyz

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://cqd.zhongyouzk.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lgp.yuanzhike.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ujr.epnwcf.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://vug.cdnleiting.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://bru.haohaochexian.top

[B11] 生成数字序列 / 区间
来源：http://wbl.guowangkeji.top

Py:   list(range(0, 10, 2))
来源：http://rcf.tarul.cn

PHP:  range(0, 10, 2);
来源：http://gmy.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ikx.cashguo.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tuy.fanxiaobao.xyz

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ous.yvedp.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://kkm.ehwqpu.com

Ruby: (0...10).step(2).to_a
来源：http://rjy.aibaodan.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://uid.zdbjq.cn

[B12] 跳出多层循环
来源：http://ach.ivvv.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://lwz.fanxiaobao.xyz

PHP:  # 无标签：用 goto 或函数返回
来源：http://tvj.yanxiufei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ngu.fktsv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://whn.cdnleiting.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ztz.zhijiandao.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://qzn.quarkkingdee.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://uyn.jlsjyb.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://umc.zhaomingkeji.xyz

[B13] 判断是否为数字
来源：http://snu.gogol.net.cn

Py:   isinstance(x, (int, float))
来源：http://czm.havefunace.top

PHP:  is_numeric($x)
来源：http://hhz.hnxiangtu.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nzo.ppjwa.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://uey.yonumen.top

Java: x instanceof Number
来源：http://twu.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qtc.smart0.xyz

Ruby: x.is_a?(Numeric)
来源：http://bqd.nwbrower.top

C#:   x is int or double or decimal
来源：http://aqx.gogol.net.cn

[B14] 判断值是否在集合内
来源：http://qbt.svipenyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://reo.gotoacloud.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://oom.zhengqikj.top

JS:   [1, 2, 3].includes(x)
来源：http://ihk.jqgfzy.top

TS:   [1, 2, 3].includes(x)
来源：http://vpn.yongpay.top

Java: List.of(1, 2, 3).contains(x)
来源：http://euq.vqdsnc.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://tjm.yangfankeji.com

Ruby: [1, 2, 3].include?(x)
来源：http://kvr.sjlbkw.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://nam.sweek.top

[B15] 布尔运算与取反
来源：http://hcq.smart0.xyz

Py:   a and b or not c
来源：http://cnt.meibo888.top

PHP:  $a && $b || !$c
来源：http://evd.fanxiaobao.xyz

JS:   a && b || !c
来源：http://lrs.sysykeji.top

TS:   a && b || !c
来源：http://con.jqgfzy.top

Java: a && b || !c
来源：http://vsw.wangshuangyany.cn

Go:   a && b || !c
来源：http://xzb.cucudq.cn

Ruby: a && b || !c
来源：http://wgh.0kj1m.cn

C#:   a && b || !c
来源：http://him.gogol.net.cn

[B16] 卫语句：不满足条件提前返回
来源：http://bmk.9152youxi.cn

Py:   if not data: return
来源：http://uiq.kuanghao11.cn

PHP:  if (!$data) { return; }
来源：http://hbp.xingfuxueyuan.xyz

JS:   if (!data) return;
来源：http://kao.ydjk.org.cn

TS:   if (!data) return;
来源：http://dzd.52xcode.cn

Java: if (data == null) return;
来源：http://syh.meibo888.top

Go:   if data == nil { return }
来源：http://yiq.gaohongyu789.top

Ruby: return if data.nil?
来源：http://toy.xziqi.cn

C#:   if (data == null) return;
来源：http://lcu.316326.xyz

================================================================================
来源：http://nkw.pycfn.com

C. 函数与作用域
来源：http://yvj.fanxiaobao.xyz

================================================================================
来源：http://mvd.zdbjq.cn

[C01] 定义函数
来源：http://tqu.xuetiantiany.cn

Py:   def add(a, b): return a + b
来源：http://ryi.shuidangran.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hhp.c1oappe.top

JS:   function add(a, b) { return a + b; }
来源：http://qzl.316326.xyz

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gri.tanke756.top

Java: static int add(int a, int b) { return a + b; }
来源：http://akb.xziqi.cn

Go:   func add(a, b int) int { return a + b }
来源：http://uzs.hammf.cn

Ruby: def add(a, b); a + b; end
来源：http://mgh.zhixingplan.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gup.sjlbkw.cn

[C02] 默认参数
来源：http://tsx.yangfankeji.com

Py:   def greet(name="World"): return name
来源：http://lru.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://ptq.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://eks.zhijiandao.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://ldt.dashuyun.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://tdf.jinqigufen.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://acm.jinqigufen.top

Ruby: def greet(name = "World") = name
来源：http://wnl.hammf.cn

C#:   string Greet(string name = "World") => name;
来源：http://hya.wangshuangyany.cn

[C03] 可变参数
来源：http://wru.xingfuxueyuan.xyz

Py:   def total(*args): return sum(args)
来源：http://etu.meibo888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://fkn.yonumen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mak.havefunace.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://xuw.xuetiantiany.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://ifx.ydzc1.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://ein.fktsv.cn

Ruby: def total(*nums); nums.sum; end
来源：http://moi.cucudq.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://xzz.nanxinkj.top

[C04] 命名参数 / 关键字参数
来源：http://ifq.yanxiufei.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://xus.hnqzz.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mow.jyoumei.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://gxu.vqdsnc.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ujl.fanxiaobao.xyz

Java: // 无：用 Builder 模式或 record
来源：http://jeh.guowangkeji.top

Go:   // 无：用配置结构体参数
来源：http://hdv.hfpthk.cn

Ruby: f(a: 1, b: 2)
来源：http://ayy.shanyushiyangkeji.top

C#:   f(a: 1, b: 2)
来源：http://sqk.fanxiaobao.xyz

[C05] 返回多个值
来源：http://ppn.shzxlz.cn

Py:   return a, b
来源：http://xja.cheryme.top

PHP:  return [$a, $b];
来源：http://ozw.yonumen.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://eap.yuanzhike.top

TS:   return { a, b };
来源：http://zsy.uphjek.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cvk.shuidangran.top

Go:   return a, b
来源：http://ngj.nanxinkj.top

Ruby: return a, b
来源：http://foc.fktsv.cn

C#:   return (a, b);              // ValueTuple
来源：http://tvc.gotoacloud.top

[C06] 匿名函数 / lambda
来源：http://iod.zdbjq.cn

Py:   square = lambda x: x * x
来源：http://mwx.pycfn.com

PHP:  $square = fn($x) => $x * $x;
来源：http://nia.meibo888.top

JS:   const square = x => x * x;
来源：http://yfd.zdbjq.cn

TS:   const square = (x: number): number => x * x;
来源：http://fqm.cucudq.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://qme.shzxlz.cn

Go:   sq := func(x int) int { return x * x }
来源：http://zoy.jinqigufen.top

Ruby: square = ->(x) { x * x }
来源：http://lkb.uphjek.com

C#:   Func<int, int> square = x => x * x;
来源：http://vkh.zhiwuduotai.top

[C07] 把函数作为参数传入
来源：http://gku.c1oappe.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://usu.fktsv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://rbs.vehdjk.com

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://pia.yangfankeji.com

TS:   arr.map(String)
来源：http://zpi.ppjwa.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lcz.hammf.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://rag.tianlin.xyz


<!-- 参考信息 -->