代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lgk.fanxiaobao.xyz

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vgs.tian-w.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://odi.yonumen.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://sgu.guannengcc.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kyu.sjlbkw.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gpt.yuxming.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kbq.andypj.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ulq.yueranfly.top

[A18] 字符与 ASCII 码互转
来源：http://lat.tian-w.cn

Py:   ord("A"); chr(65)
来源：http://ibh.gzhubu.top

PHP:  ord("A"); chr(65)
来源：http://cay.hongshengwenyu.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ogt.yangfankeji.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hxm.birdmap.top

Java: (int) 'A'; (char) 65
来源：http://mcs.yj202588.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://lwr.fehbvm.com

Ruby: "A".ord; 65.chr
来源：http://uxc.nanxinkj.top

C#:   (int)'A'; (char)65
来源：http://eta.chenzaomai.com

[A19] 交换两个变量
来源：http://kzm.smart0.xyz

Py:   a, b = b, a
来源：http://vjs.sweek.top

PHP:  [$a, $b] = [$b, $a];
来源：http://dsb.aizwys.cn

JS:   [a, b] = [b, a];
来源：http://hqh.guowangkeji.top

TS:   [a, b] = [b, a];
来源：http://eep.zhongyouzk.top

Java: int t = a; a = b; b = t;
来源：http://wlp.jiagoushi.top

Go:   a, b = b, a
来源：http://psp.jiagoushi.top

Ruby: a, b = b, a
来源：http://auy.zycfv.cn

C#:   (a, b) = (b, a);
来源：http://ewe.guannengcc.top

[A20] 读取标准输入
来源：http://eaj.pycfn.com

Py:   name = input("请输入：")
来源：http://hkh.chenlongwang.top

PHP:  $name = trim(fgets(STDIN));
来源：http://drv.yueranfly.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://amu.yj202588.top

TS:   // Node.js：readline 模块
来源：http://uhh.zhixingplan.top

Java: new Scanner(System.in).nextLine()
来源：http://lrr.shzxlz.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://cql.gotoacloud.top

Ruby: gets.chomp
来源：http://oly.pycfn.com

C#:   Console.ReadLine();
来源：http://nmy.cucudq.cn

[A21] 保留指定小数位输出
来源：http://ghw.ctjpmb.com

Py:   f"{3.14159:.2f}"
来源：http://ejw.yj202588.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pll.guowangkeji.top

JS:   (3.14159).toFixed(2)
来源：http://zia.zhongyouzk.top

TS:   (3.14159).toFixed(2)
来源：http://smt.jinyuanbaomall.cn

Java: String.format("%.2f", 3.14159)
来源：http://jpu.fehbvm.com

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xnv.aibaodan.cn

Ruby: format("%.2f", 3.14159)
来源：http://vxv.snrcjt.cn

C#:   3.14159.ToString("F2")
来源：http://kts.dashuyun.cn

[A22] 获取字符串长度
来源：http://igt.wangdashe.top

Py:   len(s)
来源：http://dvh.jianghu66.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ety.xziqi.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gii.jiagoushi.top

TS:   s.length
来源：http://cot.xuanzx.com

Java: s.length()
来源：http://ioe.jinyuanbaomall.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ywx.ydjk.org.cn

Ruby: s.length
来源：http://uck.yuanzhike.top

C#:   s.Length
来源：http://awo.wangdashe.top

[A23] 大小写转换
来源：http://mab.hammf.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://lik.chenzaomai.com

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://fbb.jiagoushi.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://sua.shzxlz.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://bqg.c1oappe.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://tdt.tanke756.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://odj.gotoacloud.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://uom.gogol.net.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://pvc.aizwys.cn

[A24] 去除首尾空白
来源：http://siw.hysaishi.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://agl.yj20258888.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://fbn.ywan-chungtsiang.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://dfa.hnqzz.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jkf.ehwqpu.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mww.ybcxt.top

Go:   strings.TrimSpace(s)
来源：http://fnr.ybcxt.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://jxb.jiagoushi.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://tub.shangyingyoupin.top

[A25] 字符串比较
来源：http://esi.jinqigufen.top

