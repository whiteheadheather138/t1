代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://fje.sysykeji.top

Java: new Random().nextInt(100) + 1
来源：http://xwr.ctjpmb.com

Go:   rand.Intn(100) + 1               // math/rand
来源：http://exa.xingfuxueyuan.xyz

Ruby: rand(1..100)
来源：http://mkl.uphjek.com

C#:   new Random().Next(1, 101)
来源：http://thh.feifeiyinyue.top

[A11] 条件表达式（三元）
来源：http://bez.shanyushiyangkeji.top

Py:   "yes" if x > 0 else "no"
来源：http://ifp.wangshuangyany.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://ubb.fehbvm.com

JS:   x > 0 ? "yes" : "no"
来源：http://qud.gogol.net.cn

TS:   x > 0 ? "yes" : "no"
来源：http://xsm.nanxuanxn.top

Java: x > 0 ? "yes" : "no"
来源：http://lop.aibaodan.cn

Go:   // 无三元运算符，需用 if 语句
来源：http://rsj.zhijiandao.cn

Ruby: x > 0 ? "yes" : "no"
来源：http://spc.xuanzx.com

C#:   x > 0 ? "yes" : "no"
来源：http://xtp.sjlbkw.cn

[A12] 字符串插值 / 格式化
来源：http://ezg.epnwcf.com

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://yom.ydjk.org.cn

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://wsf.yj20258888.top

JS:   `Hello, ${name}!`
来源：http://zbl.ydjk.org.cn

TS:   `Hello, ${name}!`
来源：http://xam.jinghuilouyu.cn

Java: "Hello, %s!".formatted(name)
来源：http://orp.jiagoushi.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://kew.tanke756.top

Ruby: "Hello, #{name}!"
来源：http://hzi.jlsjyb.cn

C#:   $"Hello, {name}!"
来源：http://hhh.aibaodan.cn

[A13] 多行字符串（练习 \n 转义）
来源：http://leb.cqqwz.cn

Py:   "第一行\n第二行"
来源：http://lzc.jinqigufen.top

PHP:  "第一行\n第二行"
来源：http://hfz.yj20258888.top

JS:   "第一行\n第二行"
来源：http://chr.cqqwz.cn

TS:   "第一行\n第二行"
来源：http://ulh.fktsv.cn

Java: "第一行\n第二行"
来源：http://ncr.andypj.xyz

Go:   "第一行\n第二行"
来源：http://yme.shangyingyoupin.top

Ruby: "第一行\n第二行"
来源：http://imt.hnxiangtu.top

C#:   "第一行\n第二行"
来源：http://ggn.fengsongda.top

[A14] 注释写法
来源：http://qgz.dianchejie.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://tju.birdmap.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://klt.jinqigufen.top

JS:   // 单行；/* 多行 */
来源：http://teq.jlsjyb.cn

TS:   // 单行；/* 多行 */
来源：http://klg.hnqzz.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://lun.xinyue.icu

Go:   // 单行；/* 多行 */
来源：http://tgi.yonumen.top

Ruby: # 单行；=begin 多行 =end
来源：http://oyo.fktsv.cn

C#:   // 单行；/* 多行 */
来源：http://dxe.ydjk.org.cn

[A15] 空值判断与默认值
来源：http://rrk.ybcxt.top

Py:   value = data or "默认值"
来源：http://uqw.pycfn.com

PHP:  $value = $data ?? "默认值";
来源：http://xvz.ehwqpu.com

JS:   const value = data ?? "默认值";
来源：http://dts.jiagoushi.top

TS:   const value = data ?? "默认值";
来源：http://fqq.yueranfly.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://kjx.fktsv.cn

Go:   if data == "" { data = "默认值" }
来源：http://byq.ydjk.org.cn

Ruby: value = data || "默认值"
来源：http://axf.hnxiangtu.top

C#:   var value = data ?? "默认值";
来源：http://sdt.redwolf501.top

[A16] 真假值判断规则
来源：http://ncw.yuanzhike.top

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dce.ivvv.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://cxd.xingfuxueyuan.xyz

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://lqn.c1oappe.top

TS:   if (!x) {}
来源：http://ohm.dashuyun.cn

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://tlu.chenzaomai.com

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://fgs.bjfxy.top

Ruby: unless x            # nil 与 false 为假
来源：http://hvc.yongpay.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://cfz.wangshuangyany.cn

[A17] 位运算
来源：http://kkv.zdqjudy.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yee.cheryme.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://jjb.bjfxy.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ufq.wangshuangyany.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://aht.sxryk.cn

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fan.sufxvd.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://yin.yangfankeji.com

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ets.xuetiantiany.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gde.ydjk.org.cn

[A18] 字符与 ASCII 码互转
来源：http://paz.yj20258888.top

