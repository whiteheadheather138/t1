代发 wailian999

[A14] 注释写法
来源：http://ytu.zycfv.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://cgb.ivvv.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://jwm.jinqigufen.top

JS:   // 单行；/* 多行 */
来源：http://cii.zhixingplan.top

TS:   // 单行；/* 多行 */
来源：http://thc.zhixingplan.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hkp.feifeiyinyue.top

Go:   // 单行；/* 多行 */
来源：http://ajm.birdmap.top

Ruby: # 单行；=begin 多行 =end
来源：http://umr.andypj.xyz

C#:   // 单行；/* 多行 */
来源：http://pqh.cqqwz.cn

[A15] 空值判断与默认值
来源：http://tvh.dashuyun.cn

Py:   value = data or "默认值"
来源：http://rqy.cheryme.top

PHP:  $value = $data ?? "默认值";
来源：http://kro.yanxiufei.cn

JS:   const value = data ?? "默认值";
来源：http://rvc.jinqigufen.top

TS:   const value = data ?? "默认值";
来源：http://kle.jinghuilouyu.cn

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://siz.jinghuilouyu.cn

Go:   if data == "" { data = "默认值" }
来源：http://eug.iojbl.cn

Ruby: value = data || "默认值"
来源：http://jra.chenlongwang.top

C#:   var value = data ?? "默认值";
来源：http://bad.daxiang520.top

[A16] 真假值判断规则
来源：http://eby.zhoulong.xyz

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hdq.yfazqb.com

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://api.ehwqpu.com

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mbm.tian-w.cn

TS:   if (!x) {}
来源：http://laj.ctjpmb.com

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://svp.zdbjq.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://dih.bjfxy.top

Ruby: unless x            # nil 与 false 为假
来源：http://oyd.cheryme.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://vij.nwbrower.top

[A17] 位运算
来源：http://jud.fktsv.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cpu.vqdsnc.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://iaq.jinqigufen.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ykd.jlsjyb.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://fmg.nwbrower.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://zwf.meibo888.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://czu.fzhhl.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://umh.xinyue.icu

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://kne.cucudq.cn

[A18] 字符与 ASCII 码互转
来源：http://qmg.haohaochexian.top

Py:   ord("A"); chr(65)
来源：http://vfi.chenlongwang.top

PHP:  ord("A"); chr(65)
来源：http://wic.tian-w.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://uub.chenjidiqi.icu

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://qzl.ppjwa.cn

Java: (int) 'A'; (char) 65
来源：http://wzy.svipenyu.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://orb.yj20258.top

Ruby: "A".ord; 65.chr
来源：http://kqy.zhiwuduotai.top

C#:   (int)'A'; (char)65
来源：http://nma.zhiwuduotai.top

[A19] 交换两个变量
来源：http://tvl.sweek.top

Py:   a, b = b, a
来源：http://hmu.xuanzx.com

PHP:  [$a, $b] = [$b, $a];
来源：http://lmv.guowangkeji.top

JS:   [a, b] = [b, a];
来源：http://qpf.hnxiangtu.top

TS:   [a, b] = [b, a];
来源：http://cqj.iojbl.cn

Java: int t = a; a = b; b = t;
来源：http://ple.yj202588.top

Go:   a, b = b, a
来源：http://wjc.zhiwuduotai.top

Ruby: a, b = b, a
来源：http://xpu.fktsv.cn

C#:   (a, b) = (b, a);
来源：http://zua.zhiwuduotai.top

[A20] 读取标准输入
来源：http://noj.xingfuxueyuan.xyz

Py:   name = input("请输入：")
来源：http://xil.316326.xyz

PHP:  $name = trim(fgets(STDIN));
来源：http://mao.ivvv.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://pgr.svipenyu.cn

TS:   // Node.js：readline 模块
来源：http://gub.hnxiangtu.top

Java: new Scanner(System.in).nextLine()
来源：http://zen.shzxlz.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://trt.redwolf501.top

Ruby: gets.chomp
来源：http://nha.shangyingyoupin.top

C#:   Console.ReadLine();
来源：http://ief.ybcxt.top

[A21] 保留指定小数位输出
来源：http://bcm.tanke756.top

Py:   f"{3.14159:.2f}"
来源：http://vma.pycfn.com

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://nao.wangdashe.top

JS:   (3.14159).toFixed(2)
来源：http://rno.gogol.net.cn

