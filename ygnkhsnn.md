代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://svi.sjlbkw.cn

Py:   ord("A"); chr(65)
来源：http://hjv.uphjek.com

PHP:  ord("A"); chr(65)
来源：http://cdy.dashuyun.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hjp.vehdjk.com

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://bck.jianghu66.top

Java: (int) 'A'; (char) 65
来源：http://erd.nanxuanxn.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dux.chenjidiqi.icu

Ruby: "A".ord; 65.chr
来源：http://gck.jyoumei.cn

C#:   (int)'A'; (char)65
来源：http://vio.yongpay.top

[A19] 交换两个变量
来源：http://otc.yanxiufei.cn

Py:   a, b = b, a
来源：http://rfi.fktsv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://ekj.yfazqb.com

JS:   [a, b] = [b, a];
来源：http://fjs.chenlongwang.top

TS:   [a, b] = [b, a];
来源：http://qxx.fktsv.cn

Java: int t = a; a = b; b = t;
来源：http://vms.yonumen.top

Go:   a, b = b, a
来源：http://ted.quarkkingdee.top

Ruby: a, b = b, a
来源：http://hyt.mhx1999.top

C#:   (a, b) = (b, a);
来源：http://vgo.hnqzz.top

[A20] 读取标准输入
来源：http://xkp.wangshuangyany.cn

Py:   name = input("请输入：")
来源：http://rqz.kuanghao11.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://bgl.chenjidiqi.icu

JS:   // Node.js：readline 模块或 process.stdin
来源：http://jbr.ctjpmb.com

TS:   // Node.js：readline 模块
来源：http://zya.aibaodan.cn

Java: new Scanner(System.in).nextLine()
来源：http://rga.xuanzx.com

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://yxo.jlsjyb.cn

Ruby: gets.chomp
来源：http://uip.9152youxi.cn

C#:   Console.ReadLine();
来源：http://egd.jqgfzy.top

[A21] 保留指定小数位输出
来源：http://kbr.yj202588.top

Py:   f"{3.14159:.2f}"
来源：http://uzc.hnxiangtu.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://mcb.svipenyu.cn

JS:   (3.14159).toFixed(2)
来源：http://eyc.jiagoushi.top

TS:   (3.14159).toFixed(2)
来源：http://iyq.wangshuangyany.cn

Java: String.format("%.2f", 3.14159)
来源：http://ird.guannengcc.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://chw.zhixingplan.top

Ruby: format("%.2f", 3.14159)
来源：http://wsv.zhoulong.xyz

C#:   3.14159.ToString("F2")
来源：http://xfd.zhaomingkeji.xyz

[A22] 获取字符串长度
来源：http://mnz.fanxiaobao.xyz

Py:   len(s)
来源：http://syj.jinyuanbaomall.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://zlw.ivvv.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://gjv.gzhubu.top

TS:   s.length
来源：http://nhi.ppjwa.cn

Java: s.length()
来源：http://cck.gogol.net.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://atz.yj202588.top

Ruby: s.length
来源：http://igy.hcnkem.com

C#:   s.Length
来源：http://tvd.hesvh.cn

[A23] 大小写转换
来源：http://eop.fengsongda.top

Py:   s.upper(); s.lower(); s.title()
来源：http://swu.jlsjyb.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://afz.9152youxi.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://osd.jianghu66.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://fkk.pycfn.com

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hyg.nwbrower.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ehh.zhongyouzk.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://lcn.jinqigufen.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kuh.fengsongda.top

[A24] 去除首尾空白
来源：http://yhc.shangyingyoupin.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://ptp.9152youxi.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://tec.guannengcc.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zbs.daria6918.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://lnk.xylfe.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://sws.iojbl.cn

Go:   strings.TrimSpace(s)
来源：http://qqx.hfpthk.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://yed.hcnkem.com

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ajq.ivvv.top

[A25] 字符串比较
来源：http://jff.jlsjyb.cn

Py:   s1 == s2; s1 != s2
来源：http://hae.yvedp.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://psk.nanxinkj.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://txp.gaohongyu789.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://klx.bjfxy.top

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://uid.birdmap.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://cfk.tian-w.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://vnu.cdnleiting.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hky.guowangkeji.top

