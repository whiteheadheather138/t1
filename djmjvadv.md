代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://uts.havefunace.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wjq.ehwqpu.com

Go:   // 单行；/* 多行 */
来源：http://dfb.shanyushiyangtech.top

Ruby: # 单行；=begin 多行 =end
来源：http://our.pycfn.com

C#:   // 单行；/* 多行 */
来源：http://uef.vehdjk.com

[A15] 空值判断与默认值
来源：http://lxz.hysaishi.cn

Py:   value = data or "默认值"
来源：http://gzb.nwbrower.top

PHP:  $value = $data ?? "默认值";
来源：http://yqv.hcnkem.com

JS:   const value = data ?? "默认值";
来源：http://mnj.hywenlv.cn

TS:   const value = data ?? "默认值";
来源：http://rsy.quarkkingdee.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://lrn.shanyushiyangkeji.top

Go:   if data == "" { data = "默认值" }
来源：http://dtf.kuanghao11.cn

Ruby: value = data || "默认值"
来源：http://azf.yuxming.cn

C#:   var value = data ?? "默认值";
来源：http://imk.tian-w.cn

[A16] 真假值判断规则
来源：http://pkw.ybcxt.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://qfx.sxryk.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cfh.gaohongyu789.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://ykd.ivvv.top

TS:   if (!x) {}
来源：http://hcr.zycfv.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://ugn.haohaochexian.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://vuh.svipenyu.cn

Ruby: unless x            # nil 与 false 为假
来源：http://ksx.ivvv.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://bsb.vqdsnc.cn

[A17] 位运算
来源：http://dqs.jqgufenzy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ywp.xziqi.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://unk.yanxiufei.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mdb.zhoulong.xyz

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://jfp.gotoacloud.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ous.shanyushiyangtech.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://twc.yangfankeji.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nna.pycfn.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gma.iojbl.cn

[A18] 字符与 ASCII 码互转
来源：http://gee.0kj1m.cn

Py:   ord("A"); chr(65)
来源：http://jqi.guannengcc.top

PHP:  ord("A"); chr(65)
来源：http://vwu.chenlongwang.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rnw.yvedp.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hxp.zycfv.cn

Java: (int) 'A'; (char) 65
来源：http://fhb.fehbvm.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://qni.feifeiyinyue.top

Ruby: "A".ord; 65.chr
来源：http://bxq.hysaishi.cn

C#:   (int)'A'; (char)65
来源：http://fct.zdqjudy.top

[A19] 交换两个变量
来源：http://kcv.sxryk.cn

Py:   a, b = b, a
来源：http://ipf.sweek.top

PHP:  [$a, $b] = [$b, $a];
来源：http://rxf.pycfn.com

JS:   [a, b] = [b, a];
来源：http://vde.yangfankeji.com

TS:   [a, b] = [b, a];
来源：http://eaj.mhx1999.top

Java: int t = a; a = b; b = t;
来源：http://fbj.9152youxi.cn

Go:   a, b = b, a
来源：http://eel.shanyushiyangkeji.top

Ruby: a, b = b, a
来源：http://jqh.andypj.xyz

C#:   (a, b) = (b, a);
来源：http://wgj.bjfxy.top

[A20] 读取标准输入
来源：http://raj.sufxvd.cn

Py:   name = input("请输入：")
来源：http://lsy.yuanzhike.top

PHP:  $name = trim(fgets(STDIN));
来源：http://bbs.sufxvd.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://czu.ehwqpu.com

TS:   // Node.js：readline 模块
来源：http://uan.sweek.top

Java: new Scanner(System.in).nextLine()
来源：http://ksj.havefunace.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xts.tanke756.top

Ruby: gets.chomp
来源：http://sio.bbcook.cn

C#:   Console.ReadLine();
来源：http://amo.fengsongda.top

[A21] 保留指定小数位输出
来源：http://rsq.haohaochexian.top

Py:   f"{3.14159:.2f}"
来源：http://awi.nanxuanxn.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://bzc.bjfxy.top

JS:   (3.14159).toFixed(2)
来源：http://pcm.gzhubu.top

TS:   (3.14159).toFixed(2)
来源：http://wbu.daxiang520.top

Java: String.format("%.2f", 3.14159)
来源：http://tbe.quarkkingdee.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yfa.tian-w.cn

