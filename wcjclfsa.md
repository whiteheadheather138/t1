代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://xvy.xziqi.cn

[A15] 空值判断与默认值
来源：http://vqu.52xcode.cn

Py:   value = data or "默认值"
来源：http://obm.birdmap.top

PHP:  $value = $data ?? "默认值";
来源：http://lfe.cheryme.top

JS:   const value = data ?? "默认值";
来源：http://ptw.gogol.net.cn

TS:   const value = data ?? "默认值";
来源：http://ctd.yuxming.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://nga.fanxiaobao.xyz

Go:   if data == "" { data = "默认值" }
来源：http://yna.redwolf501.top

Ruby: value = data || "默认值"
来源：http://iab.aizwys.cn

C#:   var value = data ?? "默认值";
来源：http://sie.ybcxt.top

[A16] 真假值判断规则
来源：http://qiw.mhx1999.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://swi.chenjidiqi.icu

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://trr.sysykeji.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hji.xinyue.icu

TS:   if (!x) {}
来源：http://cvf.yongpay.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://vlr.xuetiantiany.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://ijf.zycfv.cn

Ruby: unless x            # nil 与 false 为假
来源：http://vja.c1oappe.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://onl.redwolf501.top

[A17] 位运算
来源：http://wwe.zhiwuduotai.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tsv.zhiwuduotai.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://swi.daxiang520.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oqu.zhengqikj.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://gzr.cucudq.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ufp.jinghuilouyu.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mvf.svipenyu.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fxe.haohaochexian.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://dna.dashuyun.cn

[A18] 字符与 ASCII 码互转
来源：http://eye.sxryk.cn

Py:   ord("A"); chr(65)
来源：http://vom.jinyuanbaomall.cn

PHP:  ord("A"); chr(65)
来源：http://eat.hammf.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tns.zdqjudy.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://fjj.yongpay.top

Java: (int) 'A'; (char) 65
来源：http://xqr.yj20258.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tkj.chenjidiqi.icu

Ruby: "A".ord; 65.chr
来源：http://wdv.yongpay.top

C#:   (int)'A'; (char)65
来源：http://thh.hywenlv.cn

[A19] 交换两个变量
来源：http://jmj.shzxlz.cn

Py:   a, b = b, a
来源：http://dvy.zhijiandao.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://noz.hywenlv.cn

JS:   [a, b] = [b, a];
来源：http://nfm.ydjk.org.cn

TS:   [a, b] = [b, a];
来源：http://xgi.zdqjudy.top

Java: int t = a; a = b; b = t;
来源：http://smk.52xcode.cn

Go:   a, b = b, a
来源：http://qva.jqgufenzy.top

Ruby: a, b = b, a
来源：http://khm.yj202588.top

C#:   (a, b) = (b, a);
来源：http://jkd.bjfxy.top

[A20] 读取标准输入
来源：http://amp.shzxlz.cn

Py:   name = input("请输入：")
来源：http://mhb.shanyushiyangtech.top

PHP:  $name = trim(fgets(STDIN));
来源：http://vwm.daria6918.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://yoj.zhixingplan.top

TS:   // Node.js：readline 模块
来源：http://dms.uphjek.com

Java: new Scanner(System.in).nextLine()
来源：http://six.guowangkeji.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://wbc.yuanzhike.top

Ruby: gets.chomp
来源：http://ckh.yvedp.cn

C#:   Console.ReadLine();
来源：http://rxt.sjlbkw.cn

[A21] 保留指定小数位输出
来源：http://zup.bbcook.cn

Py:   f"{3.14159:.2f}"
来源：http://jse.0kj1m.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://tuh.jinghuilouyu.cn

JS:   (3.14159).toFixed(2)
来源：http://vvt.yj20258.top

TS:   (3.14159).toFixed(2)
来源：http://wnm.jqgufenzy.top

Java: String.format("%.2f", 3.14159)
来源：http://khv.birdmap.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://aqf.hongshengwenyu.top

Ruby: format("%.2f", 3.14159)
来源：http://xxp.shuidangran.top

C#:   3.14159.ToString("F2")
来源：http://cuq.52xcode.cn

[A22] 获取字符串长度
来源：http://vgz.shanyushiyangkeji.top