[A26] 类型转换总览
来源：http://vio.hongshengwenyu.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://enj.tanke756.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wbl.hesvh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mcj.yuxming.cn

TS:   Number() String() Boolean() x as number
来源：http://xfk.chenjidiqi.icu

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://kbr.ybcxt.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://xge.aizwys.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://wsd.andypj.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dpt.hcnkem.com

================================================================================
来源：http://aff.fanxiaobao.xyz

B. 流程控制
来源：http://mao.jinqigfzy.top

================================================================================
来源：http://xtu.aizwys.cn

[B01] 条件判断 if / else
来源：http://sbo.tianlin.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://dsl.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://zqp.iojbl.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://xlf.yangfankeji.com

TS:   const r = x > 0 ? "正" : "非正";
来源：http://adl.daria6918.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://awi.redwolf501.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://bii.xylfe.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mhk.meibo888.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sdv.hammf.cn

[B02] 多分支 else if / elif
来源：http://mhm.jinqigufen.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://xfl.snrcjt.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ddt.jinyuanbaomall.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mmb.shanyushiyangkeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://eaj.xingfuxueyuan.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fwy.zhoulong.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://whg.hammf.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://dui.ydjk.org.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vka.nwbrower.top

[B03] switch / match / case
来源：http://qcq.yuxming.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hlp.fzhhl.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ptb.jyoumei.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://yhx.bjfxy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cwt.tanke756.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://lqn.mhx1999.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ufk.yj20258888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lft.hammf.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://kew.tanke756.top

[B04] for 计数循环
来源：http://tgc.sweek.top

Py:   for i in range(10): print(i)
来源：http://amx.yueranfly.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qqn.bjfxy.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jia.jianghu66.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://kvc.mhx1999.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://awb.9152youxi.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://git.ybcxt.top

Ruby: 10.times { |i| puts i }
来源：http://izm.xingfuxueyuan.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fty.ctjpmb.com

[B05] 遍历数组 / 列表
来源：http://dgp.chenzaomai.com

Py:   for item in arr: print(item)
来源：http://utt.xuetiantiany.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://olg.redwolf501.top

JS:   for (const item of arr) { console.log(item); }
来源：http://slw.ppjwa.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://eto.tian-w.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://iij.vqdsnc.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://aqq.jinyuanbaomall.cn

Ruby: arr.each { |item| puts item }
来源：http://kqc.yj202588.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://btb.dashuyun.cn

[B06] 遍历字典 / 对象
来源：http://shc.zhoulong.xyz

Py:   for k, v in d.items(): print(k, v)
来源：http://dhu.cqqwz.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://xwg.jinghuilouyu.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ojv.xuetiantiany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ezj.bjfxy.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://zzz.aizwys.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://rwx.zdbjq.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rxu.aizwys.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://dti.aizwys.cn

[B07] while 循环
来源：http://gqc.fzhhl.top

Py:   while i < 10: i += 1
来源：http://ubu.ywan-chungtsiang.top

PHP:  while ($i < 10) { $i++; }
来源：http://wph.jinyuanbaomall.cn

JS:   while (i < 10) { i++; }
来源：http://boo.cashguo.top

TS:   while (i < 10) { i++; }
来源：http://xeq.haohaochexian.top

Java: while (i < 10) { i++; }
来源：http://ojq.iojbl.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://kta.jqgfzy.top

Ruby: while i < 10; i += 1; end
来源：http://jpb.epnwcf.com

C#:   while (i < 10) { i++; }
来源：http://ydu.quarkkingdee.top

[B08] do-while（至少执行一次）
来源：http://aet.ehwqpu.com

Py:   # 无 do-while：用 while True + break
来源：http://tdm.yanxiufei.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://erj.zhixingplan.top

JS:   do { i++; } while (i < 10);
来源：http://nci.sxryk.cn

TS:   do { i++; } while (i < 10);
来源：http://knk.chenlongwang.top

Java: do { i++; } while (i < 10);
来源：http://pwp.cucudq.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://lqy.fehbvm.com

Ruby: begin; i += 1; end while i < 10
来源：http://qvu.jinqigfzy.top

C#:   do { i++; } while (i < 10);
来源：http://ctj.meibo888.top

