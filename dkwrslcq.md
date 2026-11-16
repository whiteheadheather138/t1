代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hjb.aibaodan.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xtt.52xcode.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://frg.uphjek.com

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cam.tian-w.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ubt.guannengcc.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://dmt.shzxlz.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fpl.tianlin.xyz

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://nyu.smart0.xyz

[A18] 字符与 ASCII 码互转
来源：http://fnt.xuetiantiany.cn

Py:   ord("A"); chr(65)
来源：http://oip.wangshuangyany.cn

PHP:  ord("A"); chr(65)
来源：http://ojy.quarkkingdee.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://dyz.gotoacloud.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://cvb.yvedp.cn

Java: (int) 'A'; (char) 65
来源：http://ydf.zhixingplan.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ibh.hesvh.cn

Ruby: "A".ord; 65.chr
来源：http://gdg.xuanzx.com

C#:   (int)'A'; (char)65
来源：http://lzv.shangyingyoupin.top

[A19] 交换两个变量
来源：http://hna.svipenyu.cn

Py:   a, b = b, a
来源：http://nya.fktsv.cn

PHP:  [$a, $b] = [$b, $a];
来源：http://dyo.cqqwz.cn

JS:   [a, b] = [b, a];
来源：http://rhs.gogol.net.cn

TS:   [a, b] = [b, a];
来源：http://bhh.ydzc1.top

Java: int t = a; a = b; b = t;
来源：http://ayg.wangdashe.top

Go:   a, b = b, a
来源：http://gnp.tanke756.top

Ruby: a, b = b, a
来源：http://vuf.chenzaomai.com

C#:   (a, b) = (b, a);
来源：http://knw.zhoulong.xyz

[A20] 读取标准输入
来源：http://gcq.sweek.top

Py:   name = input("请输入：")
来源：http://qgk.jinqigufen.top

PHP:  $name = trim(fgets(STDIN));
来源：http://ela.cashguo.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wlc.dianchejie.cn

TS:   // Node.js：readline 模块
来源：http://nsp.yj20258888.top

Java: new Scanner(System.in).nextLine()
来源：http://kbq.wangshuangyany.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://jcc.yonumen.top

Ruby: gets.chomp
来源：http://oyo.quarkkingdee.top

C#:   Console.ReadLine();
来源：http://ifn.shanyushiyangtech.top

[A21] 保留指定小数位输出
来源：http://boj.shuidangran.top

Py:   f"{3.14159:.2f}"
来源：http://hgh.dianchejie.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://vmq.uphjek.com

JS:   (3.14159).toFixed(2)
来源：http://bss.ppjwa.cn

TS:   (3.14159).toFixed(2)
来源：http://dcy.chenzaomai.com

Java: String.format("%.2f", 3.14159)
来源：http://trd.yj202588.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wrh.dianchejie.cn

Ruby: format("%.2f", 3.14159)
来源：http://wwm.zycfv.cn

C#:   3.14159.ToString("F2")
来源：http://zoh.meibo888.top

[A22] 获取字符串长度
来源：http://ghu.sufxvd.cn

Py:   len(s)
来源：http://ncy.cashguo.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://sjw.feifeiyinyue.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://sjc.svipenyu.cn

TS:   s.length
来源：http://dto.shanyushiyangtech.top

Java: s.length()
来源：http://ndb.shanyushiyangkeji.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hxf.smart0.xyz

Ruby: s.length
来源：http://uof.chenjidiqi.icu

C#:   s.Length
来源：http://lyj.316326.xyz

[A23] 大小写转换
来源：http://drm.nanxuanxn.top

Py:   s.upper(); s.lower(); s.title()
来源：http://hll.wangdashe.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://afn.tarul.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://gaf.snrcjt.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mcu.jinyuanbaomall.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://fvg.zhiwuduotai.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://nbn.tianlin.xyz

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://iff.jyoumei.cn

C#:   s.ToUpper(); s.ToLower()
来源：http://goc.yvedp.cn

[A24] 去除首尾空白
来源：http://vwm.shanyushiyangtech.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://npu.shanyushiyangtech.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://nck.birdmap.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://eto.dashuyun.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wic.316326.xyz

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://izr.52xcode.cn

Go:   strings.TrimSpace(s)
来源：http://nzj.zhijiandao.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://cmr.316326.xyz

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ndi.tianlin.xyz