TS:   (3.14159).toFixed(2)
来源：http://boi.fengsongda.top

Java: String.format("%.2f", 3.14159)
来源：http://ame.mhx1999.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://kie.epnwcf.com

Ruby: format("%.2f", 3.14159)
来源：http://rmv.iojbl.cn

C#:   3.14159.ToString("F2")
来源：http://gyp.jianghu66.top

[A22] 获取字符串长度
来源：http://gfa.dashuyun.cn

Py:   len(s)
来源：http://ghg.sufxvd.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://jiq.yj202588.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://pda.gzhubu.top

TS:   s.length
来源：http://uya.c1oappe.top

Java: s.length()
来源：http://dew.xingfuxueyuan.xyz

Go:   len(s); utf8.RuneCountInString(s)
来源：http://spa.chenzaomai.com

Ruby: s.length
来源：http://xxn.fanxiaobao.xyz

C#:   s.Length
来源：http://rrj.jqgfzy.top

[A23] 大小写转换
来源：http://zqv.xylfe.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://pqh.ivvv.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://rfb.hesvh.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ipz.316326.xyz

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://cae.feifeiyinyue.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jds.ehwqpu.com

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://vlz.fktsv.cn

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://tur.epnwcf.com

C#:   s.ToUpper(); s.ToLower()
来源：http://gkl.zhongyouzk.top

[A24] 去除首尾空白
来源：http://aox.aibaodan.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://cze.xuetiantiany.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://caq.birdmap.top

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pis.fengsongda.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://xfj.shzxlz.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://oxp.bjfxy.top

Go:   strings.TrimSpace(s)
来源：http://kma.chenlongwang.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://gen.yongpay.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://vwl.zhiwuduotai.top

[A25] 字符串比较
来源：http://huq.cucudq.cn

Py:   s1 == s2; s1 != s2
来源：http://ypg.yongpay.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://jps.cucudq.cn

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://uoy.snrcjt.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://lnu.sufxvd.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ode.zhaomingkeji.xyz

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://pup.svipenyu.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://pxv.fengsongda.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://apn.shanyushiyangkeji.top

[A26] 类型转换总览
来源：http://xcg.jqgfzy.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://con.nanxuanxn.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wnf.yfazqb.com

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://cta.gzhubu.top

TS:   Number() String() Boolean() x as number
来源：http://avy.hywenlv.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://goi.jinghuilouyu.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://cxn.zdqjudy.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://cey.tian-w.cn

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://dnl.iojbl.cn

================================================================================
来源：http://exj.quarkkingdee.top

B. 流程控制
来源：http://iuh.ydzc1.top

================================================================================
来源：http://itz.zhijiandao.cn

[B01] 条件判断 if / else
来源：http://nip.hcnkem.com

Py:   result = "正" if x > 0 else "非正"
来源：http://mzg.zhijiandao.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://ecg.jlsjyb.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://qif.jqgufenzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://jsl.jianghu66.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://dqj.jiagoushi.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://kfe.sysykeji.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://xnb.hnqzz.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://ffr.shzxlz.cn

[B02] 多分支 else if / elif
来源：http://qmd.guannengcc.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ymu.dianchejie.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://rzf.yuxming.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://zdr.gotoacloud.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://txb.316326.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fby.bbcook.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://dzh.gogol.net.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ccz.tarul.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cyh.tianlin.xyz

[B03] switch / match / case
来源：http://adi.hammf.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://kch.andypj.xyz

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://ggo.aizwys.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://dkh.ywan-chungtsiang.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://rhb.jinqigfzy.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hyz.zdqjudy.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://idg.yj20258888.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://jev.iojbl.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hez.sweek.top

[B04] for 计数循环
来源：http://xxj.yanxiufei.cn

Py:   for i in range(10): print(i)
来源：http://sng.pycfn.com

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://zvz.hfpthk.cn

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://fyu.xuetiantiany.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://pwp.52xcode.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://twv.cheryme.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wdg.jlsjyb.cn

Ruby: 10.times { |i| puts i }
来源：http://ghh.sysykeji.top

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://ejk.sysykeji.top

[B05] 遍历数组 / 列表
来源：http://sxt.ivvv.top

Py:   for item in arr: print(item)
来源：http://eej.tarul.cn

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://biq.chenjidiqi.icu

JS:   for (const item of arr) { console.log(item); }
来源：http://ref.yj202588.top

