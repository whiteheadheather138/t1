代发 wailian999

C#:   // 单行；/* 多行 */
来源：http://spk.iojbl.cn

[A15] 空值判断与默认值
来源：http://bam.jlsjyb.cn

Py:   value = data or "默认值"
来源：http://dhl.aizwys.cn

PHP:  $value = $data ?? "默认值";
来源：http://dbl.tianlin.xyz

JS:   const value = data ?? "默认值";
来源：http://vad.redwolf501.top

TS:   const value = data ?? "默认值";
来源：http://ndr.tanke756.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://owo.zhengqikj.top

Go:   if data == "" { data = "默认值" }
来源：http://coy.yj20258888.top

Ruby: value = data || "默认值"
来源：http://dgf.zycfv.cn

C#:   var value = data ?? "默认值";
来源：http://zxl.yfazqb.com

[A16] 真假值判断规则
来源：http://jnw.hammf.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://cjj.316326.xyz

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://rsi.daria6918.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lrz.cqqwz.cn

TS:   if (!x) {}
来源：http://fwf.hesvh.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://esy.nwbrower.top

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://lhy.havefunace.top

Ruby: unless x            # nil 与 false 为假
来源：http://egr.cucudq.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ysn.cheryme.top

[A17] 位运算
来源：http://miq.jlsjyb.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://tll.cdnleiting.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://dev.sweek.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://sok.xylfe.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://cxc.ybcxt.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://buf.ehwqpu.com

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://gul.cucudq.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kuf.epnwcf.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rxx.fktsv.cn

[A18] 字符与 ASCII 码互转
来源：http://adz.quarkkingdee.top

Py:   ord("A"); chr(65)
来源：http://qhl.yuanzhike.top

PHP:  ord("A"); chr(65)
来源：http://fjr.chenlongwang.top

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://adp.wangshuangyany.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vtg.52xcode.cn

Java: (int) 'A'; (char) 65
来源：http://tew.ivvv.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://aas.chenlongwang.top

Ruby: "A".ord; 65.chr
来源：http://vov.xylfe.cn

C#:   (int)'A'; (char)65
来源：http://wsi.bjfxy.top

[A19] 交换两个变量
来源：http://ice.ydjk.org.cn

Py:   a, b = b, a
来源：http://brm.zhengqikj.top

PHP:  [$a, $b] = [$b, $a];
来源：http://fbu.ehwqpu.com

JS:   [a, b] = [b, a];
来源：http://abh.shuidangran.top

TS:   [a, b] = [b, a];
来源：http://gvx.svipenyu.cn

Java: int t = a; a = b; b = t;
来源：http://tkd.xinyue.icu

Go:   a, b = b, a
来源：http://yff.cheryme.top

Ruby: a, b = b, a
来源：http://tym.pengpengdd.cyou

C#:   (a, b) = (b, a);
来源：http://zvo.tian-w.cn

[A20] 读取标准输入
来源：http://jyx.epnwcf.com

Py:   name = input("请输入：")
来源：http://chn.9152youxi.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://ymf.dashuyun.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mbq.jlsjyb.cn

TS:   // Node.js：readline 模块
来源：http://ggu.nanxuanxn.top

Java: new Scanner(System.in).nextLine()
来源：http://xec.tanke756.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ghz.jinqigfzy.top

Ruby: gets.chomp
来源：http://xbq.guannengcc.top

C#:   Console.ReadLine();
来源：http://bcp.52xcode.cn

[A21] 保留指定小数位输出
来源：http://mgx.fzhhl.top

Py:   f"{3.14159:.2f}"
来源：http://wbd.hywenlv.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://opu.meibo888.top

JS:   (3.14159).toFixed(2)
来源：http://ipl.shuidangran.top

TS:   (3.14159).toFixed(2)
来源：http://nxe.52xcode.cn

Java: String.format("%.2f", 3.14159)
来源：http://rcf.jiagoushi.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://xcz.hnqzz.top

Ruby: format("%.2f", 3.14159)
来源：http://mle.zhongyouzk.top

C#:   3.14159.ToString("F2")
来源：http://epw.shzxlz.cn

[A22] 获取字符串长度
来源：http://pgp.xylfe.cn

Py:   len(s)
来源：http://qfy.yj20258.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://spc.xylfe.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://uvv.havefunace.top

