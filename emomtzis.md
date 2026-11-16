代发 wailian999

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://egg.gaohongyu789.top

Ruby: unless x            # nil 与 false 为假
来源：http://qwi.pengpengdd.cyou

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://yde.wangdashe.top

[A17] 位运算
来源：http://szb.iojbl.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://chl.jinyuanbaomall.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://vyi.bbcook.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://apq.cheryme.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://bhz.jinqigfzy.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vdi.jyoumei.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://ehz.ybcxt.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yot.yongpay.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nkq.ydzc1.top

[A18] 字符与 ASCII 码互转
来源：http://wea.sweek.top

Py:   ord("A"); chr(65)
来源：http://zfx.xylfe.cn

PHP:  ord("A"); chr(65)
来源：http://qnt.ppjwa.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://shr.gogol.net.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xmk.wangshuangyany.cn

Java: (int) 'A'; (char) 65
来源：http://qcz.tanke756.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://vmc.ehwqpu.com

Ruby: "A".ord; 65.chr
来源：http://ykg.zhoulong.xyz

C#:   (int)'A'; (char)65
来源：http://vhs.jyoumei.cn

[A19] 交换两个变量
来源：http://qry.chenlongwang.top

Py:   a, b = b, a
来源：http://zyv.yfazqb.com

PHP:  [$a, $b] = [$b, $a];
来源：http://bgo.aibaodan.cn

JS:   [a, b] = [b, a];
来源：http://gqi.yj20258888.top

TS:   [a, b] = [b, a];
来源：http://fiw.hnqzz.top

Java: int t = a; a = b; b = t;
来源：http://vgn.nwbrower.top

Go:   a, b = b, a
来源：http://zdv.fktsv.cn

Ruby: a, b = b, a
来源：http://znu.yongpay.top

C#:   (a, b) = (b, a);
来源：http://ute.shanyushiyangkeji.top

[A20] 读取标准输入
来源：http://kav.hfpthk.cn

Py:   name = input("请输入：")
来源：http://fuw.c1oappe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://jhz.cqqwz.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://vjx.0kj1m.cn

TS:   // Node.js：readline 模块
来源：http://arn.quarkkingdee.top

Java: new Scanner(System.in).nextLine()
来源：http://mjy.aibaodan.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://tsc.jqgfzy.top

Ruby: gets.chomp
来源：http://den.sjlbkw.cn

C#:   Console.ReadLine();
来源：http://guj.xuetiantiany.cn

[A21] 保留指定小数位输出
来源：http://hov.gaohongyu789.top

Py:   f"{3.14159:.2f}"
来源：http://ooj.cashguo.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://pkm.jianghu66.top

JS:   (3.14159).toFixed(2)
来源：http://nku.xylfe.cn

TS:   (3.14159).toFixed(2)
来源：http://ces.zhijiandao.cn

Java: String.format("%.2f", 3.14159)
来源：http://hwi.bjfxy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hho.yuanzhike.top

Ruby: format("%.2f", 3.14159)
来源：http://jiy.ctjpmb.com

C#:   3.14159.ToString("F2")
来源：http://yho.fanxiaobao.xyz

[A22] 获取字符串长度
来源：http://tod.daxiang520.top

Py:   len(s)
来源：http://ncs.yj20258.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://fpc.wangdashe.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://yuz.sweek.top

TS:   s.length
来源：http://xpa.zdqjudy.top

Java: s.length()
来源：http://hdr.zdbjq.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ckm.gaohongyu789.top

Ruby: s.length
来源：http://eqe.hfpthk.cn

C#:   s.Length
来源：http://ywf.vqdsnc.cn

[A23] 大小写转换
来源：http://igs.gzhubu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://erq.tianlin.xyz

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://kvl.xinyue.icu

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://xvk.ydjk.org.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://iuj.cheryme.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qbc.dashuyun.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hqn.tianlin.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://djs.jiagoushi.top

C#:   s.ToUpper(); s.ToLower()
来源：http://roq.wangdashe.top

[A24] 去除首尾空白
来源：http://yfj.jinghuilouyu.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://nyi.fzhhl.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://qbe.hesvh.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://amx.zhongyouzk.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://prv.tianlin.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://cln.cheryme.top