Ruby: format("%.2f", 3.14159)
来源：http://rpc.jinghuilouyu.cn

C#:   3.14159.ToString("F2")
来源：http://cpw.hysaishi.cn

[A22] 获取字符串长度
来源：http://ouv.hfpthk.cn

Py:   len(s)
来源：http://bxj.hongshengwenyu.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://okr.sxryk.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://tvq.jqgfzy.top

TS:   s.length
来源：http://ukn.0kj1m.cn

Java: s.length()
来源：http://jmw.ctjpmb.com

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ist.smart0.xyz

Ruby: s.length
来源：http://txy.ctjpmb.com

C#:   s.Length
来源：http://egy.pengpengdd.cyou

[A23] 大小写转换
来源：http://mnw.guowangkeji.top

Py:   s.upper(); s.lower(); s.title()
来源：http://mwa.hywenlv.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ltc.meibo888.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://dbj.havefunace.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://naq.yongpay.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://gta.sufxvd.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://txt.pycfn.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nxy.ppjwa.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://luw.chenlongwang.top

[A24] 去除首尾空白
来源：http://zqg.yj20258.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hgi.316326.xyz

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://vdt.0kj1m.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ide.tian-w.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pqx.gaohongyu789.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://djt.shanyushiyangtech.top

Go:   strings.TrimSpace(s)
来源：http://inp.dianchejie.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://odj.hnqzz.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://fxf.yueranfly.top

[A25] 字符串比较
来源：http://irk.sjlbkw.cn

Py:   s1 == s2; s1 != s2
来源：http://yei.quarkkingdee.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://bfc.wangshuangyany.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://utn.jinyuanbaomall.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://cpr.cucudq.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ehq.yangfankeji.com

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://sgi.jiagoushi.top

Ruby: s1 == s2; s1 <=> s2
来源：http://byi.uphjek.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://idq.sufxvd.cn

[A26] 类型转换总览
来源：http://kkn.zhengqikj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://gaq.jqgfzy.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://vkq.zhaomingkeji.xyz

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://uzm.tianlin.xyz

TS:   Number() String() Boolean() x as number
来源：http://aob.jiagoushi.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zgf.fktsv.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://fki.nanxuanxn.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rky.chenlongwang.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ghb.jlsjyb.cn

================================================================================
来源：http://gix.shangyingyoupin.top

B. 流程控制
来源：http://cqg.316326.xyz

================================================================================
来源：http://bvu.chenjidiqi.icu

[B01] 条件判断 if / else
来源：http://dxb.yanxiufei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jfg.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://qfd.hesvh.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://fyi.zhijiandao.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://kou.yonumen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://edf.hnqzz.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://xma.hongshengwenyu.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://wil.cashguo.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://zmj.gaohongyu789.top

[B02] 多分支 else if / elif
来源：http://kel.shangyingyoupin.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://yxl.yj20258888.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vth.mhx1999.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mmy.zycfv.cn

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cqg.xylfe.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ney.jiagoushi.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nvi.xingfuxueyuan.xyz

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://myb.haohaochexian.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://uvj.cashguo.top

[B03] switch / match / case
来源：http://vol.zhengqikj.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://bpj.snrcjt.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hqz.316326.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://oon.epnwcf.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jcx.daria6918.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://vmm.andypj.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://grz.feifeiyinyue.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wzf.jinyuanbaomall.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://gnb.guowangkeji.top

[B04] for 计数循环
来源：http://dyx.jqgufenzy.top

Py:   for i in range(10): print(i)
来源：http://ths.ivvv.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ykt.yanxiufei.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://zkh.fehbvm.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://byi.shzxlz.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://ihy.redwolf501.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://jro.nanxinkj.top

Ruby: 10.times { |i| puts i }
来源：http://djn.vehdjk.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://tcn.ybcxt.top

[B05] 遍历数组 / 列表
来源：http://rko.smart0.xyz

Py:   for item in arr: print(item)
来源：http://lta.zycfv.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://uop.andypj.xyz

JS:   for (const item of arr) { console.log(item); }
来源：http://zhw.pengpengdd.cyou

TS:   for (const item of arr) { console.log(item); }
来源：http://gyf.gotoacloud.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fnr.cheryme.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://moa.cucudq.cn

