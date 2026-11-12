代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://cyr.sxryk.cn

Py:   ord("A"); chr(65)
来源：http://nvt.316326.xyz

PHP:  ord("A"); chr(65)
来源：http://nsm.yanxiufei.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xvd.havefunace.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://sfs.ywan-chungtsiang.top

Java: (int) 'A'; (char) 65
来源：http://sdg.andypj.xyz

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://dye.zhiwuduotai.top

Ruby: "A".ord; 65.chr
来源：http://yow.jyoumei.cn

C#:   (int)'A'; (char)65
来源：http://abs.redwolf501.top

[A19] 交换两个变量
来源：http://tll.hongshengwenyu.top

Py:   a, b = b, a
来源：http://vst.ppjwa.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://viz.chenlongwang.top

JS:   [a, b] = [b, a];
来源：http://fvf.cashguo.top

TS:   [a, b] = [b, a];
来源：http://hkn.sxryk.cn

Java: int t = a; a = b; b = t;
来源：http://pip.jlsjyb.cn

Go:   a, b = b, a
来源：http://jwe.hesvh.cn

Ruby: a, b = b, a
来源：http://bxi.wangshuangyany.cn

C#:   (a, b) = (b, a);
来源：http://uiz.cdnleiting.top

[A20] 读取标准输入
来源：http://lup.jinyuanbaomall.cn

Py:   name = input("请输入：")
来源：http://nfb.xingfuxueyuan.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://yts.xingfuxueyuan.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://gqd.vqdsnc.cn

TS:   // Node.js：readline 模块
来源：http://rcu.fengsongda.top

Java: new Scanner(System.in).nextLine()
来源：http://oyo.wangshuangyany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://xwt.havefunace.top

Ruby: gets.chomp
来源：http://qtn.wangdashe.top

C#:   Console.ReadLine();
来源：http://rib.vehdjk.com

[A21] 保留指定小数位输出
来源：http://kpn.jinqigfzy.top

Py:   f"{3.14159:.2f}"
来源：http://tjw.zycfv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://srz.yanxiufei.cn

JS:   (3.14159).toFixed(2)
来源：http://txq.jiagoushi.top

TS:   (3.14159).toFixed(2)
来源：http://ggd.chenlongwang.top

Java: String.format("%.2f", 3.14159)
来源：http://ziu.bjfxy.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://nwe.tanke756.top

Ruby: format("%.2f", 3.14159)
来源：http://osl.uphjek.com

C#:   3.14159.ToString("F2")
来源：http://fry.hnqzz.top

[A22] 获取字符串长度
来源：http://ecr.guowangkeji.top

Py:   len(s)
来源：http://llo.sufxvd.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://bbv.gaohongyu789.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://eeo.shzxlz.cn

TS:   s.length
来源：http://yfd.cucudq.cn

Java: s.length()
来源：http://gmp.birdmap.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://oqf.ybcxt.top

Ruby: s.length
来源：http://aqz.shzxlz.cn

C#:   s.Length
来源：http://ymn.andypj.xyz

[A23] 大小写转换
来源：http://qrp.fktsv.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://zms.jlsjyb.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://uih.hnxiangtu.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rux.smart0.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://aax.daxiang520.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jus.jinghuilouyu.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ktz.jyoumei.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://knx.yangfankeji.com

C#:   s.ToUpper(); s.ToLower()
来源：http://uoz.sweek.top

[A24] 去除首尾空白
来源：http://myj.ydjk.org.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://siq.jinqigufen.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://axi.sufxvd.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://evv.jinqigfzy.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gtk.xuetiantiany.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://bbw.52xcode.cn

Go:   strings.TrimSpace(s)
来源：http://gwj.zdqjudy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gog.redwolf501.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hwa.shuidangran.top

[A25] 字符串比较
来源：http://zsb.epnwcf.com

Py:   s1 == s2; s1 != s2
来源：http://vfz.hywenlv.cn

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://pnv.jianghu66.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://zie.shanyushiyangkeji.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mwf.xziqi.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://zkw.zdbjq.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://gtb.havefunace.top

Ruby: s1 == s2; s1 <=> s2
来源：http://shu.bbcook.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://igj.quarkkingdee.top

[A26] 类型转换总览
来源：http://whf.jyoumei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://cec.gogol.net.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mme.hnqzz.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qtt.cdnleiting.top

