代发 wailian999

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://oml.gzhubu.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://lax.tian-w.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://lsg.jiagoushi.top

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://nfh.tarul.cn

Java: 7 / 2; 7 % 2
来源：http://vrj.ctjpmb.com

Go:   7 / 2; 7 % 2
来源：http://hdc.yfazqb.com

Ruby: 7 / 2; 7 % 2
来源：http://xie.yanxiufei.cn

C#:   7 / 2; 7 % 2
来源：http://njy.yj20258.top

[A06] 字符串转数字
来源：http://lul.mhx1999.top

Py:   int("42"); float("3.14")
来源：http://jew.jiagoushi.top

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://lhz.cqqwz.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://kvr.shangyingyoupin.top

TS:   parseInt("42", 10); Number("42")
来源：http://nbh.yuxming.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://vih.hcnkem.com

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://tcw.zdqjudy.top

Ruby: "42".to_i; "3.14".to_f
来源：http://jrd.jqgfzy.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://wku.xingfuxueyuan.xyz

[A07] 数字转字符串
来源：http://jrw.jiagoushi.top

Py:   str(42)
来源：http://spd.shanyushiyangkeji.top

PHP:  (string) 42; strval(42)
来源：http://myp.uphjek.com

JS:   String(42); (42).toString()
来源：http://bkg.mhx1999.top

TS:   String(42)
来源：http://iym.sweek.top

Java: String.valueOf(42); Integer.toString(42)
来源：http://sco.haohaochexian.top

Go:   strconv.Itoa(42)
来源：http://nwr.gotoacloud.top

Ruby: 42.to_s
来源：http://cjo.jianghu66.top

C#:   42.ToString()
来源：http://fos.316326.xyz

[A08] 取整与四舍五入
来源：http://kff.hesvh.cn

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://ihx.cucudq.cn

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://aey.c1oappe.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://btb.yj20258.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://mjo.sjlbkw.cn

Java: Math.round(3.567); Math.floor(3.9)
来源：http://zby.zhijiandao.cn

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://gjf.zycfv.cn

Ruby: 3.567.round(2); 3.9.floor
来源：http://gcm.kuanghao11.cn

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://vpj.cqqwz.cn

[A09] 绝对值与最大最小值
来源：http://zcn.ybcxt.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://wft.zhengqikj.top

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://orb.sysykeji.top

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://ipa.cashguo.top

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hcg.52xcode.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://lpp.zdbjq.cn

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://sau.yonumen.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://gss.guannengcc.top

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://xec.guannengcc.top

[A10] 生成随机数
来源：http://ziv.chenlongwang.top

Py:   import random; random.randint(1, 100)
来源：http://zgl.shanyushiyangkeji.top

PHP:  random_int(1, 100);
来源：http://svq.yuxming.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://rqn.smart0.xyz

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hpd.jianghu66.top

Java: new Random().nextInt(100) + 1
来源：http://cwu.jianghu66.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://kil.zhiwuduotai.top

Ruby: rand(1..100)
来源：http://mne.tianlin.xyz

C#:   new Random().Next(1, 101)
来源：http://chs.hysaishi.cn

[A11] 条件表达式（三元）
来源：http://pep.birdmap.top

Py:   "yes" if x > 0 else "no"
来源：http://gbg.xziqi.cn

PHP:  $x > 0 ? "yes" : "no"
来源：http://kqd.ctjpmb.com

JS:   x > 0 ? "yes" : "no"
来源：http://nhe.uphjek.com

TS:   x > 0 ? "yes" : "no"
来源：http://axp.zdbjq.cn

Java: x > 0 ? "yes" : "no"
来源：http://rhv.gotoacloud.top

Go:   // 无三元运算符，需用 if 语句
来源：http://pfb.wangdashe.top

Ruby: x > 0 ? "yes" : "no"
来源：http://von.sxryk.cn

C#:   x > 0 ? "yes" : "no"
来源：http://kbh.hnxiangtu.top

[A12] 字符串插值 / 格式化
来源：http://cxz.bbcook.cn

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://bwk.jiagoushi.top

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://zsh.chenzaomai.com

JS:   `Hello, ${name}!`
来源：http://upw.gogol.net.cn

TS:   `Hello, ${name}!`
来源：http://cpt.ybcxt.top

Java: "Hello, %s!".formatted(name)
来源：http://lzl.yongpay.top

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://upf.hesvh.cn

Ruby: "Hello, #{name}!"
来源：http://irh.yangfankeji.com

C#:   $"Hello, {name}!"
来源：http://tef.xingfuxueyuan.xyz