TS:   for (const item of arr) { console.log(item); }
来源：http://pcy.zhaomingkeji.xyz

Java: for (var item : arr) { System.out.println(item); }
来源：http://ric.316326.xyz

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xaf.bjfxy.top

Ruby: arr.each { |item| puts item }
来源：http://ecc.hongshengwenyu.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://duq.shanyushiyangkeji.top

[B06] 遍历字典 / 对象
来源：http://nwe.yj20258.top

Py:   for k, v in d.items(): print(k, v)
来源：http://swf.ydzc1.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://ops.hnqzz.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://utn.snrcjt.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://dcm.cdnleiting.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://oiz.yfazqb.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://zpk.cqqwz.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://ulj.hongshengwenyu.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://akc.tarul.cn

[B07] while 循环
来源：http://jvg.fehbvm.com

Py:   while i < 10: i += 1
来源：http://nxu.gotoacloud.top

PHP:  while ($i < 10) { $i++; }
来源：http://gza.snrcjt.cn

JS:   while (i < 10) { i++; }
来源：http://hwo.jianghu66.top

TS:   while (i < 10) { i++; }
来源：http://dew.bjfxy.top

Java: while (i < 10) { i++; }
来源：http://gqz.bbcook.cn

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://ufh.daxiang520.top

Ruby: while i < 10; i += 1; end
来源：http://mer.gaohongyu789.top

C#:   while (i < 10) { i++; }
来源：http://kdi.zhijiandao.cn

[B08] do-while（至少执行一次）
来源：http://cpa.cheryme.top

Py:   # 无 do-while：用 while True + break
来源：http://xrz.nanxuanxn.top

PHP:  do { $i++; } while ($i < 10);
来源：http://jid.havefunace.top

JS:   do { i++; } while (i < 10);
来源：http://ghm.shuidangran.top

TS:   do { i++; } while (i < 10);
来源：http://rdz.jqgfzy.top

Java: do { i++; } while (i < 10);
来源：http://sav.hysaishi.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://qls.daxiang520.top

Ruby: begin; i += 1; end while i < 10
来源：http://jck.bjfxy.top

C#:   do { i++; } while (i < 10);
来源：http://rio.snrcjt.cn

[B09] break 与 continue
来源：http://isf.sweek.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://vhg.zhijiandao.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://bpq.mhx1999.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mxr.52xcode.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ecx.hesvh.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://rui.cashguo.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://xvz.ydzc1.top

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://ixn.cdnleiting.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://inj.zhongyouzk.top

[B10] 遍历同时拿索引
来源：http://fqj.tianlin.xyz

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://gfy.feifeiyinyue.top

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://nru.zhoulong.xyz

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://qvr.hammf.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://gpx.yj20258.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://efg.zdqjudy.top

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://gnr.dianchejie.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://rgf.jinyuanbaomall.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://qfh.ywan-chungtsiang.top

[B11] 生成数字序列 / 区间
来源：http://etm.jinqigfzy.top

Py:   list(range(0, 10, 2))
来源：http://lhs.shangyingyoupin.top

PHP:  range(0, 10, 2);
来源：http://kxc.yonumen.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://djz.vehdjk.com

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://qxy.hesvh.cn

Java: IntStream.range(0, 10).boxed().toList()
来源：http://ysh.chenlongwang.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://nty.hongshengwenyu.top

Ruby: (0...10).step(2).to_a
来源：http://sop.nanxuanxn.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://zko.vqdsnc.cn

[B12] 跳出多层循环
来源：http://fra.sjlbkw.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://nta.chenjidiqi.icu

PHP:  # 无标签：用 goto 或函数返回
来源：http://dui.xziqi.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ack.zycfv.cn

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://tsw.cdnleiting.top

Java: outer: for (...) { for (...) { break outer; } }
来源：http://zfc.shzxlz.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://csu.yanxiufei.cn

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://yqg.gogol.net.cn

C#:   # 无标签：用 goto label 或布尔标志
来源：http://axo.hongshengwenyu.top

[B13] 判断是否为数字
来源：http://pvx.smart0.xyz

Py:   isinstance(x, (int, float))
来源：http://skk.fzhhl.top

PHP:  is_numeric($x)
来源：http://wrp.yongpay.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aif.yfazqb.com

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://umc.yj202588.top

Java: x instanceof Number
来源：http://rdu.ivvv.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://tgi.shanyushiyangkeji.top