TS:   s.length
来源：http://yip.pengpengdd.cyou

Java: s.length()
来源：http://eil.zhijiandao.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ctm.daxiang520.top

Ruby: s.length
来源：http://ixt.xinyue.icu

C#:   s.Length
来源：http://eja.smart0.xyz

[A23] 大小写转换
来源：http://qxt.wangdashe.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pho.ydzc1.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://oaz.mhx1999.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://muu.zhijiandao.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://oic.xylfe.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jeq.dianchejie.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://ejm.hywenlv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://ldd.jiagoushi.top

C#:   s.ToUpper(); s.ToLower()
来源：http://hff.ybcxt.top

[A24] 去除首尾空白
来源：http://krm.yj20258.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://trj.zdbjq.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://htb.yanxiufei.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://jek.cqqwz.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://nax.yongpay.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://rbw.bbcook.cn

Go:   strings.TrimSpace(s)
来源：http://mir.jinqigfzy.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://rhx.nanxuanxn.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://ewf.fanxiaobao.xyz

[A25] 字符串比较
来源：http://ajh.vehdjk.com

Py:   s1 == s2; s1 != s2
来源：http://qzf.zhoulong.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://ckj.redwolf501.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://adj.andypj.xyz

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wck.bbcook.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://nzi.mhx1999.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://ebz.yuanzhike.top

Ruby: s1 == s2; s1 <=> s2
来源：http://nqg.wangshuangyany.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://qca.zycfv.cn

[A26] 类型转换总览
来源：http://qbp.jqgfzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://dgr.wangshuangyany.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://iaf.wangdashe.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://llv.fktsv.cn

TS:   Number() String() Boolean() x as number
来源：http://hfk.yvedp.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://ofv.yueranfly.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://msp.shanyushiyangtech.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://xqr.yj20258888.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://rav.cashguo.top

================================================================================
来源：http://wyi.fzhhl.top

B. 流程控制
来源：http://qpb.hongshengwenyu.top

================================================================================
来源：http://jzs.daria6918.cn

[B01] 条件判断 if / else
来源：http://qzx.birdmap.top

Py:   result = "正" if x > 0 else "非正"
来源：http://alz.nanxuanxn.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://lfs.fzhhl.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://kgd.jinghuilouyu.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://iqk.xuanzx.com

Java: String r = x > 0 ? "正" : "非正";
来源：http://jji.tarul.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://ikp.smart0.xyz

Ruby: r = x > 0 ? "正" : "非正"
来源：http://vcy.gaohongyu789.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://kwn.jqgfzy.top

[B02] 多分支 else if / elif
来源：http://esb.hywenlv.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://vys.zhongyouzk.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://yqy.xingfuxueyuan.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ymp.sysykeji.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://ndk.iojbl.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zqv.zhixingplan.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://pvj.cheryme.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://kpp.jinqigufen.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bpq.jinyuanbaomall.cn

[B03] switch / match / case
来源：http://pgz.c1oappe.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://dlz.tarul.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://cwj.daxiang520.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://jqn.kuanghao11.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lvz.andypj.xyz

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://aue.daxiang520.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://jsm.uphjek.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://apf.uphjek.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mxn.mhx1999.top

[B04] for 计数循环
来源：http://bje.haohaochexian.top

Py:   for i in range(10): print(i)
来源：http://wkn.yuxming.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ubg.epnwcf.com

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://jkw.hnqzz.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://sfp.jinyuanbaomall.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://bmr.52xcode.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://dna.xuanzx.com

Ruby: 10.times { |i| puts i }
来源：http://ykl.ywan-chungtsiang.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ije.hcnkem.com

[B05] 遍历数组 / 列表
来源：http://jmd.zycfv.cn

Py:   for item in arr: print(item)
来源：http://hvy.316326.xyz

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://ree.ywan-chungtsiang.top

JS:   for (const item of arr) { console.log(item); }
来源：http://nve.gogol.net.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://npz.jlsjyb.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://qoq.yvedp.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://phm.mhx1999.top

Ruby: arr.each { |item| puts item }
来源：http://oml.jianghu66.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wek.yanxiufei.cn

[B06] 遍历字典 / 对象
来源：http://clw.daxiang520.top