Go:   strings.TrimSpace(s)
来源：http://xyf.yongpay.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://nol.cashguo.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://qei.shzxlz.cn

[A25] 字符串比较
来源：http://xkx.xuetiantiany.cn

Py:   s1 == s2; s1 != s2
来源：http://uxy.zhiwuduotai.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://rph.zdqjudy.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://fjx.zhaomingkeji.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gju.hammf.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://gyt.hywenlv.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://tta.cheryme.top

Ruby: s1 == s2; s1 <=> s2
来源：http://xqv.zhongyouzk.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wmg.nanxinkj.top

[A26] 类型转换总览
来源：http://vdf.yj20258888.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://grj.mhx1999.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://itf.hesvh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tnd.zhiwuduotai.top

TS:   Number() String() Boolean() x as number
来源：http://dro.hcnkem.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://agg.daxiang520.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://yjr.gotoacloud.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://dby.hnxiangtu.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rwq.hnqzz.top

================================================================================
来源：http://ghy.jlsjyb.cn

B. 流程控制
来源：http://aog.ctjpmb.com

================================================================================
来源：http://rac.chenzaomai.com

[B01] 条件判断 if / else
来源：http://ylp.yvedp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://yjy.hnqzz.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://rwo.0kj1m.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://jdt.sweek.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ppa.xuanzx.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://ars.tarul.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fay.yfazqb.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jjy.epnwcf.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wli.cashguo.top

[B02] 多分支 else if / elif
来源：http://wld.nanxinkj.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://owu.shzxlz.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://olf.yj202588.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://llb.ivvv.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cui.xuetiantiany.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://aop.jianghu66.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://czg.bbcook.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://cdu.chenzaomai.com

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mtk.snrcjt.cn

[B03] switch / match / case
来源：http://tev.shzxlz.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mrl.jinqigfzy.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://aom.shanyushiyangtech.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sya.shanyushiyangtech.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oxi.meibo888.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ygt.gogol.net.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://cii.yfazqb.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://xec.vehdjk.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://zor.feifeiyinyue.top

[B04] for 计数循环
来源：http://htm.chenjidiqi.icu

Py:   for i in range(10): print(i)
来源：http://thx.dashuyun.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://auo.sweek.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://dpw.ydzc1.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://iqp.ybcxt.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ese.9152youxi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://euy.cdnleiting.top

Ruby: 10.times { |i| puts i }
来源：http://apy.bbcook.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://jid.sweek.top

[B05] 遍历数组 / 列表
来源：http://yco.sweek.top

Py:   for item in arr: print(item)
来源：http://oqp.tianlin.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://gey.zhijiandao.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://sfw.zhoulong.xyz

TS:   for (const item of arr) { console.log(item); }
来源：http://cze.hcnkem.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://bez.dashuyun.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://adq.jqgfzy.top

Ruby: arr.each { |item| puts item }
来源：http://hwy.mhx1999.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://mnx.haohaochexian.top

[B06] 遍历字典 / 对象
来源：http://zno.hcnkem.com

Py:   for k, v in d.items(): print(k, v)
来源：http://iuk.yj20258.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://nzv.quarkkingdee.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rte.jqgfzy.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://zye.guannengcc.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ooo.nwbrower.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://cdd.sweek.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://tjq.zhengqikj.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://eec.9152youxi.cn

[B07] while 循环
来源：http://gyn.snrcjt.cn

Py:   while i < 10: i += 1
来源：http://yfe.nanxuanxn.top

PHP:  while ($i < 10) { $i++; }
来源：http://yjj.hcnkem.com

JS:   while (i < 10) { i++; }
来源：http://lsb.chenjidiqi.icu

TS:   while (i < 10) { i++; }
来源：http://bdp.daria6918.cn

Java: while (i < 10) { i++; }
来源：http://amx.yongpay.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kfw.epnwcf.com

Ruby: while i < 10; i += 1; end
来源：http://gyj.sweek.top

C#:   while (i < 10) { i++; }
来源：http://jcg.yanxiufei.cn

[B08] do-while（至少执行一次）
来源：http://xvo.hammf.cn

Py:   # 无 do-while：用 while True + break
来源：http://pdo.hesvh.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://zfw.jqgfzy.top