Py:   s1 == s2; s1 != s2
来源：http://oha.hfpthk.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://iir.daxiang520.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rii.zhijiandao.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://zwa.xylfe.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://lyr.0kj1m.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ioo.cheryme.top

Ruby: s1 == s2; s1 <=> s2
来源：http://kab.sxryk.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nnf.tanke756.top

[A26] 类型转换总览
来源：http://hjd.jianghu66.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://chk.fehbvm.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://bss.nanxuanxn.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://sjo.jinghuilouyu.cn

TS:   Number() String() Boolean() x as number
来源：http://ibk.hnxiangtu.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://wjg.316326.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://guc.havefunace.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://stz.jinqigfzy.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://fui.yongpay.top

================================================================================
来源：http://gic.xingfuxueyuan.xyz

B. 流程控制
来源：http://wxk.shzxlz.cn

================================================================================
来源：http://hif.guannengcc.top

[B01] 条件判断 if / else
来源：http://umf.xylfe.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://tpm.yj202588.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ukz.smart0.xyz

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zmc.zhaomingkeji.xyz

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ecw.fktsv.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://dki.hysaishi.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://shx.gotoacloud.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ydv.yanxiufei.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://rvi.jyoumei.cn

[B02] 多分支 else if / elif
来源：http://awi.9152youxi.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://fym.redwolf501.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://dje.vehdjk.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://sli.ivvv.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rct.fanxiaobao.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hkt.zycfv.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://rbo.hnqzz.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://lpx.xuanzx.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://liq.feifeiyinyue.top

[B03] switch / match / case
来源：http://joo.guannengcc.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://rxz.yuxming.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://oxs.sysykeji.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yql.ppjwa.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cwx.zhoulong.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://bqa.yj202588.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://vzn.yfazqb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wct.daxiang520.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://exs.c1oappe.top

[B04] for 计数循环
来源：http://vhk.jianghu66.top

Py:   for i in range(10): print(i)
来源：http://vez.jqgufenzy.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://icq.jlsjyb.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fmy.jinqigfzy.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://bdh.yj20258888.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pls.smart0.xyz

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://bft.shangyingyoupin.top

Ruby: 10.times { |i| puts i }
来源：http://luy.hywenlv.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wbr.sweek.top

[B05] 遍历数组 / 列表
来源：http://wak.ywan-chungtsiang.top

Py:   for item in arr: print(item)
来源：http://sli.ydjk.org.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://cpj.fanxiaobao.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://kix.hongshengwenyu.top

TS:   for (const item of arr) { console.log(item); }
来源：http://mqq.hfpthk.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://ezm.zhijiandao.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://bgr.sweek.top

Ruby: arr.each { |item| puts item }
来源：http://lmt.pengpengdd.cyou

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uuy.xingfuxueyuan.xyz

[B06] 遍历字典 / 对象
来源：http://jmb.shzxlz.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://kxo.vehdjk.com

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nzm.xziqi.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://klt.316326.xyz

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://kui.cdnleiting.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://xux.ywan-chungtsiang.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hdq.redwolf501.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hpy.jiagoushi.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hxu.svipenyu.cn

[B07] while 循环
来源：http://syl.tianlin.xyz

Py:   while i < 10: i += 1
来源：http://kab.zycfv.cn

PHP:  while ($i < 10) { $i++; }
来源：http://aul.jianghu66.top

JS:   while (i < 10) { i++; }
来源：http://duq.yj202588.top

TS:   while (i < 10) { i++; }
来源：http://ory.meibo888.top

Java: while (i < 10) { i++; }
来源：http://drc.pengpengdd.cyou

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nrl.ppjwa.cn

Ruby: while i < 10; i += 1; end
来源：http://zcq.andypj.xyz

C#:   while (i < 10) { i++; }
来源：http://oum.gogol.net.cn

[B08] do-while（至少执行一次）
来源：http://qpw.mhx1999.top

Py:   # 无 do-while：用 while True + break
来源：http://amw.gogol.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://jdy.jyoumei.cn

JS:   do { i++; } while (i < 10);
来源：http://wfw.ivvv.top

TS:   do { i++; } while (i < 10);
来源：http://ctn.ydjk.org.cn

Java: do { i++; } while (i < 10);
来源：http://rcz.ehwqpu.com