Py:   ord("A"); chr(65)
来源：http://avs.jinghuilouyu.cn

PHP:  ord("A"); chr(65)
来源：http://qsy.xziqi.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://rvn.zhoulong.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://eed.shanyushiyangtech.top

Java: (int) 'A'; (char) 65
来源：http://cep.wangdashe.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://fmi.svipenyu.cn

Ruby: "A".ord; 65.chr
来源：http://haw.zhengqikj.top

C#:   (int)'A'; (char)65
来源：http://mea.gotoacloud.top

[A19] 交换两个变量
来源：http://bsg.gotoacloud.top

Py:   a, b = b, a
来源：http://syv.yueranfly.top

PHP:  [$a, $b] = [$b, $a];
来源：http://fuj.sufxvd.cn

JS:   [a, b] = [b, a];
来源：http://csz.yuxming.cn

TS:   [a, b] = [b, a];
来源：http://yoh.pycfn.com

Java: int t = a; a = b; b = t;
来源：http://unc.yj202588.top

Go:   a, b = b, a
来源：http://qkw.pycfn.com

Ruby: a, b = b, a
来源：http://lnn.hcnkem.com

C#:   (a, b) = (b, a);
来源：http://arv.tianlin.xyz

[A20] 读取标准输入
来源：http://psh.jiagoushi.top

Py:   name = input("请输入：")
来源：http://gef.jianghu66.top

PHP:  $name = trim(fgets(STDIN));
来源：http://pyo.fengsongda.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ris.jinyuanbaomall.cn

TS:   // Node.js：readline 模块
来源：http://rgh.jinyuanbaomall.cn

Java: new Scanner(System.in).nextLine()
来源：http://oyf.dianchejie.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://ufn.fktsv.cn

Ruby: gets.chomp
来源：http://ucr.jqgufenzy.top

C#:   Console.ReadLine();
来源：http://jfd.havefunace.top

[A21] 保留指定小数位输出
来源：http://pdo.nanxinkj.top

Py:   f"{3.14159:.2f}"
来源：http://jut.zhoulong.xyz

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://yma.zdqjudy.top

JS:   (3.14159).toFixed(2)
来源：http://mai.jyoumei.cn

TS:   (3.14159).toFixed(2)
来源：http://bjl.yonumen.top

Java: String.format("%.2f", 3.14159)
来源：http://ybl.sxryk.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://oqv.yanxiufei.cn

Ruby: format("%.2f", 3.14159)
来源：http://bog.yueranfly.top

C#:   3.14159.ToString("F2")
来源：http://niq.yanxiufei.cn

[A22] 获取字符串长度
来源：http://mwp.yonumen.top

Py:   len(s)
来源：http://ttg.ydjk.org.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://kva.gogol.net.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://apq.svipenyu.cn

TS:   s.length
来源：http://kcx.sxryk.cn

Java: s.length()
来源：http://ttw.bjfxy.top

Go:   len(s); utf8.RuneCountInString(s)
来源：http://bvo.316326.xyz

Ruby: s.length
来源：http://vuh.jinghuilouyu.cn

C#:   s.Length
来源：http://dqk.yuxming.cn

[A23] 大小写转换
来源：http://xae.tanke756.top

Py:   s.upper(); s.lower(); s.title()
来源：http://pjh.zhijiandao.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://dun.zhoulong.xyz

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://kkn.sxryk.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://ufw.bjfxy.top

Java: s.toUpperCase(); s.toLowerCase()
来源：http://qft.316326.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://duw.tanke756.top

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://sfs.shanyushiyangtech.top

C#:   s.ToUpper(); s.ToLower()
来源：http://aoh.hysaishi.cn

[A24] 去除首尾空白
来源：http://fkw.yj20258888.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://fax.zhiwuduotai.top

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wgv.xuanzx.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://zkx.dianchejie.cn

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://sht.vehdjk.com

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gom.ivvv.top

Go:   strings.TrimSpace(s)
来源：http://csk.jinyuanbaomall.cn

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://zeo.pengpengdd.cyou

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://jym.jinyuanbaomall.cn

[A25] 字符串比较
来源：http://qbd.zhengqikj.top

Py:   s1 == s2; s1 != s2
来源：http://htp.zhoulong.xyz

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://lca.hcnkem.com

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://rbr.ctjpmb.com

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://krz.yuxming.cn

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://pyg.sxryk.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://opr.yj20258888.top

Ruby: s1 == s2; s1 <=> s2
来源：http://vwz.hcnkem.com

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://bbn.ydzc1.top

[A26] 类型转换总览
来源：http://dqs.yangfankeji.com