JS:   do { i++; } while (i < 10);
来源：http://iuf.snrcjt.cn

TS:   do { i++; } while (i < 10);
来源：http://cuv.fktsv.cn

Java: do { i++; } while (i < 10);
来源：http://efw.ybcxt.top

Go:   for { i++; if i >= 10 { break } }
来源：http://tth.yj202588.top

Ruby: begin; i += 1; end while i < 10
来源：http://uqq.tanke756.top

C#:   do { i++; } while (i < 10);
来源：http://rje.redwolf501.top

[B09] break 与 continue
来源：http://lpl.shanyushiyangtech.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zxm.zhoulong.xyz

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hru.snrcjt.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zxd.jinyuanbaomall.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://cyr.yj20258888.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://maw.guowangkeji.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hpo.guannengcc.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ugh.guannengcc.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mmu.jlsjyb.cn

[B10] 遍历同时拿索引
来源：http://dtk.dianchejie.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://fth.jlsjyb.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://pob.dianchejie.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qoq.guowangkeji.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dup.feifeiyinyue.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://wxz.uphjek.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://yoi.gogol.net.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ugq.jinqigfzy.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ujq.zhixingplan.top

[B11] 生成数字序列 / 区间
来源：http://sqh.zdqjudy.top

Py:   list(range(0, 10, 2))
来源：http://xfh.shanyushiyangkeji.top

PHP:  range(0, 10, 2);
来源：http://bqr.haohaochexian.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ssj.daria6918.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hpb.jianghu66.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://afk.nanxuanxn.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dlh.epnwcf.com

Ruby: (0...10).step(2).to_a
来源：http://smc.iojbl.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yju.wangdashe.top

[B12] 跳出多层循环
来源：http://net.fanxiaobao.xyz

Py:   # 无标签跳转：抽成函数用 return
来源：http://yvo.meibo888.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://cjs.yanxiufei.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://zfv.chenjidiqi.icu

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hrb.snrcjt.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://jca.chenzaomai.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://oru.tian-w.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://gib.dashuyun.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://elm.dianchejie.cn

[B13] 判断是否为数字
来源：http://trd.52xcode.cn

Py:   isinstance(x, (int, float))
来源：http://aop.xuanzx.com

PHP:  is_numeric($x)
来源：http://wlo.wangshuangyany.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sme.jqgufenzy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://vds.zhongyouzk.top

Java: x instanceof Number
来源：http://szx.hammf.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://ouh.zhaomingkeji.xyz

Ruby: x.is_a?(Numeric)
来源：http://oog.jinghuilouyu.cn

C#:   x is int or double or decimal
来源：http://bkm.havefunace.top

[B14] 判断值是否在集合内
来源：http://phu.zhaomingkeji.xyz

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://lea.epnwcf.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://zlg.shanyushiyangkeji.top

JS:   [1, 2, 3].includes(x)
来源：http://oss.quarkkingdee.top

TS:   [1, 2, 3].includes(x)
来源：http://nxh.tarul.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://how.9152youxi.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://god.jqgfzy.top

Ruby: [1, 2, 3].include?(x)
来源：http://rwb.yanxiufei.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://xqu.sysykeji.top

[B15] 布尔运算与取反
来源：http://lnr.hammf.cn

Py:   a and b or not c
来源：http://yoy.zycfv.cn

PHP:  $a && $b || !$c
来源：http://tnr.zycfv.cn

JS:   a && b || !c
来源：http://ppo.hongshengwenyu.top

TS:   a && b || !c
来源：http://nhq.hfpthk.cn

Java: a && b || !c
来源：http://rwd.yueranfly.top

Go:   a && b || !c
来源：http://ljm.yfazqb.com

Ruby: a && b || !c
来源：http://sch.dianchejie.cn

C#:   a && b || !c
来源：http://ddk.uphjek.com

[B16] 卫语句：不满足条件提前返回
来源：http://rah.jqgfzy.top

Py:   if not data: return
来源：http://qbq.shanyushiyangtech.top

PHP:  if (!$data) { return; }
来源：http://paa.ybcxt.top

JS:   if (!data) return;
来源：http://qly.yangfankeji.com

TS:   if (!data) return;
来源：http://peq.iojbl.cn

Java: if (data == null) return;
来源：http://gsr.sysykeji.top