Go:   for { i++; if i >= 10 { break } }
来源：http://xwo.wangshuangyany.cn

Ruby: begin; i += 1; end while i < 10
来源：http://tny.guannengcc.top

C#:   do { i++; } while (i < 10);
来源：http://hwn.cheryme.top

[B09] break 与 continue
来源：http://jhp.ybcxt.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://yss.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://pgh.yuxming.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mnb.fktsv.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ewd.wangshuangyany.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ykm.gotoacloud.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://okn.pycfn.com

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://xqn.chenjidiqi.icu

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://tan.redwolf501.top

[B10] 遍历同时拿索引
来源：http://zhe.ivvv.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://zkd.pycfn.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://iwb.zhongyouzk.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://iyy.jinqigufen.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://era.fktsv.cn

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://bls.vqdsnc.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://fut.sufxvd.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rld.zhiwuduotai.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vcv.yj20258888.top

[B11] 生成数字序列 / 区间
来源：http://nbd.xuetiantiany.cn

Py:   list(range(0, 10, 2))
来源：http://kkb.chenlongwang.top

PHP:  range(0, 10, 2);
来源：http://kqd.sufxvd.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://onl.xylfe.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dfj.mhx1999.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://pls.feifeiyinyue.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://djh.yj20258.top

Ruby: (0...10).step(2).to_a
来源：http://mmt.zhengqikj.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://dag.fehbvm.com

[B12] 跳出多层循环
来源：http://klz.vqdsnc.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://scv.9152youxi.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://mhn.ybcxt.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://vup.pycfn.com

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ipj.jlsjyb.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://ovq.shanyushiyangtech.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cyr.sjlbkw.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://vha.ehwqpu.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wfq.nwbrower.top

[B13] 判断是否为数字
来源：http://yzp.yueranfly.top

Py:   isinstance(x, (int, float))
来源：http://gqq.chenjidiqi.icu

PHP:  is_numeric($x)
来源：http://snh.xingfuxueyuan.xyz

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://yrt.guannengcc.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://dup.snrcjt.cn

Java: x instanceof Number
来源：http://mqu.pycfn.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xyi.sufxvd.cn

Ruby: x.is_a?(Numeric)
来源：http://qlf.shangyingyoupin.top

C#:   x is int or double or decimal
来源：http://spz.tianlin.xyz

[B14] 判断值是否在集合内
来源：http://zdm.xuetiantiany.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://upn.aizwys.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://uro.kuanghao11.cn

JS:   [1, 2, 3].includes(x)
来源：http://dbm.quarkkingdee.top

TS:   [1, 2, 3].includes(x)
来源：http://udi.gogol.net.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://kim.fengsongda.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://aci.xuanzx.com

Ruby: [1, 2, 3].include?(x)
来源：http://ckj.yonumen.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://woj.ywan-chungtsiang.top

[B15] 布尔运算与取反
来源：http://hpx.daria6918.cn

Py:   a and b or not c
来源：http://jad.yuxming.cn

PHP:  $a && $b || !$c
来源：http://zwn.zhaomingkeji.xyz

JS:   a && b || !c
来源：http://vwh.zdbjq.cn

TS:   a && b || !c
来源：http://cwm.shuidangran.top

Java: a && b || !c
来源：http://keo.ctjpmb.com

Go:   a && b || !c
来源：http://xnd.zhengqikj.top

Ruby: a && b || !c
来源：http://jxm.svipenyu.cn

C#:   a && b || !c
来源：http://meh.cucudq.cn

[B16] 卫语句：不满足条件提前返回
来源：http://qut.cdnleiting.top

Py:   if not data: return
来源：http://hbq.epnwcf.com

PHP:  if (!$data) { return; }
来源：http://yuz.vehdjk.com

JS:   if (!data) return;
来源：http://jvw.andypj.xyz

TS:   if (!data) return;
来源：http://eln.xuanzx.com

Java: if (data == null) return;
来源：http://gkd.tian-w.cn

Go:   if data == nil { return }
来源：http://iig.xuanzx.com

Ruby: return if data.nil?
来源：http://dyq.yanxiufei.cn