[A25] 字符串比较
来源：http://cjh.tian-w.cn

Py:   s1 == s2; s1 != s2
来源：http://dlo.jinqigfzy.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://qjg.aizwys.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://bhf.ywan-chungtsiang.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://tgg.ehwqpu.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wmq.fanxiaobao.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hpy.hfpthk.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://tej.yuanzhike.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://nkw.guannengcc.top

[A26] 类型转换总览
来源：http://pnk.9152youxi.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dko.ydzc1.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://nke.hesvh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://qmr.ehwqpu.com

TS:   Number() String() Boolean() x as number
来源：http://hxe.yvedp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://okp.cheryme.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://rry.wangdashe.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://njb.ctjpmb.com

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://zbi.tian-w.cn

================================================================================
来源：http://otp.0kj1m.cn

B. 流程控制
来源：http://znj.yj202588.top

================================================================================
来源：http://orj.nanxinkj.top

[B01] 条件判断 if / else
来源：http://qgv.316326.xyz

Py:   result = "正" if x > 0 else "非正"
来源：http://pto.ivvv.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://oby.zhengqikj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://vup.cdnleiting.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://pdx.jinqigufen.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://hyv.ehwqpu.com

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://fxp.xuanzx.com

Ruby: r = x > 0 ? "正" : "非正"
来源：http://ehz.cashguo.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kua.guannengcc.top

[B02] 多分支 else if / elif
来源：http://tuo.yvedp.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://llg.zhongyouzk.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hsd.hnxiangtu.top

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xlk.ybcxt.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://jih.tianlin.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ure.haohaochexian.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://xpy.yfazqb.com

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://xwv.guannengcc.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vlr.hesvh.cn

[B03] switch / match / case
来源：http://bhc.yvedp.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mtz.tarul.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ycu.yonumen.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://xor.zdqjudy.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dna.quarkkingdee.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://mdg.zhongyouzk.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://bak.9152youxi.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://rdd.tian-w.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://vvc.snrcjt.cn

[B04] for 计数循环
来源：http://uwk.zycfv.cn

Py:   for i in range(10): print(i)
来源：http://wox.hcnkem.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://njj.316326.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fdj.yfazqb.com

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mxp.316326.xyz

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://dni.jinqigufen.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wdp.uphjek.com

Ruby: 10.times { |i| puts i }
来源：http://mlz.yanxiufei.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://pli.yuxming.cn

[B05] 遍历数组 / 列表
来源：http://zkf.svipenyu.cn

Py:   for item in arr: print(item)
来源：http://uhd.redwolf501.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xwe.fengsongda.top

JS:   for (const item of arr) { console.log(item); }
来源：http://mmw.nanxuanxn.top

TS:   for (const item of arr) { console.log(item); }
来源：http://tsv.jinqigufen.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://fqx.andypj.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wzm.cucudq.cn

Ruby: arr.each { |item| puts item }
来源：http://gbu.guannengcc.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://oxx.ehwqpu.com

[B06] 遍历字典 / 对象
来源：http://gep.cucudq.cn

Py:   for k, v in d.items(): print(k, v)
来源：http://tky.dashuyun.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://zdg.gzhubu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://jrc.wangshuangyany.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://awd.yuanzhike.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://cqe.yanxiufei.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://apv.hongshengwenyu.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://rbb.ivvv.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://bpi.ydzc1.top

[B07] while 循环
来源：http://dlo.shuidangran.top

Py:   while i < 10: i += 1
来源：http://mgk.jiagoushi.top

PHP:  while ($i < 10) { $i++; }
来源：http://fvu.yuxming.cn

JS:   while (i < 10) { i++; }
来源：http://kow.hnqzz.top

TS:   while (i < 10) { i++; }
来源：http://ksm.guannengcc.top

Java: while (i < 10) { i++; }
来源：http://bjp.smart0.xyz

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ajs.ehwqpu.com

Ruby: while i < 10; i += 1; end
来源：http://zwr.aibaodan.cn

C#:   while (i < 10) { i++; }
来源：http://qtq.hfpthk.cn

[B08] do-while（至少执行一次）
来源：http://alq.feifeiyinyue.top

Py:   # 无 do-while：用 while True + break
来源：http://iay.0kj1m.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ksc.jinqigfzy.top

JS:   do { i++; } while (i < 10);
来源：http://fvn.cashguo.top

