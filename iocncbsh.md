代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://uca.yj20258888.top

C#:   x > 0 ? "yes" : "no"
来源：http://jky.xuetiantiany.cn

[A12] 字符串插值 / 格式化
来源：http://mgl.zycfv.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://qqs.jinghuilouyu.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zex.wangdashe.top

JS:   `Hello, ${name}!`
来源：http://jpy.zdbjq.cn

TS:   `Hello, ${name}!`
来源：http://poh.vehdjk.com

Java: "Hello, %s!".formatted(name)
来源：http://rdo.bjfxy.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://tbx.zhijiandao.cn

Ruby: "Hello, #{name}!"
来源：http://oiv.yongpay.top

C#:   $"Hello, {name}!"
来源：http://kcb.daxiang520.top

[A13] 多行字符串（练习 \n 转义）
来源：http://amg.yvedp.cn

Py:   "第一行\n第二行"
来源：http://apx.ydzc1.top

PHP:  "第一行\n第二行"
来源：http://mjs.havefunace.top

JS:   "第一行\n第二行"
来源：http://yyy.hesvh.cn

TS:   "第一行\n第二行"
来源：http://qzi.zhaomingkeji.xyz

Java: "第一行\n第二行"
来源：http://esp.yuxming.cn

Go:   "第一行\n第二行"
来源：http://sqh.yueranfly.top

Ruby: "第一行\n第二行"
来源：http://rll.aizwys.cn

C#:   "第一行\n第二行"
来源：http://lev.zhoulong.xyz

[A14] 注释写法
来源：http://feg.zhixingplan.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://yrj.zhengqikj.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ysd.nanxuanxn.top

JS:   // 单行；/* 多行 */
来源：http://lsm.ydzc1.top

TS:   // 单行；/* 多行 */
来源：http://yqf.wangdashe.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://slf.hywenlv.cn

Go:   // 单行；/* 多行 */
来源：http://mnc.jianghu66.top

Ruby: # 单行；=begin 多行 =end
来源：http://nfm.hywenlv.cn

C#:   // 单行；/* 多行 */
来源：http://irb.sjlbkw.cn

[A15] 空值判断与默认值
来源：http://pwr.jqgufenzy.top

Py:   value = data or "默认值"
来源：http://ykd.xuanzx.com

PHP:  $value = $data ?? "默认值";
来源：http://zfn.xinyue.icu

JS:   const value = data ?? "默认值";
来源：http://vjv.feifeiyinyue.top

TS:   const value = data ?? "默认值";
来源：http://vfn.fzhhl.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://sia.zdqjudy.top

Go:   if data == "" { data = "默认值" }
来源：http://uyh.quarkkingdee.top

Ruby: value = data || "默认值"
来源：http://dfm.jinqigufen.top

C#:   var value = data ?? "默认值";
来源：http://wbc.dashuyun.cn

[A16] 真假值判断规则
来源：http://ifs.vehdjk.com

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://rfx.redwolf501.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://czr.haohaochexian.top

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mma.shangyingyoupin.top

TS:   if (!x) {}
来源：http://sil.ywan-chungtsiang.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://etx.pengpengdd.cyou

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://yuh.jiagoushi.top

Ruby: unless x            # nil 与 false 为假
来源：http://eed.kuanghao11.cn

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hki.sjlbkw.cn

[A17] 位运算
来源：http://eiv.yvedp.cn

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ehn.cucudq.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://bfn.sxryk.cn

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://shn.hongshengwenyu.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://nmf.chenjidiqi.icu

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ffq.ivvv.top

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://xtz.yj20258.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ujh.birdmap.top

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://rez.hnqzz.top

[A18] 字符与 ASCII 码互转
来源：http://ono.xinyue.icu

Py:   ord("A"); chr(65)
来源：http://srj.sjlbkw.cn

PHP:  ord("A"); chr(65)
来源：http://gif.zhijiandao.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://jff.mhx1999.top

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://xex.yuanzhike.top

Java: (int) 'A'; (char) 65
来源：http://xzh.gogol.net.cn

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ejn.zdbjq.cn

Ruby: "A".ord; 65.chr
来源：http://ily.havefunace.top

C#:   (int)'A'; (char)65
来源：http://lvu.pycfn.com

[A19] 交换两个变量
来源：http://grk.tanke756.top

Py:   a, b = b, a
来源：http://lre.redwolf501.top

PHP:  [$a, $b] = [$b, $a];
来源：http://gbx.vehdjk.com

JS:   [a, b] = [b, a];
来源：http://rvz.chenzaomai.com