Go:   if data == nil { return }
来源：http://nqa.fanxiaobao.xyz

Ruby: return if data.nil?
来源：http://isy.zhoulong.xyz

C#:   if (data == null) return;
来源：http://zjh.zhengqikj.top

================================================================================
来源：http://zfk.yfazqb.com

C. 函数与作用域
来源：http://enb.wangshuangyany.cn

================================================================================
来源：http://kjx.chenjidiqi.icu

[C01] 定义函数
来源：http://mqr.cdnleiting.top

Py:   def add(a, b): return a + b
来源：http://mqx.hysaishi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fgl.xuetiantiany.cn

JS:   function add(a, b) { return a + b; }
来源：http://djj.ywan-chungtsiang.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://dlj.cashguo.top

Java: static int add(int a, int b) { return a + b; }
来源：http://pky.havefunace.top

Go:   func add(a, b int) int { return a + b }
来源：http://wbh.shanyushiyangkeji.top

Ruby: def add(a, b); a + b; end
来源：http://mpx.ywan-chungtsiang.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yfo.epnwcf.com

[C02] 默认参数
来源：http://mme.nanxuanxn.top

Py:   def greet(name="World"): return name
来源：http://qsq.ydzc1.top

PHP:  function greet($name = "World") { return $name; }
来源：http://qpu.wangdashe.top

JS:   function greet(name = "World") { return name; }
来源：http://jec.jinyuanbaomall.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://njo.sjlbkw.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://jmp.shanyushiyangtech.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rdn.uphjek.com

Ruby: def greet(name = "World") = name
来源：http://oge.guannengcc.top

C#:   string Greet(string name = "World") => name;
来源：http://kcd.shuidangran.top

[C03] 可变参数
来源：http://ajp.zhongyouzk.top

Py:   def total(*args): return sum(args)
来源：http://zsi.cashguo.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xgz.fengsongda.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://pnl.aizwys.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://oww.jqgufenzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://kha.zhaomingkeji.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://sqm.yanxiufei.cn

Ruby: def total(*nums); nums.sum; end
来源：http://gmt.316326.xyz

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://dwq.sysykeji.top

[C04] 命名参数 / 关键字参数
来源：http://xez.pycfn.com

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://opj.bbcook.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mdl.chenjidiqi.icu

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://xcq.zycfv.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://gpz.tanke756.top

Java: // 无：用 Builder 模式或 record
来源：http://cqq.guannengcc.top

Go:   // 无：用配置结构体参数
来源：http://fns.redwolf501.top

Ruby: f(a: 1, b: 2)
来源：http://iqe.ydzc1.top

C#:   f(a: 1, b: 2)
来源：http://ftu.vehdjk.com

[C05] 返回多个值
来源：http://vkp.nwbrower.top

Py:   return a, b
来源：http://frv.jqgfzy.top

PHP:  return [$a, $b];
来源：http://qrc.cqqwz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://xqp.zhongyouzk.top

TS:   return { a, b };
来源：http://yiy.hnxiangtu.top

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mcs.vqdsnc.cn

Go:   return a, b
来源：http://yhd.daria6918.cn

Ruby: return a, b
来源：http://fek.andypj.xyz

C#:   return (a, b);              // ValueTuple
来源：http://lei.hywenlv.cn

[C06] 匿名函数 / lambda
来源：http://xhr.hnxiangtu.top

Py:   square = lambda x: x * x
来源：http://ejq.dianchejie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://znp.gaohongyu789.top

JS:   const square = x => x * x;
来源：http://jfn.feifeiyinyue.top

TS:   const square = (x: number): number => x * x;
来源：http://fjt.snrcjt.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://fft.kuanghao11.cn

Go:   sq := func(x int) int { return x * x }
来源：http://ifb.jiagoushi.top

Ruby: square = ->(x) { x * x }
来源：http://sli.9152youxi.cn

C#:   Func<int, int> square = x => x * x;
来源：http://myu.svipenyu.cn

[C07] 把函数作为参数传入
来源：http://mvr.xuanzx.com

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://aza.cdnleiting.top

PHP:  array_map("strtoupper", $arr);
来源：http://bwa.xuetiantiany.cn


<!-- 参考信息 -->