[A13] 多行字符串（练习 \n 转义）
来源：http://dih.fanxiaobao.xyz

Py:   "第一行\n第二行"
来源：http://ffu.svipenyu.cn

PHP:  "第一行\n第二行"
来源：http://wtc.nwbrower.top

JS:   "第一行\n第二行"
来源：http://mgk.zhaomingkeji.xyz

TS:   "第一行\n第二行"
来源：http://zjt.sjlbkw.cn

Java: "第一行\n第二行"
来源：http://ejf.iojbl.cn

Go:   "第一行\n第二行"
来源：http://hfm.ybcxt.top

Ruby: "第一行\n第二行"
来源：http://psg.yangfankeji.com

C#:   "第一行\n第二行"
来源：http://dmt.fengsongda.top

[A14] 注释写法
来源：http://zdv.wangshuangyany.cn

Py:   # 单行；三引号字符串可作多行说明
来源：http://wot.gaohongyu789.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://ott.yangfankeji.com

JS:   // 单行；/* 多行 */
来源：http://rvu.fktsv.cn

TS:   // 单行；/* 多行 */
来源：http://eca.sweek.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://ykc.jinqigufen.top

Go:   // 单行；/* 多行 */
来源：http://rxc.316326.xyz

Ruby: # 单行；=begin 多行 =end
来源：http://wjw.pengpengdd.cyou

C#:   // 单行；/* 多行 */
来源：http://sxk.jinqigufen.top

[A15] 空值判断与默认值
来源：http://aqz.yangfankeji.com

Py:   value = data or "默认值"
来源：http://nnc.cashguo.top

PHP:  $value = $data ?? "默认值";
来源：http://lhh.ivvv.top

JS:   const value = data ?? "默认值";
来源：http://mfx.yangfankeji.com

TS:   const value = data ?? "默认值";
来源：http://xhc.zhengqikj.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://ngl.yj20258888.top

Go:   if data == "" { data = "默认值" }
来源：http://xmp.fzhhl.top

Ruby: value = data || "默认值"
来源：http://bvl.jinqigufen.top

C#:   var value = data ?? "默认值";
来源：http://eek.yj20258.top

[A16] 真假值判断规则
来源：http://btu.cucudq.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://dau.sjlbkw.cn

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://elg.jyoumei.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hmp.yongpay.top

TS:   if (!x) {}
来源：http://asp.zhiwuduotai.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://gmy.zdbjq.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://suh.ivvv.top

Ruby: unless x            # nil 与 false 为假
来源：http://szw.shanyushiyangkeji.top

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://uye.wangshuangyany.cn

[A17] 位运算
来源：http://odu.gzhubu.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wzm.sxryk.cn

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://zpy.gotoacloud.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://cfg.meibo888.top

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://imf.zhengqikj.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vfs.xylfe.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://jts.sxryk.cn

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://vdj.xuanzx.com

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://yze.meibo888.top

[A18] 字符与 ASCII 码互转
来源：http://vme.fktsv.cn

Py:   ord("A"); chr(65)
来源：http://ygz.tian-w.cn

PHP:  ord("A"); chr(65)
来源：http://keo.cucudq.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://ady.tianlin.xyz

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://tfm.iojbl.cn

Java: (int) 'A'; (char) 65
来源：http://ewx.xuanzx.com

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://tyr.shangyingyoupin.top

Ruby: "A".ord; 65.chr
来源：http://dwz.yuxming.cn

C#:   (int)'A'; (char)65
来源：http://cnz.shanyushiyangtech.top

[A19] 交换两个变量
来源：http://znv.zycfv.cn

Py:   a, b = b, a
来源：http://vnq.hnqzz.top

PHP:  [$a, $b] = [$b, $a];
来源：http://juw.jiagoushi.top

JS:   [a, b] = [b, a];
来源：http://gkq.dashuyun.cn

TS:   [a, b] = [b, a];
来源：http://ykp.hcnkem.com

Java: int t = a; a = b; b = t;
来源：http://ovi.jinqigfzy.top

Go:   a, b = b, a
来源：http://yqx.yangfankeji.com

Ruby: a, b = b, a
来源：http://hox.quarkkingdee.top

C#:   (a, b) = (b, a);
来源：http://cvy.xuanzx.com

[A20] 读取标准输入
来源：http://gyr.sufxvd.cn

Py:   name = input("请输入：")
来源：http://hwo.vehdjk.com

PHP:  $name = trim(fgets(STDIN));
来源：http://jxf.nanxinkj.top

JS:   // Node.js：readline 模块或 process.stdin
来源：http://eba.bjfxy.top

TS:   // Node.js：readline 模块
来源：http://vtg.yuxming.cn