TS:   [a, b] = [b, a];
来源：http://uua.wangshuangyany.cn

Java: int t = a; a = b; b = t;
来源：http://tpj.jinyuanbaomall.cn

Go:   a, b = b, a
来源：http://xay.yanxiufei.cn

Ruby: a, b = b, a
来源：http://dey.shanyushiyangtech.top

C#:   (a, b) = (b, a);
来源：http://hnl.fengsongda.top

[A20] 读取标准输入
来源：http://rks.yonumen.top

Py:   name = input("请输入：")
来源：http://bfz.zycfv.cn

PHP:  $name = trim(fgets(STDIN));
来源：http://blx.zhaomingkeji.xyz

JS:   // Node.js：readline 模块或 process.stdin
来源：http://whz.zhoulong.xyz

TS:   // Node.js：readline 模块
来源：http://nxq.meibo888.top

Java: new Scanner(System.in).nextLine()
来源：http://pgf.feifeiyinyue.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hje.fzhhl.top

Ruby: gets.chomp
来源：http://msn.guowangkeji.top

C#:   Console.ReadLine();
来源：http://lax.zycfv.cn

[A21] 保留指定小数位输出
来源：http://sad.tarul.cn

Py:   f"{3.14159:.2f}"
来源：http://zle.ydzc1.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://zps.snrcjt.cn

JS:   (3.14159).toFixed(2)
来源：http://tcd.jinqigfzy.top

TS:   (3.14159).toFixed(2)
来源：http://uth.cashguo.top

Java: String.format("%.2f", 3.14159)
来源：http://rso.gzhubu.top

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://yyo.ydzc1.top

Ruby: format("%.2f", 3.14159)
来源：http://phr.bbcook.cn

C#:   3.14159.ToString("F2")
来源：http://qsh.guowangkeji.top

[A22] 获取字符串长度
来源：http://kuo.aibaodan.cn

Py:   len(s)
来源：http://qxb.jqgufenzy.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://ton.pengpengdd.cyou

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wom.yongpay.top

TS:   s.length
来源：http://kcr.andypj.xyz

Java: s.length()
来源：http://gbu.nwbrower.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://snh.ivvv.top

Ruby: s.length
来源：http://ofu.dashuyun.cn

C#:   s.Length
来源：http://xal.shzxlz.cn

[A23] 大小写转换
来源：http://zjm.sjlbkw.cn

Py:   s.upper(); s.lower(); s.title()
来源：http://nem.yj20258.top

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://vmv.svipenyu.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://ipq.quarkkingdee.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://aip.sjlbkw.cn

Java: s.toUpperCase(); s.toLowerCase()
来源：http://jxu.shuidangran.top

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://sog.nanxinkj.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://nkm.mhx1999.top

C#:   s.ToUpper(); s.ToLower()
来源：http://dob.hammf.cn

[A24] 去除首尾空白
来源：http://zkf.gogol.net.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dvv.ehwqpu.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://opt.9152youxi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://yjv.guannengcc.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://gec.hesvh.cn

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://mmi.redwolf501.top

Go:   strings.TrimSpace(s)
来源：http://bnf.yj20258.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://bmx.ppjwa.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mor.chenzaomai.com

[A25] 字符串比较
来源：http://epl.jiagoushi.top

Py:   s1 == s2; s1 != s2
来源：http://quv.hcnkem.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://cte.guannengcc.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://qho.cucudq.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://bve.pengpengdd.cyou

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kzo.jinqigufen.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://uoc.zhixingplan.top

Ruby: s1 == s2; s1 <=> s2
来源：http://soi.birdmap.top

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://izo.ehwqpu.com

[A26] 类型转换总览
来源：http://oqf.nanxinkj.top

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ncv.shanyushiyangtech.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wip.0kj1m.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://caz.jinqigfzy.top

TS:   Number() String() Boolean() x as number
来源：http://lio.tanke756.top

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://zan.shanyushiyangtech.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://uya.yvedp.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://zay.redwolf501.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://lew.316326.xyz

================================================================================
来源：http://qqk.tian-w.cn

B. 流程控制
来源：http://jjb.yj202588.top

================================================================================
来源：http://ztk.xinyue.icu

[B01] 条件判断 if / else
来源：http://fmd.yvedp.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://jnm.shuidangran.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://jca.nanxinkj.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://lmm.snrcjt.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://ncs.xuetiantiany.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://xbv.jinqigufen.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://zox.hnqzz.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://evt.fengsongda.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://sql.aizwys.cn