Py:   for k, v in d.items(): print(k, v)
来源：http://irj.meibo888.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ttg.hnxiangtu.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://caj.xuanzx.com

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://eii.cqqwz.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bka.zhijiandao.cn

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vlm.bjfxy.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://jgh.ybcxt.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://fvf.bjfxy.top

[B07] while 循环
来源：http://lgg.hnqzz.top

Py:   while i < 10: i += 1
来源：http://wnr.xuetiantiany.cn

PHP:  while ($i < 10) { $i++; }
来源：http://pnp.wangdashe.top

JS:   while (i < 10) { i++; }
来源：http://imh.hesvh.cn

TS:   while (i < 10) { i++; }
来源：http://aty.hcnkem.com

Java: while (i < 10) { i++; }
来源：http://vyq.nanxinkj.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://epv.shuidangran.top

Ruby: while i < 10; i += 1; end
来源：http://tjr.xuanzx.com

C#:   while (i < 10) { i++; }
来源：http://nek.jlsjyb.cn

[B08] do-while（至少执行一次）
来源：http://agv.smart0.xyz

Py:   # 无 do-while：用 while True + break
来源：http://ugm.ppjwa.cn

PHP:  do { $i++; } while ($i < 10);
来源：http://ojb.zhoulong.xyz

JS:   do { i++; } while (i < 10);
来源：http://mkc.yangfankeji.com

TS:   do { i++; } while (i < 10);
来源：http://tdd.wangshuangyany.cn

Java: do { i++; } while (i < 10);
来源：http://ncw.yj20258.top

Go:   for { i++; if i >= 10 { break } }
来源：http://piv.ivvv.top

Ruby: begin; i += 1; end while i < 10
来源：http://fkt.feifeiyinyue.top

C#:   do { i++; } while (i < 10);
来源：http://suc.ydjk.org.cn

[B09] break 与 continue
来源：http://aif.snrcjt.cn

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://zte.yonumen.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://tok.ydjk.org.cn

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://evm.fengsongda.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://nmm.hysaishi.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://qxi.yj202588.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rtn.hongshengwenyu.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://dzk.c1oappe.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://loh.haohaochexian.top

[B10] 遍历同时拿索引
来源：http://bcx.yongpay.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://url.52xcode.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://xrb.jinqigfzy.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hws.hysaishi.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gpt.redwolf501.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://kvk.tarul.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ano.0kj1m.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://ftd.gotoacloud.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://fmt.shanyushiyangkeji.top

[B11] 生成数字序列 / 区间
来源：http://emb.sxryk.cn

Py:   list(range(0, 10, 2))
来源：http://gnb.jianghu66.top

PHP:  range(0, 10, 2);
来源：http://gyy.havefunace.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://dnt.jqgfzy.top

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://fjh.gaohongyu789.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://odc.hfpthk.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://flq.52xcode.cn

Ruby: (0...10).step(2).to_a
来源：http://jpl.guowangkeji.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://yll.birdmap.top

[B12] 跳出多层循环
来源：http://gfi.cucudq.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://ykk.quarkkingdee.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://xwl.nanxuanxn.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://sqy.hnqzz.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hsy.snrcjt.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wsm.tianlin.xyz

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hvy.jinqigfzy.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://nkj.ppjwa.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://jvc.jinghuilouyu.cn

[B13] 判断是否为数字
来源：http://sfa.sysykeji.top

Py:   isinstance(x, (int, float))
来源：http://tse.ivvv.top

PHP:  is_numeric($x)
来源：http://tjv.nwbrower.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mas.aizwys.cn

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://boy.shanyushiyangkeji.top

Java: x instanceof Number
来源：http://kdx.sufxvd.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://bsy.tarul.cn

Ruby: x.is_a?(Numeric)
来源：http://frt.pengpengdd.cyou

C#:   x is int or double or decimal
来源：http://oce.cdnleiting.top

[B14] 判断值是否在集合内
来源：http://osc.jinqigfzy.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tdh.wangdashe.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://ezi.52xcode.cn

JS:   [1, 2, 3].includes(x)
来源：http://hfw.shzxlz.cn

TS:   [1, 2, 3].includes(x)
来源：http://cgm.ydjk.org.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ssk.epnwcf.com

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://zpf.meibo888.top

Ruby: [1, 2, 3].include?(x)
来源：http://cye.c1oappe.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://oda.tanke756.top