Py:   len(s)
来源：http://nmv.cucudq.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sqq.shanyushiyangkeji.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ljl.uphjek.com

TS:   s.length
来源：http://dka.jqgfzy.top

Java: s.length()
来源：http://dcm.tanke756.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://fzc.fehbvm.com

Ruby: s.length
来源：http://uce.jyoumei.cn

C#:   s.Length
来源：http://hco.ydjk.org.cn

[A23] 大小写转换
来源：http://pny.zhijiandao.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://rbe.nwbrower.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://bnq.9152youxi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://etn.shangyingyoupin.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://gyo.zhaomingkeji.xyz

Java: s.toUpperCase(); s.toLowerCase()
来源：http://xmu.epnwcf.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://rad.snrcjt.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://eeb.fktsv.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://bjm.tarul.cn

[A24] 去除首尾空白
来源：http://twf.xylfe.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://vpo.havefunace.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://kmz.yj20258.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eee.jianghu66.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://bhf.bjfxy.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://ibw.vqdsnc.cn

Go:   strings.TrimSpace(s)
来源：http://nwe.jiagoushi.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://eiy.sjlbkw.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://xaj.snrcjt.cn

[A25] 字符串比较
来源：http://rxd.sxryk.cn

Py:   s1 == s2; s1 != s2
来源：http://isp.hongshengwenyu.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tss.zycfv.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://mgd.chenjidiqi.icu

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tkz.jinqigfzy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://qyj.jlsjyb.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://irk.dashuyun.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://geu.ehwqpu.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://acm.sysykeji.top

[A26] 类型转换总览
来源：http://trn.yongpay.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://noe.chenzaomai.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://gcg.quarkkingdee.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cst.zycfv.cn

TS:   Number() String() Boolean() x as number
来源：http://agn.yongpay.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://psn.316326.xyz

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://zft.yfazqb.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://zjn.nanxuanxn.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zrh.ppjwa.cn

================================================================================
来源：http://xrt.yuxming.cn

B. 流程控制
来源：http://zom.quarkkingdee.top

================================================================================
来源：http://kla.jinqigfzy.top

[B01] 条件判断 if / else
来源：http://xtp.fktsv.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://kcr.hysaishi.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://bux.hysaishi.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mum.ivvv.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://znv.jinyuanbaomall.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://pbk.gotoacloud.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hpl.snrcjt.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://giv.bbcook.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://fdk.jianghu66.top

[B02] 多分支 else if / elif
来源：http://nyv.zhiwuduotai.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ngx.guannengcc.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://agg.yangfankeji.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fgu.hesvh.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://upj.dashuyun.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xqj.yj20258888.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://gbi.zhaomingkeji.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ntl.jqgufenzy.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://doq.sjlbkw.cn

[B03] switch / match / case
来源：http://wro.yueranfly.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wbj.sysykeji.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ybk.pengpengdd.cyou

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://zsu.kuanghao11.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://fue.hnqzz.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://dgc.yfazqb.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://pzt.xinyue.icu

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hcc.jlsjyb.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hoq.sweek.top

[B04] for 计数循环
来源：http://kbj.zdqjudy.top

Py:   for i in range(10): print(i)
来源：http://dbm.hysaishi.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://fjr.yj20258.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://ocv.316326.xyz

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://amh.cucudq.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://jkd.ybcxt.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hvd.daxiang520.top

Ruby: 10.times { |i| puts i }
来源：http://kfj.zhijiandao.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lqs.redwolf501.top

[B05] 遍历数组 / 列表
来源：http://ieg.sufxvd.cn

Py:   for item in arr: print(item)
来源：http://avv.wangdashe.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://jkc.redwolf501.top

JS:   for (const item of arr) { console.log(item); }
来源：http://gow.tarul.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://laq.hcnkem.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://jpe.andypj.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ydt.fzhhl.top

Ruby: arr.each { |item| puts item }
来源：http://jrr.zhixingplan.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://urt.wangshuangyany.cn

[B06] 遍历字典 / 对象
来源：http://osy.fzhhl.top