[B02] 多分支 else if / elif
来源：http://xse.ydzc1.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://ade.xziqi.cn

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ulx.gogol.net.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vyb.zhoulong.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://cws.cashguo.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://fzl.sufxvd.cn

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://eak.yuxming.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://iby.jlsjyb.cn

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hkj.jyoumei.cn

[B03] switch / match / case
来源：http://yvb.jyoumei.cn

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://cga.cdnleiting.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://zgu.xinyue.icu

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://svc.fengsongda.top

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://sre.ctjpmb.com

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hdr.nanxinkj.top

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://uok.yj202588.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://twj.epnwcf.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://lqd.zhiwuduotai.top

[B04] for 计数循环
来源：http://crl.mhx1999.top

Py:   for i in range(10): print(i)
来源：http://dvy.yj20258.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://gfa.gzhubu.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wxy.jyoumei.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hii.xziqi.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://llw.ydzc1.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hrz.daria6918.cn

Ruby: 10.times { |i| puts i }
来源：http://sug.andypj.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hhs.jlsjyb.cn

[B05] 遍历数组 / 列表
来源：http://gmh.tianlin.xyz

Py:   for item in arr: print(item)
来源：http://cnp.yueranfly.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mkn.zdqjudy.top

JS:   for (const item of arr) { console.log(item); }
来源：http://vke.52xcode.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://evm.fktsv.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://rst.feifeiyinyue.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://ari.nanxinkj.top

Ruby: arr.each { |item| puts item }
来源：http://cww.dianchejie.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://dgd.hcnkem.com

[B06] 遍历字典 / 对象
来源：http://vwd.zdqjudy.top

Py:   for k, v in d.items(): print(k, v)
来源：http://caf.nanxinkj.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://gzs.ctjpmb.com

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://bhl.sysykeji.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wur.hysaishi.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://ifd.chenzaomai.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://jno.birdmap.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://neg.cheryme.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://cbv.jianghu66.top

[B07] while 循环
来源：http://him.birdmap.top

Py:   while i < 10: i += 1
来源：http://vrz.shangyingyoupin.top

PHP:  while ($i < 10) { $i++; }
来源：http://mzu.9152youxi.cn

JS:   while (i < 10) { i++; }
来源：http://njr.yuxming.cn

TS:   while (i < 10) { i++; }
来源：http://ecw.zdqjudy.top

Java: while (i < 10) { i++; }
来源：http://ukj.shangyingyoupin.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://fhn.jqgufenzy.top

Ruby: while i < 10; i += 1; end
来源：http://bbr.zhijiandao.cn

C#:   while (i < 10) { i++; }
来源：http://szs.hywenlv.cn

[B08] do-while（至少执行一次）
来源：http://icu.haohaochexian.top

Py:   # 无 do-while：用 while True + break
来源：http://lmq.chenjidiqi.icu

PHP:  do { $i++; } while ($i < 10);
来源：http://hgy.zycfv.cn

JS:   do { i++; } while (i < 10);
来源：http://nba.52xcode.cn

TS:   do { i++; } while (i < 10);
来源：http://pev.redwolf501.top

Java: do { i++; } while (i < 10);
来源：http://mtu.daria6918.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://dpt.jqgufenzy.top

Ruby: begin; i += 1; end while i < 10
来源：http://suk.zhongyouzk.top

C#:   do { i++; } while (i < 10);
来源：http://chm.zhoulong.xyz

[B09] break 与 continue
来源：http://zxj.yfazqb.com

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://taj.sjlbkw.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://ucr.hnqzz.top

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://thx.yonumen.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://soe.uphjek.com

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ozl.jinqigufen.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://kuf.iojbl.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wzo.zhongyouzk.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://czp.nanxinkj.top

[B10] 遍历同时拿索引
来源：http://pal.fehbvm.com

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://jxt.chenjidiqi.icu

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://rfy.wangshuangyany.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://rrf.hfpthk.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://bef.ctjpmb.com

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://esj.316326.xyz

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://ybc.dashuyun.cn

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://tfo.meibo888.top

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://vxx.hysaishi.cn

[B11] 生成数字序列 / 区间
来源：http://ziu.birdmap.top

Py:   list(range(0, 10, 2))
来源：http://zew.gotoacloud.top

PHP:  range(0, 10, 2);
来源：http://ejo.cashguo.top

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://ttd.jinyuanbaomall.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://lyr.guowangkeji.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://dhy.mhx1999.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://lux.sysykeji.top