C#:   if (data == null) return;
来源：http://aol.bjfxy.top

================================================================================
来源：http://huh.yangfankeji.com

C. 函数与作用域
来源：http://ifk.meibo888.top

================================================================================
来源：http://mlp.aibaodan.cn

[C01] 定义函数
来源：http://euq.zhongyouzk.top

Py:   def add(a, b): return a + b
来源：http://ias.zycfv.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xwg.yongpay.top

JS:   function add(a, b) { return a + b; }
来源：http://jjg.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ogp.ctjpmb.com

Java: static int add(int a, int b) { return a + b; }
来源：http://onp.sjlbkw.cn

Go:   func add(a, b int) int { return a + b }
来源：http://hvz.jinqigfzy.top

Ruby: def add(a, b); a + b; end
来源：http://npt.ybcxt.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fsz.aizwys.cn

[C02] 默认参数
来源：http://sql.guannengcc.top

Py:   def greet(name="World"): return name
来源：http://vrf.fehbvm.com

PHP:  function greet($name = "World") { return $name; }
来源：http://shp.zdbjq.cn

JS:   function greet(name = "World") { return name; }
来源：http://lzd.hnqzz.top

TS:   function greet(name: string = "World") { return name; }
来源：http://zbx.hysaishi.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://ddq.sufxvd.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://tbl.daxiang520.top

Ruby: def greet(name = "World") = name
来源：http://phe.nanxinkj.top

C#:   string Greet(string name = "World") => name;
来源：http://jxs.ydzc1.top

[C03] 可变参数
来源：http://nzt.guowangkeji.top

Py:   def total(*args): return sum(args)
来源：http://vvh.hysaishi.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://iaw.chenlongwang.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://afs.shuidangran.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://zjy.vqdsnc.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://vvh.yongpay.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://vnd.ehwqpu.com

Ruby: def total(*nums); nums.sum; end
来源：http://ziv.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://omm.9152youxi.cn

[C04] 命名参数 / 关键字参数
来源：http://lrq.mhx1999.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://lfp.yfazqb.com

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://dtm.xinyue.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://jvy.snrcjt.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://jhq.yj202588.top

Java: // 无：用 Builder 模式或 record
来源：http://kap.ehwqpu.com

Go:   // 无：用配置结构体参数
来源：http://piq.tianlin.xyz

Ruby: f(a: 1, b: 2)
来源：http://peu.aizwys.cn

C#:   f(a: 1, b: 2)
来源：http://naz.shangyingyoupin.top

[C05] 返回多个值
来源：http://sfb.xuanzx.com

Py:   return a, b
来源：http://qdc.cashguo.top

PHP:  return [$a, $b];
来源：http://rav.xinyue.icu

JS:   return [a, b];             // 或 return { a, b };
来源：http://rxg.dianchejie.cn

TS:   return { a, b };
来源：http://omq.ywan-chungtsiang.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://jct.shuidangran.top

Go:   return a, b
来源：http://sgz.aizwys.cn

Ruby: return a, b
来源：http://eve.c1oappe.top

C#:   return (a, b);              // ValueTuple
来源：http://qak.jianghu66.top

[C06] 匿名函数 / lambda
来源：http://xjq.xinyue.icu

Py:   square = lambda x: x * x
来源：http://van.fehbvm.com

PHP:  $square = fn($x) => $x * $x;
来源：http://chy.jqgfzy.top

JS:   const square = x => x * x;
来源：http://ynf.zdqjudy.top

TS:   const square = (x: number): number => x * x;
来源：http://awu.snrcjt.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://nex.shangyingyoupin.top

Go:   sq := func(x int) int { return x * x }
来源：http://rgt.bbcook.cn

Ruby: square = ->(x) { x * x }
来源：http://djq.yuxming.cn

C#:   Func<int, int> square = x => x * x;
来源：http://btj.hesvh.cn

[C07] 把函数作为参数传入
来源：http://zrh.cashguo.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://oaq.zycfv.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wej.jinqigfzy.top

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yes.xuetiantiany.cn

TS:   arr.map(String)
来源：http://tgu.mhx1999.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dnl.gaohongyu789.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hsi.chenjidiqi.icu


<!-- 参考信息 -->