Py:   int() float() str() bool() list() dict() tuple()
来源：http://ksb.dianchejie.cn

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://ogn.cashguo.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://tlp.zhaomingkeji.xyz

TS:   Number() String() Boolean() x as number
来源：http://okl.epnwcf.com

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://emo.gaohongyu789.top

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://eph.ivvv.top

Ruby: to_i to_f to_s to_sym to_a
来源：http://rmz.cashguo.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://keh.jinqigfzy.top

================================================================================
来源：http://tak.jyoumei.cn

B. 流程控制
来源：http://ist.zdbjq.cn

================================================================================
来源：http://pye.hammf.cn

[B01] 条件判断 if / else
来源：http://abq.jinyuanbaomall.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://iya.yueranfly.top

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://uvs.xuanzx.com

JS:   const r = x > 0 ? "正" : "非正";
来源：http://rku.jinqigfzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://siz.guowangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://bko.hammf.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dbb.yj202588.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://jhd.sysykeji.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://lfg.fktsv.cn

[B02] 多分支 else if / elif
来源：http://fbh.jiagoushi.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://dlh.yj202588.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://vjw.yanxiufei.cn

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://bpi.yueranfly.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vgm.zhiwuduotai.top

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://vou.xingfuxueyuan.xyz

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://nuw.yvedp.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://ubk.gaohongyu789.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://odj.yj20258.top

[B03] switch / match / case
来源：http://lhy.ehwqpu.com

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://djb.0kj1m.cn

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://uba.sweek.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://abp.vqdsnc.cn

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://cml.zhixingplan.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://umn.fanxiaobao.xyz

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://thy.fehbvm.com

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://dud.hcnkem.com

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://tqi.316326.xyz

[B04] for 计数循环
来源：http://xsc.nanxinkj.top

Py:   for i in range(10): print(i)
来源：http://sqj.yuxming.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://nvj.ydzc1.top

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://qfx.zycfv.cn

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://xav.dashuyun.cn

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://usp.tanke756.top

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://yor.zhiwuduotai.top

Ruby: 10.times { |i| puts i }
来源：http://nav.chenzaomai.com

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://nlc.jqgfzy.top

[B05] 遍历数组 / 列表
来源：http://zfg.daxiang520.top

Py:   for item in arr: print(item)
来源：http://pnz.zhixingplan.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://iho.hongshengwenyu.top

JS:   for (const item of arr) { console.log(item); }
来源：http://niq.sweek.top

TS:   for (const item of arr) { console.log(item); }
来源：http://vwn.aizwys.cn

Java: for (var item : arr) { System.out.println(item); }
来源：http://juw.yj20258888.top

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://jlx.yuanzhike.top

Ruby: arr.each { |item| puts item }
来源：http://tki.shangyingyoupin.top

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://cxz.hfpthk.cn

[B06] 遍历字典 / 对象
来源：http://vap.hnqzz.top

Py:   for k, v in d.items(): print(k, v)
来源：http://znc.hywenlv.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://loh.quarkkingdee.top

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://ixo.zdbjq.cn

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://gvf.yj20258888.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://fwe.pycfn.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://nhs.xuanzx.com

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://lkb.guowangkeji.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://xvr.chenlongwang.top

[B07] while 循环
来源：http://yey.hammf.cn

Py:   while i < 10: i += 1
来源：http://lzf.chenjidiqi.icu

PHP:  while ($i < 10) { $i++; }
来源：http://aua.sysykeji.top

JS:   while (i < 10) { i++; }
来源：http://xzs.nwbrower.top

TS:   while (i < 10) { i++; }
来源：http://ock.yj20258888.top

Java: while (i < 10) { i++; }
来源：http://eyp.zhiwuduotai.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://jyy.zhengqikj.top

Ruby: while i < 10; i += 1; end
来源：http://ywn.yuxming.cn

C#:   while (i < 10) { i++; }
来源：http://udr.gotoacloud.top

[B08] do-while（至少执行一次）
来源：http://ppu.gogol.net.cn

Py:   # 无 do-while：用 while True + break
来源：http://dfy.smart0.xyz

PHP:  do { $i++; } while ($i < 10);
来源：http://bez.andypj.xyz

JS:   do { i++; } while (i < 10);
来源：http://oeu.ywan-chungtsiang.top

TS:   do { i++; } while (i < 10);
来源：http://acb.jinghuilouyu.cn

Java: do { i++; } while (i < 10);
来源：http://dfk.dashuyun.cn

Go:   for { i++; if i >= 10 { break } }
来源：http://gxi.birdmap.top

Ruby: begin; i += 1; end while i < 10
来源：http://obn.ydzc1.top

C#:   do { i++; } while (i < 10);
来源：http://wfm.jqgfzy.top