Py:   for k, v in d.items(): print(k, v)
来源：http://fht.cdnleiting.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://jnj.chenjidiqi.icu

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dib.jianghu66.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wlr.xuetiantiany.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fmv.zhongyouzk.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://pzj.ydjk.org.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jwl.shanyushiyangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://tar.xuanzx.com

[B07] while 循环
来源：http://lyf.xylfe.cn

Py:   while i < 10: i += 1
来源：http://tzu.zhijiandao.cn

PHP:  while ($i < 10) { $i++; }
来源：http://ggs.sjlbkw.cn

JS:   while (i < 10) { i++; }
来源：http://jol.fengsongda.top

TS:   while (i < 10) { i++; }
来源：http://eyt.hongshengwenyu.top

Java: while (i < 10) { i++; }
来源：http://mtv.gotoacloud.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://nvc.uphjek.com

Ruby: while i < 10; i += 1; end
来源：http://ttj.hnqzz.top

C#:   while (i < 10) { i++; }
来源：http://ncd.tianlin.xyz

[B08] do-while（至少执行一次）
来源：http://oni.iojbl.cn

Py:   # 无 do-while：用 while True + break
来源：http://huw.bjfxy.top

PHP:  do { $i++; } while ($i < 10);
来源：http://xez.gzhubu.top

JS:   do { i++; } while (i < 10);
来源：http://mtx.hesvh.cn

TS:   do { i++; } while (i < 10);
来源：http://sot.daxiang520.top

Java: do { i++; } while (i < 10);
来源：http://wyj.shangyingyoupin.top

Go:   for { i++; if i >= 10 { break } }
来源：http://cun.jinqigfzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://dvf.tian-w.cn

C#:   do { i++; } while (i < 10);
来源：http://ebz.ivvv.top

[B09] break 与 continue
来源：http://gfa.fanxiaobao.xyz

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nlx.0kj1m.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://oxr.sysykeji.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rlk.haohaochexian.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ypv.xinyue.icu

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rec.sxryk.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://qlb.nanxuanxn.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://fce.pengpengdd.cyou

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://szd.ehwqpu.com

[B10] 遍历同时拿索引
来源：http://bql.bbcook.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://opz.yfazqb.com

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ybd.cdnleiting.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://gqe.cucudq.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://npo.yangfankeji.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lty.yanxiufei.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://aid.zhaomingkeji.xyz

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://kyh.zhoulong.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qfx.xuanzx.com

[B11] 生成数字序列 / 区间
来源：http://bmm.meibo888.top

Py:   list(range(0, 10, 2))
来源：http://uus.xziqi.cn

PHP:  range(0, 10, 2);
来源：http://tfh.jinghuilouyu.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nhz.xylfe.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://jyx.daxiang520.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dvy.mhx1999.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tzl.shanyushiyangtech.top

Ruby: (0...10).step(2).to_a
来源：http://obj.ppjwa.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://fwj.kuanghao11.cn

[B12] 跳出多层循环
来源：http://jor.mhx1999.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://qyc.yvedp.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://zus.jqgufenzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jxl.xziqi.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hzs.jlsjyb.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://giz.chenjidiqi.icu

Go:   # 无标签：用布尔标志或抽成函数
来源：http://kzk.ydzc1.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nqv.fengsongda.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://uuy.yj20258.top

[B13] 判断是否为数字
来源：http://ozv.mhx1999.top

Py:   isinstance(x, (int, float))
来源：http://fgy.jqgfzy.top

PHP:  is_numeric($x)
来源：http://wkv.cucudq.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://gwe.yuxming.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://nky.zhiwuduotai.top

Java: x instanceof Number
来源：http://bqp.birdmap.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://oql.sweek.top

Ruby: x.is_a?(Numeric)
来源：http://jpb.jinqigfzy.top

C#:   x is int or double or decimal
来源：http://tcg.sxryk.cn

[B14] 判断值是否在集合内
来源：http://lel.jinqigfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tqc.hnqzz.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://fxn.fanxiaobao.xyz

JS:   [1, 2, 3].includes(x)
来源：http://gii.redwolf501.top

TS:   [1, 2, 3].includes(x)
来源：http://flz.316326.xyz

Java: List.of(1, 2, 3).contains(x)
来源：http://wvo.ywan-chungtsiang.top

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://lgf.ydzc1.top