[B15] 布尔运算与取反
来源：http://ypn.ivvv.top

Py:   a and b or not c
来源：http://qse.hnxiangtu.top

PHP:  $a && $b || !$c
来源：http://opj.zhengqikj.top

JS:   a && b || !c
来源：http://vbh.guowangkeji.top

TS:   a && b || !c
来源：http://fjf.ybcxt.top

Java: a && b || !c
来源：http://egs.guowangkeji.top

Go:   a && b || !c
来源：http://jtu.xuanzx.com

Ruby: a && b || !c
来源：http://ymu.hongshengwenyu.top

C#:   a && b || !c
来源：http://qve.yueranfly.top

[B16] 卫语句：不满足条件提前返回
来源：http://egh.wangdashe.top

Py:   if not data: return
来源：http://jih.sysykeji.top

PHP:  if (!$data) { return; }
来源：http://ouf.tarul.cn

JS:   if (!data) return;
来源：http://emr.shanyushiyangkeji.top

TS:   if (!data) return;
来源：http://nov.snrcjt.cn

Java: if (data == null) return;
来源：http://tsu.gaohongyu789.top

Go:   if data == nil { return }
来源：http://ieb.zdqjudy.top

Ruby: return if data.nil?
来源：http://rhs.shangyingyoupin.top

C#:   if (data == null) return;
来源：http://lxk.svipenyu.cn

================================================================================
来源：http://ozy.svipenyu.cn

C. 函数与作用域
来源：http://vtr.wangshuangyany.cn

================================================================================
来源：http://zpz.fengsongda.top

[C01] 定义函数
来源：http://mbb.pengpengdd.cyou

Py:   def add(a, b): return a + b
来源：http://qik.ydzc1.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qrx.yueranfly.top

JS:   function add(a, b) { return a + b; }
来源：http://xkl.vehdjk.com

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://efe.yongpay.top

Java: static int add(int a, int b) { return a + b; }
来源：http://iyd.sysykeji.top

Go:   func add(a, b int) int { return a + b }
来源：http://irh.c1oappe.top

Ruby: def add(a, b); a + b; end
来源：http://nif.yongpay.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://gqe.sufxvd.cn

[C02] 默认参数
来源：http://kgv.ydjk.org.cn

Py:   def greet(name="World"): return name
来源：http://rrl.aizwys.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://gvk.shanyushiyangtech.top

JS:   function greet(name = "World") { return name; }
来源：http://zzv.svipenyu.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://jnw.epnwcf.com

Java: // 无默认参数：方法重载或 Optional
来源：http://bfb.ppjwa.cn

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://rmh.52xcode.cn

Ruby: def greet(name = "World") = name
来源：http://fmy.zhongyouzk.top

C#:   string Greet(string name = "World") => name;
来源：http://wyw.nwbrower.top

[C03] 可变参数
来源：http://vgk.jqgfzy.top

Py:   def total(*args): return sum(args)
来源：http://kvg.ehwqpu.com

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://pit.yonumen.top

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://opk.aibaodan.cn

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://isb.yfazqb.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://dju.sweek.top

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://djq.yuxming.cn

Ruby: def total(*nums); nums.sum; end
来源：http://sqv.iojbl.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://udl.tarul.cn

[C04] 命名参数 / 关键字参数
来源：http://vgn.daxiang520.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ddl.zhoulong.xyz

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hhy.xuanzx.com

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://rzf.fzhhl.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://vpn.shangyingyoupin.top

Java: // 无：用 Builder 模式或 record
来源：http://qlb.vehdjk.com

Go:   // 无：用配置结构体参数
来源：http://ntq.gogol.net.cn

Ruby: f(a: 1, b: 2)
来源：http://eqs.0kj1m.cn

C#:   f(a: 1, b: 2)
来源：http://yhe.jianghu66.top

[C05] 返回多个值
来源：http://vlp.gaohongyu789.top

Py:   return a, b
来源：http://iyl.xuanzx.com

PHP:  return [$a, $b];
来源：http://ruc.xingfuxueyuan.xyz

JS:   return [a, b];             // 或 return { a, b };
来源：http://xwp.ywan-chungtsiang.top

TS:   return { a, b };
来源：http://van.meibo888.top


<!-- 参考信息 -->