TS:   do { i++; } while (i < 10);
来源：http://jqk.vehdjk.com

Java: do { i++; } while (i < 10);
来源：http://djq.ywan-chungtsiang.top

Go:   for { i++; if i >= 10 { break } }
来源：http://nwa.smart0.xyz

Ruby: begin; i += 1; end while i < 10
来源：http://fqj.jqgfzy.top

C#:   do { i++; } while (i < 10);
来源：http://zsx.yj20258888.top

[B09] break 与 continue
来源：http://rfo.sufxvd.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://uwj.ppjwa.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://usb.daxiang520.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://sro.xziqi.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://bzi.redwolf501.top

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ddx.zhixingplan.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://crd.vqdsnc.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://puj.ehwqpu.com

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://jkm.c1oappe.top

[B10] 遍历同时拿索引
来源：http://tvz.shanyushiyangtech.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://bkr.zhoulong.xyz

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://guu.hongshengwenyu.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://lcc.yongpay.top

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://pey.hcnkem.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://dsq.hesvh.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://zzb.hywenlv.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://zrf.jinghuilouyu.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ija.fktsv.cn

[B11] 生成数字序列 / 区间
来源：http://hjd.vqdsnc.cn

Py:   list(range(0, 10, 2))
来源：http://nnv.haohaochexian.top

PHP:  range(0, 10, 2);
来源：http://fpg.pengpengdd.cyou

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://zag.c1oappe.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tlm.mhx1999.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ulu.xylfe.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nnj.ivvv.top

Ruby: (0...10).step(2).to_a
来源：http://lsi.cucudq.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://srs.bjfxy.top

[B12] 跳出多层循环
来源：http://jbd.guannengcc.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://utx.jinghuilouyu.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://poe.zdqjudy.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://afk.birdmap.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://seo.aizwys.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://rib.sweek.top

Go:   # 无标签：用布尔标志或抽成函数
来源：http://fuc.feifeiyinyue.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://ebm.fzhhl.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://whb.chenzaomai.com

[B13] 判断是否为数字
来源：http://dbs.tianlin.xyz

Py:   isinstance(x, (int, float))
来源：http://fdm.xylfe.cn

PHP:  is_numeric($x)
来源：http://xja.vehdjk.com

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://pbq.xingfuxueyuan.xyz

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://lae.yfazqb.com

Java: x instanceof Number
来源：http://pgk.yonumen.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://gao.jinqigfzy.top

Ruby: x.is_a?(Numeric)
来源：http://abo.yj20258888.top

C#:   x is int or double or decimal
来源：http://xlk.vqdsnc.cn

[B14] 判断值是否在集合内
来源：http://ozl.shangyingyoupin.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://bry.cqqwz.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ywn.yonumen.top

JS:   [1, 2, 3].includes(x)
来源：http://tfv.dianchejie.cn

TS:   [1, 2, 3].includes(x)
来源：http://ist.zhiwuduotai.top

Java: List.of(1, 2, 3).contains(x)
来源：http://hrg.kuanghao11.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://iin.ppjwa.cn

Ruby: [1, 2, 3].include?(x)
来源：http://byu.zhengqikj.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://dwd.bjfxy.top

[B15] 布尔运算与取反
来源：http://rpu.ctjpmb.com

Py:   a and b or not c
来源：http://jzz.chenlongwang.top

PHP:  $a && $b || !$c
来源：http://pna.yuxming.cn

JS:   a && b || !c
来源：http://oig.ydzc1.top

TS:   a && b || !c
来源：http://wuo.nanxinkj.top

Java: a && b || !c
来源：http://mtw.hammf.cn

Go:   a && b || !c
来源：http://fxc.yonumen.top

Ruby: a && b || !c
来源：http://fjm.ehwqpu.com

C#:   a && b || !c
来源：http://yio.epnwcf.com

[B16] 卫语句：不满足条件提前返回
来源：http://ivk.cheryme.top

Py:   if not data: return
来源：http://vbm.guowangkeji.top

PHP:  if (!$data) { return; }
来源：http://kug.yonumen.top

JS:   if (!data) return;
来源：http://ypd.daxiang520.top

TS:   if (!data) return;
来源：http://cpk.hongshengwenyu.top

Java: if (data == null) return;
来源：http://ahs.ybcxt.top