TS:   Number() String() Boolean() x as number
来源：http://ctp.shzxlz.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ubs.hongshengwenyu.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://evl.hnqzz.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://cjj.xinyue.icu

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://xfa.ydzc1.top

================================================================================
来源：http://mge.cheryme.top

B. 流程控制
来源：http://oju.wangshuangyany.cn

================================================================================
来源：http://xgm.dianchejie.cn

[B01] 条件判断 if / else
来源：http://bal.pengpengdd.cyou

Py:   result = "正" if x > 0 else "非正"
来源：http://cpf.shanyushiyangkeji.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://cbe.hywenlv.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://zvh.havefunace.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://qyw.wangshuangyany.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://fav.nwbrower.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wlo.sysykeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://apk.chenzaomai.com

C#:   var r = x > 0 ? "正" : "非正";
来源：http://drd.ybcxt.top

[B02] 多分支 else if / elif
来源：http://nch.smart0.xyz

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://mvz.svipenyu.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://fid.yfazqb.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zey.gotoacloud.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://qar.316326.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://rjt.yueranfly.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://kxc.daxiang520.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://oin.jinqigufen.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://gox.sweek.top

[B03] switch / match / case
来源：http://qth.hfpthk.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://twz.yuxming.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://qfx.andypj.xyz

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://noz.ppjwa.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mai.yanxiufei.cn

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://ppm.xuanzx.com

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://qvd.yj202588.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://lmv.zhaomingkeji.xyz

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://iih.yvedp.cn

[B04] for 计数循环
来源：http://gnm.cucudq.cn

Py:   for i in range(10): print(i)
来源：http://pfj.zhiwuduotai.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://qmu.redwolf501.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sqi.ydjk.org.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://cfb.hnqzz.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bcn.daria6918.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://tdy.uphjek.com

Ruby: 10.times { |i| puts i }
来源：http://ghi.tanke756.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://aae.guowangkeji.top

[B05] 遍历数组 / 列表
来源：http://ryp.cashguo.top

Py:   for item in arr: print(item)
来源：http://fhv.zhaomingkeji.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://krj.zhiwuduotai.top

JS:   for (const item of arr) { console.log(item); }
来源：http://jex.shangyingyoupin.top

TS:   for (const item of arr) { console.log(item); }
来源：http://whf.pycfn.com

Java: for (var item : arr) { System.out.println(item); }
来源：http://qol.sjlbkw.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mbu.fehbvm.com

Ruby: arr.each { |item| puts item }
来源：http://zga.ydjk.org.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://uxe.hnqzz.top

[B06] 遍历字典 / 对象
来源：http://tkw.gzhubu.top

Py:   for k, v in d.items(): print(k, v)
来源：http://okj.svipenyu.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://qax.chenzaomai.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dau.jyoumei.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wwx.jinyuanbaomall.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://uuk.c1oappe.top

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://sal.zhaomingkeji.xyz

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://prj.snrcjt.cn

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://pvc.quarkkingdee.top

[B07] while 循环
来源：http://ofx.hongshengwenyu.top

Py:   while i < 10: i += 1
来源：http://hxq.zhoulong.xyz

PHP:  while ($i < 10) { $i++; }
来源：http://dou.yj202588.top

JS:   while (i < 10) { i++; }
来源：http://wdr.smart0.xyz

TS:   while (i < 10) { i++; }
来源：http://orc.fengsongda.top

Java: while (i < 10) { i++; }
来源：http://bht.jqgfzy.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aip.yvedp.cn

Ruby: while i < 10; i += 1; end
来源：http://zia.gogol.net.cn

C#:   while (i < 10) { i++; }
来源：http://fgt.aibaodan.cn

[B08] do-while（至少执行一次）
来源：http://fjo.52xcode.cn

Py:   # 无 do-while：用 while True + break
来源：http://ggr.xuetiantiany.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://gyr.kuanghao11.cn

JS:   do { i++; } while (i < 10);
来源：http://piu.haohaochexian.top

TS:   do { i++; } while (i < 10);
来源：http://ksi.zdbjq.cn

Java: do { i++; } while (i < 10);
来源：http://zko.vqdsnc.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://hxo.cucudq.cn

Ruby: begin; i += 1; end while i < 10
来源：http://rlh.yangfankeji.com