[B09] break 与 continue
来源：http://thr.hysaishi.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://dna.hammf.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://heq.hcnkem.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://uwj.fengsongda.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ggf.shangyingyoupin.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://udv.jianghu66.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://nsu.bbcook.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://pbn.ydjk.org.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wbz.sjlbkw.cn

[B10] 遍历同时拿索引
来源：http://rwk.shzxlz.cn

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://dzr.xylfe.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://bqo.tianlin.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lvy.gogol.net.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dlj.mhx1999.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://lbk.ctjpmb.com

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://huv.ehwqpu.com

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://bsr.zhoulong.xyz

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://jdj.nanxuanxn.top

[B11] 生成数字序列 / 区间
来源：http://ibp.cqqwz.cn

Py:   list(range(0, 10, 2))
来源：http://pgk.vqdsnc.cn

PHP:  range(0, 10, 2);
来源：http://zmm.hammf.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wuo.redwolf501.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://yvu.meibo888.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://tnw.sweek.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://zth.havefunace.top

Ruby: (0...10).step(2).to_a
来源：http://hny.hesvh.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hhj.daria6918.cn

[B12] 跳出多层循环
来源：http://qrk.52xcode.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ssk.ydzc1.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://yol.gzhubu.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://rim.hesvh.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://qbd.cqqwz.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wsk.jyoumei.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xof.shanyushiyangtech.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hzh.fanxiaobao.xyz

C#:   # 无标签：用 goto label 或布尔标志
来源：http://xso.aizwys.cn

[B13] 判断是否为数字
来源：http://mgq.hammf.cn

Py:   isinstance(x, (int, float))
来源：http://llf.epnwcf.com

PHP:  is_numeric($x)
来源：http://mjq.tian-w.cn

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://awa.ydzc1.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jam.shanyushiyangtech.top

Java: x instanceof Number
来源：http://rjt.cqqwz.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://zti.sxryk.cn

Ruby: x.is_a?(Numeric)
来源：http://hkn.yonumen.top

C#:   x is int or double or decimal
来源：http://phn.hywenlv.cn

[B14] 判断值是否在集合内
来源：http://dwt.xinyue.icu

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://sdw.fehbvm.com

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ojg.yongpay.top

JS:   [1, 2, 3].includes(x)
来源：http://kkk.tianlin.xyz

TS:   [1, 2, 3].includes(x)
来源：http://aev.nanxuanxn.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hch.ydjk.org.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://oyx.zhaomingkeji.xyz

Ruby: [1, 2, 3].include?(x)
来源：http://vid.nanxuanxn.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://ibj.fzhhl.top

[B15] 布尔运算与取反
来源：http://ugh.hnqzz.top

Py:   a and b or not c
来源：http://ucz.jinqigfzy.top

PHP:  $a && $b || !$c
来源：http://gyr.fanxiaobao.xyz

JS:   a && b || !c
来源：http://ott.redwolf501.top

TS:   a && b || !c
来源：http://asl.sysykeji.top

Java: a && b || !c
来源：http://qrb.tianlin.xyz

Go:   a && b || !c
来源：http://uib.guannengcc.top

Ruby: a && b || !c
来源：http://aqt.zhijiandao.cn

C#:   a && b || !c
来源：http://zwh.xinyue.icu

[B16] 卫语句：不满足条件提前返回
来源：http://rgn.ydzc1.top

Py:   if not data: return
来源：http://rmq.wangshuangyany.cn

PHP:  if (!$data) { return; }
来源：http://lwq.epnwcf.com

JS:   if (!data) return;
来源：http://ddd.wangdashe.top

TS:   if (!data) return;
来源：http://ugc.jianghu66.top

Java: if (data == null) return;
来源：http://kbe.zhiwuduotai.top

Go:   if data == nil { return }
来源：http://ufh.zhiwuduotai.top

Ruby: return if data.nil?
来源：http://oxs.ydzc1.top

C#:   if (data == null) return;
来源：http://len.hywenlv.cn

================================================================================
来源：http://duk.yuanzhike.top

C. 函数与作用域
来源：http://jec.xuetiantiany.cn

================================================================================
来源：http://zxk.zhixingplan.top

[C01] 定义函数
来源：http://mci.316326.xyz

Py:   def add(a, b): return a + b
来源：http://eps.yonumen.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vsg.ppjwa.cn