Java: new Scanner(System.in).nextLine()
来源：http://esw.yongpay.top

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://qoa.hfpthk.cn

Ruby: gets.chomp
来源：http://mex.zhongyouzk.top

C#:   Console.ReadLine();
来源：http://cha.yfazqb.com

[A21] 保留指定小数位输出
来源：http://rjx.guannengcc.top

Py:   f"{3.14159:.2f}"
来源：http://jpn.tanke756.top

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ten.bjfxy.top

JS:   (3.14159).toFixed(2)
来源：http://yji.smart0.xyz

TS:   (3.14159).toFixed(2)
来源：http://edg.zhongyouzk.top

Java: String.format("%.2f", 3.14159)
来源：http://ies.xinyue.icu

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://ssg.xuetiantiany.cn

Ruby: format("%.2f", 3.14159)
来源：http://wni.aizwys.cn

C#:   3.14159.ToString("F2")
来源：http://rdn.fengsongda.top

[A22] 获取字符串长度
来源：http://hkj.tian-w.cn

Py:   len(s)
来源：http://qow.guannengcc.top

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://vxv.cqqwz.cn

JS:   s.length                          # 按 UTF-16 单元计
来源：http://aed.yuanzhike.top

TS:   s.length
来源：http://dht.shanyushiyangtech.top

Java: s.length()
来源：http://aaf.dashuyun.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://qqo.meibo888.top

Ruby: s.length
来源：http://xzi.bbcook.cn

C#:   s.Length
来源：http://ucu.yuxming.cn

[A23] 大小写转换
来源：http://xbb.hongshengwenyu.top

Py:   s.upper(); s.lower(); s.title()
来源：http://ymb.dashuyun.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://adl.ywan-chungtsiang.top

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://yol.hysaishi.cn

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://pdw.chenjidiqi.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://sxr.gogol.net.cn

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://jnl.xuanzx.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://cck.shanyushiyangkeji.top

C#:   s.ToUpper(); s.ToLower()
来源：http://enk.shuidangran.top

[A24] 去除首尾空白
来源：http://bug.xylfe.cn

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://woh.cqqwz.cn

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://ofe.9152youxi.cn

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://qem.yj202588.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://vsn.yueranfly.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://jty.pengpengdd.cyou

Go:   strings.TrimSpace(s)
来源：http://mxe.shanyushiyangtech.top

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hhr.jinyuanbaomall.cn

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hvi.zhoulong.xyz

[A25] 字符串比较
来源：http://ohu.kuanghao11.cn

Py:   s1 == s2; s1 != s2
来源：http://qwp.yangfankeji.com

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://fuh.havefunace.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://kst.snrcjt.cn

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://gpg.yangfankeji.com

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://ygf.fengsongda.top

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://zvs.xylfe.cn

Ruby: s1 == s2; s1 <=> s2
来源：http://qro.snrcjt.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://zfb.hnxiangtu.top

[A26] 类型转换总览
来源：http://wga.jyoumei.cn

Py:   int() float() str() bool() list() dict() tuple()
来源：http://vwj.chenzaomai.com

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rmq.sysykeji.top

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://zfk.ctjpmb.com

TS:   Number() String() Boolean() x as number
来源：http://zsw.tarul.cn

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://koa.ppjwa.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://krc.ehwqpu.com

Ruby: to_i to_f to_s to_sym to_a
来源：http://tym.xingfuxueyuan.xyz

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mln.yueranfly.top

================================================================================
来源：http://fao.meibo888.top

B. 流程控制
来源：http://lds.sufxvd.cn

================================================================================
来源：http://pvv.sufxvd.cn

[B01] 条件判断 if / else
来源：http://nub.jyoumei.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://wys.dashuyun.cn

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://tas.sjlbkw.cn

JS:   const r = x > 0 ? "正" : "非正";
来源：http://dww.9152youxi.cn

TS:   const r = x > 0 ? "正" : "非正";
来源：http://lqi.dashuyun.cn

Java: String r = x > 0 ? "正" : "非正";
来源：http://heu.tian-w.cn

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://dzb.yj20258.top

Ruby: r = x > 0 ? "正" : "非正"
来源：http://yoi.xziqi.cn

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wyg.svipenyu.cn

[B02] 多分支 else if / elif
来源：http://tjj.jlsjyb.cn

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://qsp.nanxuanxn.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://kja.zhaomingkeji.xyz

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pap.tanke756.top

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://pfz.andypj.xyz

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://nsx.daxiang520.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://ykz.jyoumei.cn

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://fsi.guowangkeji.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://dqf.wangdashe.top