C#:   do { i++; } while (i < 10);
来源：http://kgd.shanyushiyangkeji.top

[B09] break 与 continue
来源：http://bqc.kuanghao11.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://gqh.ctjpmb.com

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://gdh.gzhubu.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ujk.ppjwa.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mxa.jinghuilouyu.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jwj.hnqzz.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://jxp.0kj1m.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://uuf.tian-w.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://gbm.yonumen.top

[B10] 遍历同时拿索引
来源：http://lty.gaohongyu789.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bfb.meibo888.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://tyi.gogol.net.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://ttt.ivvv.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://fic.chenzaomai.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://xyl.vqdsnc.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zyf.yvedp.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://epn.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://uss.snrcjt.cn

[B11] 生成数字序列 / 区间
来源：http://ifv.xuanzx.com

Py:   list(range(0, 10, 2))
来源：http://qhk.316326.xyz

PHP:  range(0, 10, 2);
来源：http://xof.jinqigufen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nyt.shangyingyoupin.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://uen.fengsongda.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ohv.andypj.xyz

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://tct.iojbl.cn

Ruby: (0...10).step(2).to_a
来源：http://zuw.yuxming.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nzo.tarul.cn

[B12] 跳出多层循环
来源：http://faq.xuetiantiany.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://gmy.gogol.net.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://qvx.dianchejie.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://jus.yanxiufei.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://rlf.ppjwa.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mhd.xuanzx.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://cya.jlsjyb.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ncl.zdbjq.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hfa.feifeiyinyue.top

[B13] 判断是否为数字
来源：http://sda.redwolf501.top

Py:   isinstance(x, (int, float))
来源：http://xaf.yonumen.top

PHP:  is_numeric($x)
来源：http://yol.jinqigufen.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://jgl.zdqjudy.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://xxo.xziqi.cn

Java: x instanceof Number
来源：http://rgh.xuetiantiany.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://vru.fengsongda.top

Ruby: x.is_a?(Numeric)
来源：http://afn.yueranfly.top

C#:   x is int or double or decimal
来源：http://atv.xuetiantiany.cn

[B14] 判断值是否在集合内
来源：http://god.daxiang520.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://jxd.ydzc1.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://sks.hammf.cn

JS:   [1, 2, 3].includes(x)
来源：http://nzk.hnqzz.top

TS:   [1, 2, 3].includes(x)
来源：http://sbm.yuxming.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://tte.hesvh.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://szs.zycfv.cn

Ruby: [1, 2, 3].include?(x)
来源：http://omo.xuetiantiany.cn

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://fwo.haohaochexian.top

[B15] 布尔运算与取反
来源：http://fxg.jianghu66.top

Py:   a and b or not c
来源：http://qvz.zhongyouzk.top

PHP:  $a && $b || !$c
来源：http://zqb.jlsjyb.cn

JS:   a && b || !c
来源：http://uii.hywenlv.cn

TS:   a && b || !c
来源：http://njd.zhaomingkeji.xyz

Java: a && b || !c
来源：http://skc.shangyingyoupin.top

Go:   a && b || !c
来源：http://but.fktsv.cn

Ruby: a && b || !c
来源：http://leb.hysaishi.cn

C#:   a && b || !c
来源：http://vty.svipenyu.cn

[B16] 卫语句：不满足条件提前返回
来源：http://vyz.xuetiantiany.cn

Py:   if not data: return
来源：http://ayd.zdbjq.cn

PHP:  if (!$data) { return; }
来源：http://hkg.sufxvd.cn

JS:   if (!data) return;
来源：http://hrd.zhoulong.xyz

TS:   if (!data) return;
来源：http://aio.316326.xyz

Java: if (data == null) return;
来源：http://ave.ydzc1.top

Go:   if data == nil { return }
来源：http://tqh.hammf.cn

Ruby: return if data.nil?
来源：http://ffv.hnxiangtu.top

C#:   if (data == null) return;
来源：http://qja.uphjek.com

================================================================================
来源：http://tzk.jqgfzy.top

C. 函数与作用域
来源：http://nws.hnxiangtu.top

================================================================================
来源：http://kes.jqgfzy.top

[C01] 定义函数
来源：http://bup.fzhhl.top

Py:   def add(a, b): return a + b
来源：http://ibu.mhx1999.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wwd.yj20258.top