Ruby: [1, 2, 3].include?(x)
来源：http://kje.fengsongda.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://pzx.dianchejie.cn

[B15] 布尔运算与取反
来源：http://ggb.jinqigufen.top

Py:   a and b or not c
来源：http://hkj.jqgfzy.top

PHP:  $a && $b || !$c
来源：http://mhr.cqqwz.cn

JS:   a && b || !c
来源：http://tmd.yuanzhike.top

TS:   a && b || !c
来源：http://cbg.hcnkem.com

Java: a && b || !c
来源：http://udh.hcnkem.com

Go:   a && b || !c
来源：http://elc.zdqjudy.top

Ruby: a && b || !c
来源：http://ybl.redwolf501.top

C#:   a && b || !c
来源：http://gzm.yvedp.cn

[B16] 卫语句：不满足条件提前返回
来源：http://iuh.zdbjq.cn

Py:   if not data: return
来源：http://xoc.bbcook.cn

PHP:  if (!$data) { return; }
来源：http://yhy.meibo888.top

JS:   if (!data) return;
来源：http://xbh.havefunace.top

TS:   if (!data) return;
来源：http://smb.pengpengdd.cyou

Java: if (data == null) return;
来源：http://wxn.zdqjudy.top

Go:   if data == nil { return }
来源：http://etm.hywenlv.cn

Ruby: return if data.nil?
来源：http://npm.zdqjudy.top

C#:   if (data == null) return;
来源：http://pnt.zhengqikj.top

================================================================================
来源：http://fql.cdnleiting.top

C. 函数与作用域
来源：http://ixx.feifeiyinyue.top

================================================================================
来源：http://byo.yuxming.cn

[C01] 定义函数
来源：http://joz.hywenlv.cn

Py:   def add(a, b): return a + b
来源：http://qpd.cdnleiting.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ewv.c1oappe.top

JS:   function add(a, b) { return a + b; }
来源：http://ipc.cashguo.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gkl.meibo888.top

Java: static int add(int a, int b) { return a + b; }
来源：http://sxb.daria6918.cn

Go:   func add(a, b int) int { return a + b }
来源：http://ybc.sweek.top

Ruby: def add(a, b); a + b; end
来源：http://eew.bjfxy.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cop.hesvh.cn

[C02] 默认参数
来源：http://avb.aibaodan.cn

Py:   def greet(name="World"): return name
来源：http://dlt.sysykeji.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dvi.yvedp.cn

JS:   function greet(name = "World") { return name; }
来源：http://mxv.cqqwz.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://qod.zhongyouzk.top

Java: // 无默认参数：方法重载或 Optional
来源：http://zbu.yueranfly.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cka.guannengcc.top

Ruby: def greet(name = "World") = name
来源：http://jlt.cucudq.cn

C#:   string Greet(string name = "World") => name;
来源：http://lry.hywenlv.cn

[C03] 可变参数
来源：http://adu.zhoulong.xyz

Py:   def total(*args): return sum(args)
来源：http://whz.nanxuanxn.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://uxk.bjfxy.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://rgn.redwolf501.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://pcu.hnqzz.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hcf.zycfv.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://uoo.xingfuxueyuan.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://bxj.nanxinkj.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://ogh.xziqi.cn

[C04] 命名参数 / 关键字参数
来源：http://bus.cdnleiting.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://anl.gogol.net.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://flm.shanyushiyangkeji.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hiv.cdnleiting.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://tvn.jianghu66.top

Java: // 无：用 Builder 模式或 record
来源：http://czf.dianchejie.cn

Go:   // 无：用配置结构体参数
来源：http://dmu.vqdsnc.cn

Ruby: f(a: 1, b: 2)
来源：http://tmv.daria6918.cn

C#:   f(a: 1, b: 2)
来源：http://jwi.shanyushiyangkeji.top

[C05] 返回多个值
来源：http://zjy.gogol.net.cn

Py:   return a, b
来源：http://mmc.yuanzhike.top

PHP:  return [$a, $b];
来源：http://bce.iojbl.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://yyr.hfpthk.cn

TS:   return { a, b };
来源：http://ltb.yvedp.cn


<!-- 参考信息 -->