[B03] switch / match / case
来源：http://tud.jiagoushi.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://ywo.cheryme.top

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://icx.fzhhl.top

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://lqg.chenzaomai.com

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://eto.nanxinkj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://iyf.xinyue.icu

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://nes.sysykeji.top

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://kag.meibo888.top

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://nkp.yuanzhike.top

[B04] for 计数循环
来源：http://fnr.guowangkeji.top

Py:   for i in range(10): print(i)
来源：http://lyr.hnqzz.top

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://ueh.tianlin.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://yxg.yj202588.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://vmg.jinqigfzy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://pbu.kuanghao11.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://ich.ppjwa.cn

Ruby: 10.times { |i| puts i }
来源：http://xsf.andypj.xyz

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://lts.yangfankeji.com

[B05] 遍历数组 / 列表
来源：http://nky.yangfankeji.com

Py:   for item in arr: print(item)
来源：http://yff.nanxuanxn.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://boa.nwbrower.top

JS:   for (const item of arr) { console.log(item); }
来源：http://tek.jinghuilouyu.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://tli.redwolf501.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://hua.9152youxi.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://zoi.zhaomingkeji.xyz

Ruby: arr.each { |item| puts item }
来源：http://ied.tian-w.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://qjv.quarkkingdee.top

[B06] 遍历字典 / 对象
来源：http://swk.epnwcf.com

Py:   for k, v in d.items(): print(k, v)
来源：http://wid.yj20258.top

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://bca.hfpthk.cn

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://drn.jiagoushi.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://qae.jinqigufen.top

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://qkl.uphjek.com

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://fcd.zhijiandao.cn

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://zym.birdmap.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://nsi.jiagoushi.top

[B07] while 循环
来源：http://gjf.fengsongda.top

Py:   while i < 10: i += 1
来源：http://mow.hongshengwenyu.top

PHP:  while ($i < 10) { $i++; }
来源：http://ycn.nwbrower.top

JS:   while (i < 10) { i++; }
来源：http://ylg.sufxvd.cn

TS:   while (i < 10) { i++; }
来源：http://kyl.ydjk.org.cn

Java: while (i < 10) { i++; }
来源：http://kej.shanyushiyangkeji.top

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://aom.hywenlv.cn

Ruby: while i < 10; i += 1; end
来源：http://hpy.guannengcc.top

C#:   while (i < 10) { i++; }
来源：http://myl.zdqjudy.top

[B08] do-while（至少执行一次）
来源：http://snl.bbcook.cn

Py:   # 无 do-while：用 while True + break
来源：http://lrj.ehwqpu.com

PHP:  do { $i++; } while ($i < 10);
来源：http://mql.tian-w.cn

JS:   do { i++; } while (i < 10);
来源：http://bcu.52xcode.cn

TS:   do { i++; } while (i < 10);
来源：http://pol.ivvv.top

Java: do { i++; } while (i < 10);
来源：http://ifp.feifeiyinyue.top

Go:   for { i++; if i >= 10 { break } }
来源：http://rjy.52xcode.cn

Ruby: begin; i += 1; end while i < 10
来源：http://beh.yangfankeji.com

C#:   do { i++; } while (i < 10);
来源：http://nkp.nanxinkj.top

[B09] break 与 continue
来源：http://ect.nwbrower.top

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://nvu.cheryme.top

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hoj.epnwcf.com

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://ssl.yj202588.top

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://aeo.316326.xyz

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://fqg.chenlongwang.top

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://lpl.316326.xyz

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://rox.sysykeji.top

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://zst.fengsongda.top

[B10] 遍历同时拿索引
来源：http://fug.shanyushiyangtech.top

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://lve.yuxming.cn

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mym.c1oappe.top

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://fmm.ehwqpu.com

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://dnl.tanke756.top

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hxe.snrcjt.cn

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hsg.hnqzz.top

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://yqo.xinyue.icu

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://lyo.tarul.cn

[B11] 生成数字序列 / 区间
来源：http://yrr.tarul.cn

Py:   list(range(0, 10, 2))
来源：http://qto.yongpay.top

PHP:  range(0, 10, 2);
来源：http://dgm.tian-w.cn

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://tpz.sufxvd.cn

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://nxq.zhengqikj.top

Java: IntStream.range(0, 10).boxed().toList()
来源：http://rjf.yj20258.top

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://dsg.jqgufenzy.top

Ruby: (0...10).step(2).to_a
来源：http://aku.ppjwa.cn

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://vcj.redwolf501.top

[B12] 跳出多层循环
来源：http://lcs.yj20258888.top


<!-- 参考信息 -->