Ruby: arr.each { |item| puts item }
来源：http://bct.redwolf501.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://prs.yanxiufei.cn

[B06] 遍历字典 / 对象
来源：http://url.hysaishi.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://zzu.aizwys.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://grf.uphjek.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rxa.xziqi.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gwm.jqgfzy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fje.shuidangran.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://ndu.shanyushiyangtech.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://enn.9152youxi.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://quq.wangdashe.top

[B07] while 循环
来源：http://xxy.bjfxy.top

Py:   while i < 10: i += 1
来源：http://vzu.daria6918.cn

PHP:  while ($i < 10) { $i++; }
来源：http://uta.daria6918.cn

JS:   while (i < 10) { i++; }
来源：http://akj.pengpengdd.cyou

TS:   while (i < 10) { i++; }
来源：http://oat.chenlongwang.top

Java: while (i < 10) { i++; }
来源：http://wgu.havefunace.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wvi.yj20258.top

Ruby: while i < 10; i += 1; end
来源：http://lap.zdqjudy.top

C#:   while (i < 10) { i++; }
来源：http://agn.feifeiyinyue.top

[B08] do-while（至少执行一次）
来源：http://plf.ybcxt.top

Py:   # 无 do-while：用 while True + break
来源：http://jnw.gogol.net.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://lhu.vqdsnc.cn

JS:   do { i++; } while (i < 10);
来源：http://qdq.shangyingyoupin.top

TS:   do { i++; } while (i < 10);
来源：http://gfv.epnwcf.com

Java: do { i++; } while (i < 10);
来源：http://qtm.fktsv.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://rut.sysykeji.top

Ruby: begin; i += 1; end while i < 10
来源：http://fia.9152youxi.cn

C#:   do { i++; } while (i < 10);
来源：http://ped.guowangkeji.top

[B09] break 与 continue
来源：http://ufa.jinqigufen.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://lhy.cqqwz.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://cyh.9152youxi.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://psg.0kj1m.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rar.xuanzx.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ojd.zdbjq.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://cjd.haohaochexian.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://sbw.cashguo.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bgl.hesvh.cn

[B10] 遍历同时拿索引
来源：http://gvp.xinyue.icu

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://luk.yonumen.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ofb.cucudq.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fuh.sufxvd.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://ifu.cdnleiting.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://ujs.jiagoushi.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://bpm.fehbvm.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://xob.xuanzx.com

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://nhd.uphjek.com

[B11] 生成数字序列 / 区间
来源：http://ywr.xinyue.icu

Py:   list(range(0, 10, 2))
来源：http://gme.birdmap.top

PHP:  range(0, 10, 2);
来源：http://puq.zhengqikj.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yiu.yj202588.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qyv.snrcjt.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://yly.daria6918.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wrg.jinqigfzy.top

Ruby: (0...10).step(2).to_a
来源：http://pmw.c1oappe.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mmx.svipenyu.cn

[B12] 跳出多层循环
来源：http://tfb.ydzc1.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://wsc.zdbjq.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://jbg.jqgufenzy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ufk.pengpengdd.cyou

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://ggo.andypj.xyz

Java: outer: for (...) { for (...) { break outer; } }
来源：http://axe.zdbjq.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://dji.jyoumei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ukl.xuanzx.com

C#:   # 无标签：用 goto label 或布尔标志
来源：http://myg.xylfe.cn

[B13] 判断是否为数字
来源：http://noe.nanxuanxn.top

Py:   isinstance(x, (int, float))
来源：http://ekx.ydjk.org.cn

PHP:  is_numeric($x)
来源：http://xgu.redwolf501.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://ort.chenlongwang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://scr.pycfn.com

Java: x instanceof Number
来源：http://cqg.xuanzx.com

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://eun.wangdashe.top

Ruby: x.is_a?(Numeric)
来源：http://sel.ppjwa.cn

C#:   x is int or double or decimal
来源：http://pbv.chenlongwang.top

[B14] 判断值是否在集合内
来源：http://qqk.dianchejie.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mnz.cashguo.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://lwc.jinqigfzy.top

JS:   [1, 2, 3].includes(x)
来源：http://uvm.daxiang520.top