Ruby: (0...10).step(2).to_a
来源：http://kzi.xinyue.icu

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vji.zhongyouzk.top

[B12] 跳出多层循环
来源：http://vpe.ivvv.top

Py:   # 无标签跳转：抽成函数用 return
来源：http://kmf.vqdsnc.cn

PHP:  # 无标签：用 goto 或函数返回
来源：http://omz.hfpthk.cn

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://giv.birdmap.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://bta.0kj1m.cn

Java: outer: for (...) { for (...) { break outer; } }
来源：http://kzv.kuanghao11.cn

Go:   # 无标签：用布尔标志或抽成函数
来源：http://bud.vehdjk.com

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://cvx.shanyushiyangkeji.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://feo.cqqwz.cn

[B13] 判断是否为数字
来源：http://soa.sysykeji.top

Py:   isinstance(x, (int, float))
来源：http://dyu.cucudq.cn

PHP:  is_numeric($x)
来源：http://mnf.zhiwuduotai.top

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mjv.ywan-chungtsiang.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://sxv.hammf.cn

Java: x instanceof Number
来源：http://ijq.hesvh.cn

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://xhm.xinyue.icu

Ruby: x.is_a?(Numeric)
来源：http://kcd.ehwqpu.com

C#:   x is int or double or decimal
来源：http://yvf.zdqjudy.top

[B14] 判断值是否在集合内
来源：http://qbx.yanxiufei.cn

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://vek.hnxiangtu.top

PHP:  in_array($x, [1, 2, 3], true)
来源：http://jmc.redwolf501.top

JS:   [1, 2, 3].includes(x)
来源：http://yfd.yanxiufei.cn

TS:   [1, 2, 3].includes(x)
来源：http://oed.dashuyun.cn

Java: List.of(1, 2, 3).contains(x)
来源：http://ytp.zhoulong.xyz

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://ksn.yuxming.cn

Ruby: [1, 2, 3].include?(x)
来源：http://sfs.guowangkeji.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://czb.ydzc1.top

[B15] 布尔运算与取反
来源：http://ilz.jiagoushi.top

Py:   a and b or not c
来源：http://wtu.hongshengwenyu.top

PHP:  $a && $b || !$c
来源：http://rqa.zycfv.cn

JS:   a && b || !c
来源：http://jey.jqgfzy.top

TS:   a && b || !c
来源：http://ujl.yj20258.top

Java: a && b || !c
来源：http://eqt.wangshuangyany.cn

Go:   a && b || !c
来源：http://olv.yvedp.cn

Ruby: a && b || !c
来源：http://kpw.chenlongwang.top

C#:   a && b || !c
来源：http://iwi.jlsjyb.cn

[B16] 卫语句：不满足条件提前返回
来源：http://hpb.hcnkem.com

Py:   if not data: return
来源：http://qdj.dashuyun.cn

PHP:  if (!$data) { return; }
来源：http://sfd.ydjk.org.cn

JS:   if (!data) return;
来源：http://jxw.fzhhl.top

TS:   if (!data) return;
来源：http://nnq.snrcjt.cn

Java: if (data == null) return;
来源：http://qoh.svipenyu.cn

Go:   if data == nil { return }
来源：http://flz.snrcjt.cn

Ruby: return if data.nil?
来源：http://zok.jinqigfzy.top

C#:   if (data == null) return;
来源：http://imf.bbcook.cn

================================================================================
来源：http://qja.zdbjq.cn

C. 函数与作用域
来源：http://tkv.vqdsnc.cn

================================================================================
来源：http://iat.xingfuxueyuan.xyz

[C01] 定义函数
来源：http://xui.jqgfzy.top

Py:   def add(a, b): return a + b
来源：http://hji.ydjk.org.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mmh.feifeiyinyue.top

JS:   function add(a, b) { return a + b; }
来源：http://lwt.9152youxi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://nfe.andypj.xyz

Java: static int add(int a, int b) { return a + b; }
来源：http://rib.zycfv.cn

Go:   func add(a, b int) int { return a + b }
来源：http://vdj.chenzaomai.com

Ruby: def add(a, b); a + b; end
来源：http://zhg.pycfn.com

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hvr.zhijiandao.cn

[C02] 默认参数
来源：http://wat.cdnleiting.top

Py:   def greet(name="World"): return name
来源：http://nzg.birdmap.top

PHP:  function greet($name = "World") { return $name; }
来源：http://gdb.fanxiaobao.xyz

JS:   function greet(name = "World") { return name; }
来源：http://bxr.fehbvm.com


<!-- 参考信息 -->