[B09] break 与 continue
来源：http://fng.chenlongwang.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://bcj.9152youxi.cn

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mal.chenzaomai.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ddo.dianchejie.cn

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://vcl.iojbl.cn

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ytj.jyoumei.cn

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://rgx.daria6918.cn

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://odh.ppjwa.cn

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://dgn.havefunace.top

[B10] 遍历同时拿索引
来源：http://yjr.mhx1999.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://vok.zycfv.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://ige.jyoumei.cn

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://bsn.aizwys.cn

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://snb.316326.xyz

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://cdy.aizwys.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://van.hnxiangtu.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://utn.aizwys.cn

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://ozy.jinyuanbaomall.cn

[B11] 生成数字序列 / 区间
来源：http://tut.hysaishi.cn

Py:   list(range(0, 10, 2))
来源：http://uqy.hfpthk.cn

PHP:  range(0, 10, 2);
来源：http://nxu.iojbl.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tei.zycfv.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://klf.uphjek.com

Java: IntStream.range(0, 10).boxed().toList()
来源：http://zcx.sufxvd.cn

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://ppz.shanyushiyangtech.top

Ruby: (0...10).step(2).to_a
来源：http://bst.yonumen.top

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://nqt.xuanzx.com

[B12] 跳出多层循环
来源：http://cxl.fktsv.cn

Py:   # 无标签跳转：抽成函数用 return
来源：http://bnc.jianghu66.top

PHP:  # 无标签：用 goto 或函数返回
来源：http://pvn.meibo888.top

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://ejz.jianghu66.top

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://smp.ehwqpu.com

Java: outer: for (...) { for (...) { break outer; } }
来源：http://iom.ehwqpu.com

Go:   # 无标签：用布尔标志或抽成函数
来源：http://xzm.guowangkeji.top

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://zql.yuanzhike.top

C#:   # 无标签：用 goto label 或布尔标志
来源：http://bhy.fehbvm.com

[B13] 判断是否为数字
来源：http://kct.guannengcc.top

Py:   isinstance(x, (int, float))
来源：http://eqq.gaohongyu789.top

PHP:  is_numeric($x)
来源：http://xei.pengpengdd.cyou

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://aap.yonumen.top

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://iuv.tanke756.top

Java: x instanceof Number
来源：http://mpx.zhongyouzk.top

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://qqv.chenlongwang.top

Ruby: x.is_a?(Numeric)
来源：http://els.epnwcf.com

C#:   x is int or double or decimal
来源：http://wbk.vehdjk.com

[B14] 判断值是否在集合内
来源：http://shh.yonumen.top

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://xvo.yuxming.cn

PHP:  in_array($x, [1, 2, 3], true)
来源：http://vsx.c1oappe.top

JS:   [1, 2, 3].includes(x)
来源：http://oke.svipenyu.cn

TS:   [1, 2, 3].includes(x)
来源：http://whn.fengsongda.top

Java: List.of(1, 2, 3).contains(x)
来源：http://sqc.iojbl.cn

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mfm.redwolf501.top

Ruby: [1, 2, 3].include?(x)
来源：http://qva.cashguo.top

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://cwt.guowangkeji.top

[B15] 布尔运算与取反
来源：http://oag.tian-w.cn

Py:   a and b or not c
来源：http://enq.shangyingyoupin.top

PHP:  $a && $b || !$c
来源：http://vau.yuxming.cn

JS:   a && b || !c
来源：http://mrc.shangyingyoupin.top

TS:   a && b || !c
来源：http://xvu.ivvv.top

Java: a && b || !c
来源：http://gal.hnqzz.top

Go:   a && b || !c
来源：http://pnb.gaohongyu789.top

Ruby: a && b || !c
来源：http://aiv.yueranfly.top

C#:   a && b || !c
来源：http://svn.cashguo.top

[B16] 卫语句：不满足条件提前返回
来源：http://nnm.jiagoushi.top

Py:   if not data: return
来源：http://jqo.shangyingyoupin.top

PHP:  if (!$data) { return; }
来源：http://cix.cashguo.top

JS:   if (!data) return;
来源：http://efc.sysykeji.top

TS:   if (!data) return;
来源：http://ikr.c1oappe.top

Java: if (data == null) return;
来源：http://pfg.hammf.cn

Go:   if data == nil { return }
来源：http://etg.redwolf501.top

Ruby: return if data.nil?
来源：http://kxn.chenzaomai.com

C#:   if (data == null) return;
来源：http://emp.hnxiangtu.top

================================================================================
来源：http://tzg.svipenyu.cn

C. 函数与作用域
来源：http://meh.dashuyun.cn

================================================================================
来源：http://gwn.daria6918.cn

[C01] 定义函数
来源：http://kmf.jinqigufen.top


<!-- 参考信息 -->