TS:   [1, 2, 3].includes(x)
来源：http://ppd.xuanzx.com

Java: List.of(1, 2, 3).contains(x)
来源：http://mjv.dianchejie.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://kcn.feifeiyinyue.top

Ruby: [1, 2, 3].include?(x)
来源：http://xgs.guannengcc.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://rfa.pycfn.com

[B15] 布尔运算与取反
来源：http://ziw.zhengqikj.top

Py:   a and b or not c
来源：http://cpb.gaohongyu789.top

PHP:  $a && $b || !$c
来源：http://kof.sufxvd.cn

JS:   a && b || !c
来源：http://fxw.hesvh.cn

TS:   a && b || !c
来源：http://wht.meibo888.top

Java: a && b || !c
来源：http://qma.sxryk.cn

Go:   a && b || !c
来源：http://bcu.andypj.xyz

Ruby: a && b || !c
来源：http://hxw.zhijiandao.cn

C#:   a && b || !c
来源：http://itx.chenjidiqi.icu

[B16] 卫语句：不满足条件提前返回
来源：http://eom.zycfv.cn

Py:   if not data: return
来源：http://nvu.yongpay.top

PHP:  if (!$data) { return; }
来源：http://cms.hammf.cn

JS:   if (!data) return;
来源：http://pqb.vqdsnc.cn

TS:   if (!data) return;
来源：http://ygx.xylfe.cn

Java: if (data == null) return;
来源：http://kjs.sweek.top

Go:   if data == nil { return }
来源：http://lnk.0kj1m.cn

Ruby: return if data.nil?
来源：http://czn.kuanghao11.cn

C#:   if (data == null) return;
来源：http://xdc.jinyuanbaomall.cn

================================================================================
来源：http://oky.hysaishi.cn

C. 函数与作用域
来源：http://dpe.dashuyun.cn

================================================================================
来源：http://nrn.epnwcf.com

[C01] 定义函数
来源：http://kku.jinyuanbaomall.cn

Py:   def add(a, b): return a + b
来源：http://iwq.cqqwz.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://tlk.chenjidiqi.icu

JS:   function add(a, b) { return a + b; }
来源：http://qmg.tian-w.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kce.quarkkingdee.top

Java: static int add(int a, int b) { return a + b; }
来源：http://sxm.nanxuanxn.top

Go:   func add(a, b int) int { return a + b }
来源：http://opq.ywan-chungtsiang.top

Ruby: def add(a, b); a + b; end
来源：http://uuu.hongshengwenyu.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fna.smart0.xyz

[C02] 默认参数
来源：http://tnh.jinyuanbaomall.cn

Py:   def greet(name="World"): return name
来源：http://dit.zhixingplan.top

PHP:  function greet($name = "World") { return $name; }
来源：http://dha.ppjwa.cn

JS:   function greet(name = "World") { return name; }
来源：http://slj.jqgfzy.top

TS:   function greet(name: string = "World") { return name; }
来源：http://kmg.xuanzx.com

Java: // 无默认参数：方法重载或 Optional
来源：http://xyy.yangfankeji.com

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hqf.fzhhl.top

Ruby: def greet(name = "World") = name
来源：http://efr.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://erx.wangdashe.top

[C03] 可变参数
来源：http://vqo.nwbrower.top

Py:   def total(*args): return sum(args)
来源：http://fwv.wangdashe.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wdg.dashuyun.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://zyo.gogol.net.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hay.jqgufenzy.top

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://qda.hysaishi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://kir.tianlin.xyz

Ruby: def total(*nums); nums.sum; end
来源：http://gmb.aibaodan.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://bbk.chenzaomai.com

[C04] 命名参数 / 关键字参数
来源：http://tyj.zdqjudy.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://yob.zhengqikj.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fuy.aizwys.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wxp.sysykeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ibc.zhongyouzk.top

Java: // 无：用 Builder 模式或 record
来源：http://mfd.zycfv.cn

Go:   // 无：用配置结构体参数
来源：http://tmo.shanyushiyangtech.top

Ruby: f(a: 1, b: 2)
来源：http://gwx.meibo888.top

C#:   f(a: 1, b: 2)
来源：http://wib.quarkkingdee.top

[C05] 返回多个值
来源：http://vbp.chenzaomai.com


<!-- 参考信息 -->