Go:   if data == nil { return }
来源：http://way.cheryme.top

Ruby: return if data.nil?
来源：http://qjr.pycfn.com

C#:   if (data == null) return;
来源：http://zbd.mhx1999.top

================================================================================
来源：http://hpd.meibo888.top

C. 函数与作用域
来源：http://kfk.zdqjudy.top

================================================================================
来源：http://htk.xuetiantiany.cn

[C01] 定义函数
来源：http://lmz.cqqwz.cn

Py:   def add(a, b): return a + b
来源：http://aym.jiagoushi.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gor.hfpthk.cn

JS:   function add(a, b) { return a + b; }
来源：http://gwz.zhixingplan.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uzb.gzhubu.top

Java: static int add(int a, int b) { return a + b; }
来源：http://xbe.gotoacloud.top

Go:   func add(a, b int) int { return a + b }
来源：http://mdq.wangdashe.top

Ruby: def add(a, b); a + b; end
来源：http://kju.cashguo.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://fad.gotoacloud.top

[C02] 默认参数
来源：http://qkf.hesvh.cn

Py:   def greet(name="World"): return name
来源：http://hyq.andypj.xyz

PHP:  function greet($name = "World") { return $name; }
来源：http://vkv.chenzaomai.com

JS:   function greet(name = "World") { return name; }
来源：http://fsj.bbcook.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://dxf.xingfuxueyuan.xyz

Java: // 无默认参数：方法重载或 Optional
来源：http://khk.316326.xyz

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://cui.yj20258888.top

Ruby: def greet(name = "World") = name
来源：http://bgn.hywenlv.cn

C#:   string Greet(string name = "World") => name;
来源：http://pic.sweek.top

[C03] 可变参数
来源：http://spe.fzhhl.top

Py:   def total(*args): return sum(args)
来源：http://bff.cheryme.top

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://xqd.birdmap.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bcr.sxryk.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wnu.svipenyu.cn

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://csd.gotoacloud.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://zmb.nwbrower.top

Ruby: def total(*nums); nums.sum; end
来源：http://ogy.redwolf501.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://jmj.xingfuxueyuan.xyz

[C04] 命名参数 / 关键字参数
来源：http://zrf.yonumen.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://zex.yj20258.top

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://jwb.yonumen.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://tcg.sysykeji.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://rmp.iojbl.cn

Java: // 无：用 Builder 模式或 record
来源：http://nap.zhixingplan.top

Go:   // 无：用配置结构体参数
来源：http://tqb.kuanghao11.cn

Ruby: f(a: 1, b: 2)
来源：http://ugq.hammf.cn

C#:   f(a: 1, b: 2)
来源：http://bwa.zhongyouzk.top

[C05] 返回多个值
来源：http://jrh.zhaomingkeji.xyz

Py:   return a, b
来源：http://ayf.hnqzz.top

PHP:  return [$a, $b];
来源：http://nxv.smart0.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://kau.yueranfly.top

TS:   return { a, b };
来源：http://wgh.daria6918.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ort.havefunace.top

Go:   return a, b
来源：http://hcr.cashguo.top

Ruby: return a, b
来源：http://wag.bbcook.cn

C#:   return (a, b);              // ValueTuple
来源：http://srw.0kj1m.cn

[C06] 匿名函数 / lambda
来源：http://djq.kuanghao11.cn

Py:   square = lambda x: x * x
来源：http://ebl.hcnkem.com

PHP:  $square = fn($x) => $x * $x;
来源：http://vcd.pengpengdd.cyou

JS:   const square = x => x * x;
来源：http://iwi.fktsv.cn

TS:   const square = (x: number): number => x * x;
来源：http://cyw.ybcxt.top

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://man.ppjwa.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bol.quarkkingdee.top

Ruby: square = ->(x) { x * x }
来源：http://mfe.ctjpmb.com

C#:   Func<int, int> square = x => x * x;
来源：http://okp.jlsjyb.cn

[C07] 把函数作为参数传入
来源：http://kbs.smart0.xyz

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wrm.yueranfly.top

PHP:  array_map("strtoupper", $arr);
来源：http://hbw.sufxvd.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cuu.shuidangran.top

TS:   arr.map(String)
来源：http://aii.haohaochexian.top

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://khz.jqgfzy.top

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://deq.tian-w.cn


<!-- 参考信息 -->