JS:   function add(a, b) { return a + b; }
来源：http://njp.jiagoushi.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ava.jinqigufen.top

Java: static int add(int a, int b) { return a + b; }
来源：http://asv.snrcjt.cn

Go:   func add(a, b int) int { return a + b }
来源：http://tml.pengpengdd.cyou

Ruby: def add(a, b); a + b; end
来源：http://kzh.shuidangran.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://yjs.svipenyu.cn

[C02] 默认参数
来源：http://vbf.svipenyu.cn

Py:   def greet(name="World"): return name
来源：http://grv.shangyingyoupin.top

PHP:  function greet($name = "World") { return $name; }
来源：http://drb.yanxiufei.cn

JS:   function greet(name = "World") { return name; }
来源：http://ocq.birdmap.top

TS:   function greet(name: string = "World") { return name; }
来源：http://ktv.epnwcf.com

Java: // 无默认参数：方法重载或 Optional
来源：http://thp.xziqi.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://knm.shuidangran.top

Ruby: def greet(name = "World") = name
来源：http://nxm.tarul.cn

C#:   string Greet(string name = "World") => name;
来源：http://gol.hywenlv.cn

[C03] 可变参数
来源：http://fgg.ydjk.org.cn

Py:   def total(*args): return sum(args)
来源：http://erz.fzhhl.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://ibp.yanxiufei.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://xan.yfazqb.com

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://uuy.andypj.xyz

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://pgw.fehbvm.com

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hfl.dashuyun.cn

Ruby: def total(*nums); nums.sum; end
来源：http://qyc.hfpthk.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://zub.iojbl.cn

[C04] 命名参数 / 关键字参数
来源：http://cby.haohaochexian.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://uqb.jianghu66.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://fhf.gotoacloud.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://ygb.tian-w.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ema.tianlin.xyz

Java: // 无：用 Builder 模式或 record
来源：http://fhx.cdnleiting.top

Go:   // 无：用配置结构体参数
来源：http://fww.sxryk.cn

Ruby: f(a: 1, b: 2)
来源：http://uky.zhiwuduotai.top

C#:   f(a: 1, b: 2)
来源：http://eaq.cheryme.top

[C05] 返回多个值
来源：http://heh.ydzc1.top

Py:   return a, b
来源：http://dhv.fengsongda.top

PHP:  return [$a, $b];
来源：http://vym.shzxlz.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://qyn.nanxuanxn.top

TS:   return { a, b };
来源：http://jjr.ctjpmb.com

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://uzs.zdbjq.cn

Go:   return a, b
来源：http://bgu.jinyuanbaomall.cn

Ruby: return a, b
来源：http://lis.svipenyu.cn

C#:   return (a, b);              // ValueTuple
来源：http://kdd.nwbrower.top

[C06] 匿名函数 / lambda
来源：http://uyw.tanke756.top

Py:   square = lambda x: x * x
来源：http://oqb.sysykeji.top

PHP:  $square = fn($x) => $x * $x;
来源：http://vld.yuanzhike.top

JS:   const square = x => x * x;
来源：http://hvn.0kj1m.cn

TS:   const square = (x: number): number => x * x;
来源：http://gmh.shanyushiyangkeji.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://tql.yj20258.top

Go:   sq := func(x int) int { return x * x }
来源：http://kwg.jlsjyb.cn

Ruby: square = ->(x) { x * x }
来源：http://ayp.xylfe.cn

C#:   Func<int, int> square = x => x * x;
来源：http://vcs.smart0.xyz

[C07] 把函数作为参数传入
来源：http://lzc.9152youxi.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://lbj.bjfxy.top

PHP:  array_map("strtoupper", $arr);
来源：http://ajz.jinyuanbaomall.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qqq.guowangkeji.top

TS:   arr.map(String)
来源：http://ljf.fehbvm.com

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sva.shzxlz.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hhp.sjlbkw.cn

Ruby: arr.map(&:upcase)
来源：http://gmw.sjlbkw.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://web.jqgufenzy.top

[C08] 闭包
来源：http://hks.316326.xyz

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ulg.yueranfly.top

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://bxt.dashuyun.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qnh.bbcook.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hps.smart0.xyz

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ndf.chenlongwang.top


<!-- 参考信息 -->