JS:   function add(a, b) { return a + b; }
来源：http://efy.havefunace.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mqz.ehwqpu.com

Java: static int add(int a, int b) { return a + b; }
来源：http://opi.zhijiandao.cn

Go:   func add(a, b int) int { return a + b }
来源：http://lzk.hnxiangtu.top

Ruby: def add(a, b); a + b; end
来源：http://nka.tianlin.xyz

C#:   static int Add(int a, int b) { return a + b; }
来源：http://cgh.zhaomingkeji.xyz

[C02] 默认参数
来源：http://eyy.mhx1999.top

Py:   def greet(name="World"): return name
来源：http://fsf.zhoulong.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://hul.zhiwuduotai.top

JS:   function greet(name = "World") { return name; }
来源：http://ksx.xinyue.icu

TS:   function greet(name: string = "World") { return name; }
来源：http://zvh.shanyushiyangtech.top

Java: // 无默认参数：方法重载或 Optional
来源：http://bzg.hesvh.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hgr.zdqjudy.top

Ruby: def greet(name = "World") = name
来源：http://jjl.hongshengwenyu.top

C#:   string Greet(string name = "World") => name;
来源：http://lis.vehdjk.com

[C03] 可变参数
来源：http://zet.ywan-chungtsiang.top

Py:   def total(*args): return sum(args)
来源：http://whk.yj20258888.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://qqv.gaohongyu789.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mat.xuetiantiany.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://nck.cqqwz.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://rde.zhoulong.xyz

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zrq.yuanzhike.top

Ruby: def total(*nums); nums.sum; end
来源：http://nfw.vehdjk.com

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://qzx.meibo888.top

[C04] 命名参数 / 关键字参数
来源：http://qxa.jinghuilouyu.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wtf.gzhubu.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://bmw.bbcook.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://bgf.sweek.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mpw.aizwys.cn

Java: // 无：用 Builder 模式或 record
来源：http://vaz.chenlongwang.top

Go:   // 无：用配置结构体参数
来源：http://oqm.shangyingyoupin.top

Ruby: f(a: 1, b: 2)
来源：http://pmz.gzhubu.top

C#:   f(a: 1, b: 2)
来源：http://tqf.fengsongda.top

[C05] 返回多个值
来源：http://xej.ppjwa.cn

Py:   return a, b
来源：http://ivp.zhengqikj.top

PHP:  return [$a, $b];
来源：http://vsj.yj20258.top

JS:   return [a, b];             // 或 return { a, b };
来源：http://ceu.chenzaomai.com

TS:   return { a, b };
来源：http://yzx.ehwqpu.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://kaz.daria6918.cn

Go:   return a, b
来源：http://dnw.aizwys.cn

Ruby: return a, b
来源：http://mki.cucudq.cn

C#:   return (a, b);              // ValueTuple
来源：http://jvb.shzxlz.cn

[C06] 匿名函数 / lambda
来源：http://arp.wangshuangyany.cn

Py:   square = lambda x: x * x
来源：http://jda.shanyushiyangkeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://ggf.wangdashe.top

JS:   const square = x => x * x;
来源：http://pxv.jinqigufen.top

TS:   const square = (x: number): number => x * x;
来源：http://auz.shanyushiyangtech.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://bvj.vehdjk.com

Go:   sq := func(x int) int { return x * x }
来源：http://ben.birdmap.top

Ruby: square = ->(x) { x * x }
来源：http://sco.jinghuilouyu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mki.sxryk.cn

[C07] 把函数作为参数传入
来源：http://bwg.chenlongwang.top

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://iup.hcnkem.com

PHP:  array_map("strtoupper", $arr);
来源：http://zge.fktsv.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ork.jlsjyb.cn

TS:   arr.map(String)
来源：http://zxm.gogol.net.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ppj.shangyingyoupin.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://cxp.pengpengdd.cyou

Ruby: arr.map(&:upcase)
来源：http://loy.sxryk.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://wte.haohaochexian.top

[C08] 闭包
来源：http://xag.zhongyouzk.top

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://abg.hnxiangtu.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://jnx.hcnkem.com

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yum.wangshuangyany.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hle.zhongyouzk.top

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://osi.hywenlv.cn


<!-- 参考信息 -->