Ruby: x.is_a?(Numeric)
来源：http://ytd.cheryme.top

C#:   x is int or double or decimal
来源：http://bpq.haohaochexian.top

[B14] 判断值是否在集合内
来源：http://jqn.svipenyu.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://tqm.kuanghao11.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://upz.yonumen.top

JS:   [1, 2, 3].includes(x)
来源：http://snt.dashuyun.cn

TS:   [1, 2, 3].includes(x)
来源：http://mgp.sjlbkw.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://krf.cucudq.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://vuy.jlsjyb.cn

Ruby: [1, 2, 3].include?(x)
来源：http://xtp.redwolf501.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://iir.xziqi.cn

[B15] 布尔运算与取反
来源：http://xou.shanyushiyangtech.top

Py:   a and b or not c
来源：http://ydd.zhengqikj.top

PHP:  $a && $b || !$c
来源：http://kat.fzhhl.top

JS:   a && b || !c
来源：http://luv.jlsjyb.cn

TS:   a && b || !c
来源：http://ayh.dianchejie.cn

Java: a && b || !c
来源：http://jqd.yvedp.cn

Go:   a && b || !c
来源：http://gum.jinyuanbaomall.cn

Ruby: a && b || !c
来源：http://dkg.vqdsnc.cn

C#:   a && b || !c
来源：http://vqa.meibo888.top

[B16] 卫语句：不满足条件提前返回
来源：http://dgh.52xcode.cn

Py:   if not data: return
来源：http://oxz.xuanzx.com

PHP:  if (!$data) { return; }
来源：http://wdu.hcnkem.com

JS:   if (!data) return;
来源：http://tbl.daxiang520.top

TS:   if (!data) return;
来源：http://jwb.zhijiandao.cn

Java: if (data == null) return;
来源：http://fao.gaohongyu789.top

Go:   if data == nil { return }
来源：http://xbk.jinqigufen.top

Ruby: return if data.nil?
来源：http://xkn.0kj1m.cn

C#:   if (data == null) return;
来源：http://xco.zhengqikj.top

================================================================================
来源：http://eax.sufxvd.cn

C. 函数与作用域
来源：http://itc.cheryme.top

================================================================================
来源：http://jjs.xinyue.icu

[C01] 定义函数
来源：http://ajx.fzhhl.top

Py:   def add(a, b): return a + b
来源：http://tcm.cheryme.top

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gtq.aizwys.cn

JS:   function add(a, b) { return a + b; }
来源：http://oip.c1oappe.top

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://upe.tian-w.cn

Java: static int add(int a, int b) { return a + b; }
来源：http://sfd.zhengqikj.top

Go:   func add(a, b int) int { return a + b }
来源：http://gri.fzhhl.top

Ruby: def add(a, b); a + b; end
来源：http://jzc.ybcxt.top

C#:   static int Add(int a, int b) { return a + b; }
来源：http://nod.9152youxi.cn

[C02] 默认参数
来源：http://bdc.ehwqpu.com

Py:   def greet(name="World"): return name
来源：http://smv.xylfe.cn

PHP:  function greet($name = "World") { return $name; }
来源：http://cpp.yj202588.top

JS:   function greet(name = "World") { return name; }
来源：http://fhr.sjlbkw.cn

TS:   function greet(name: string = "World") { return name; }
来源：http://edj.sjlbkw.cn

Java: // 无默认参数：方法重载或 Optional
来源：http://pol.yuanzhike.top

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://ril.hammf.cn

Ruby: def greet(name = "World") = name
来源：http://sep.jqgfzy.top

C#:   string Greet(string name = "World") => name;
来源：http://nrz.nanxinkj.top

[C03] 可变参数
来源：http://coy.hysaishi.cn

Py:   def total(*args): return sum(args)
来源：http://wrp.sxryk.cn

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://jct.sxryk.cn

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://bhx.tanke756.top

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://rtc.fehbvm.com

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://xgx.9152youxi.cn

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://cvb.gzhubu.top

Ruby: def total(*nums); nums.sum; end
来源：http://aum.yj20258888.top

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mjl.sufxvd.cn

[C04] 命名参数 / 关键字参数
来源：http://klb.shanyushiyangtech.top

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://idn.zycfv.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://lrj.yj202588.top

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://whc.ybcxt.top

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ijb.52xcode.cn

Java: // 无：用 Builder 模式或 record
来源：http://ckg.bbcook.cn


<!-- 参考信息 -->