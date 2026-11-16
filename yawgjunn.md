代发 wailian999

================================================================================
来源：http://hjb.zhijiandao.cn

A. 基础语法与类型
来源：http://eyj.chenlongwang.top

================================================================================
来源：http://lta.dianchejie.cn

[A01] Hello World
来源：http://tby.xuetiantiany.cn

Py:   print("Hello, World!")
来源：http://cqy.guannengcc.top

PHP:  echo "Hello, World!";
来源：http://qph.shzxlz.cn

JS:   console.log("Hello, World!");
来源：http://qmh.shuidangran.top

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://wkx.nwbrower.top

Java: System.out.println("Hello, World!");
来源：http://jke.zhengqikj.top

Go:   fmt.Println("Hello, World!")
来源：http://slc.yj202588.top

Ruby: puts "Hello, World!"
来源：http://kwe.jinqigfzy.top

C#:   Console.WriteLine("Hello, World!");
来源：http://lsg.hesvh.cn

[A02] 变量声明与赋值
来源：http://jyf.andypj.xyz

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://shq.hnxiangtu.top

PHP:  $name = "Alex"; $age = 20;
来源：http://yph.sufxvd.cn

JS:   let name = "Alex"; const age = 20;
来源：http://ygd.chenzaomai.com

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://gzf.cqqwz.cn

Java: String name = "Alex"; int age = 20;
来源：http://qej.redwolf501.top

Go:   name := "Alex"; age := 20
来源：http://ots.hammf.cn

Ruby: name = "Alex"; age = 20
来源：http://gkh.hysaishi.cn

C#:   string name = "Alex"; int age = 20;
来源：http://ghn.meibo888.top

[A03] 常量定义
来源：http://jvn.jlsjyb.cn

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://bob.xinyue.icu

PHP:  const PI = 3.14159;
来源：http://jrk.jinyuanbaomall.cn

JS:   const PI = 3.14159;
来源：http://aqv.cucudq.cn

TS:   const PI: number = 3.14159;
来源：http://qfq.ppjwa.cn

Java: static final double PI = 3.14159;
来源：http://ewv.ctjpmb.com

Go:   const PI = 3.14159
来源：http://abt.xinyue.icu

Ruby: PI = 3.14159
来源：http://jik.fanxiaobao.xyz

C#:   const double PI = 3.14159;
来源：http://cyq.hesvh.cn

[A04] 判断变量类型
来源：http://vph.xinyue.icu

Py:   type(x).__name__; isinstance(x, int)
来源：http://dmw.jqgfzy.top

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://xxj.jqgfzy.top

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://hzf.yonumen.top

TS:   typeof x; x instanceof Date
来源：http://psu.aibaodan.cn

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://oqy.xinyue.icu

Go:   reflect.TypeOf(x).Name()
来源：http://mlv.hnqzz.top

Ruby: x.class; x.is_a?(Integer)
来源：http://hwa.sysykeji.top

C#:   x.GetType().Name; x is int
来源：http://vhx.chenlongwang.top

[A05] 整数除法与取模
来源：http://tnv.zhaomingkeji.xyz

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://pnk.ywan-chungtsiang.top

PHP:  intdiv(7, 2); 7 % 2
来源：http://trv.yanxiufei.cn

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://mai.zycfv.cn

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://gjg.yongpay.top

Java: 7 / 2; 7 % 2
来源：http://dqz.birdmap.top

Go:   7 / 2; 7 % 2
来源：http://ljo.epnwcf.com

Ruby: 7 / 2; 7 % 2
来源：http://kcc.snrcjt.cn

C#:   7 / 2; 7 % 2
来源：http://bnt.yanxiufei.cn

[A06] 字符串转数字
来源：http://eyq.gotoacloud.top

Py:   int("42"); float("3.14")
来源：http://bbc.sufxvd.cn

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://kag.0kj1m.cn

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://jvz.zhixingplan.top

TS:   parseInt("42", 10); Number("42")
来源：http://vay.cqqwz.cn

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://xnh.zhengqikj.top

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://hhj.xylfe.cn

Ruby: "42".to_i; "3.14".to_f
来源：http://tcj.sweek.top

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://rtu.hysaishi.cn

[A07] 数字转字符串
来源：http://lrl.havefunace.top

Py:   str(42)
来源：http://nar.kuanghao11.cn

PHP:  (string) 42; strval(42)
来源：http://swb.yj20258.top

JS:   String(42); (42).toString()
来源：http://pow.xylfe.cn

TS:   String(42)
来源：http://tuo.daria6918.cn

Java: String.valueOf(42); Integer.toString(42)
来源：http://vcp.svipenyu.cn

Go:   strconv.Itoa(42)
来源：http://hdd.jqgufenzy.top

Ruby: 42.to_s
来源：http://iep.tianlin.xyz

C#:   42.ToString()
来源：http://vzr.ivvv.top

[A08] 取整与四舍五入
来源：http://egj.havefunace.top

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://vad.ydzc1.top

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://wyl.yongpay.top

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://iru.feifeiyinyue.top

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://gjk.nanxuanxn.top

Java: Math.round(3.567); Math.floor(3.9)
来源：http://ufy.sweek.top

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://tta.yj202588.top

Ruby: 3.567.round(2); 3.9.floor
来源：http://pyz.zhongyouzk.top

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://krv.wangshuangyany.cn

[A09] 绝对值与最大最小值
来源：http://ymi.guowangkeji.top

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://tdd.aibaodan.cn

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://xuz.ppjwa.cn

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://caw.yfazqb.com

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://eoo.9152youxi.cn

Java: Math.abs(-5); Math.max(1, 2)
来源：http://gbn.zhaomingkeji.xyz

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://wtv.gaohongyu789.top

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://vac.dianchejie.cn

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://pgl.yanxiufei.cn

[A10] 生成随机数
来源：http://slj.yonumen.top

Py:   import random; random.randint(1, 100)
来源：http://jyn.nanxuanxn.top

PHP:  random_int(1, 100);
来源：http://ljt.hysaishi.cn

JS:   Math.floor(Math.random() * 100) + 1
来源：http://fgu.quarkkingdee.top

TS:   Math.floor(Math.random() * 100) + 1
来源：http://apa.iojbl.cn

Java: new Random().nextInt(100) + 1
来源：http://ybu.gzhubu.top

Go:   rand.Intn(100) + 1               // math/rand
来源：http://vbm.tarul.cn

Ruby: rand(1..100)
来源：http://gol.fengsongda.top

C#:   new Random().Next(1, 101)
来源：http://lsn.chenlongwang.top

[A11] 条件表达式（三元）
来源：http://ceu.yuxming.cn

Py:   "yes" if x > 0 else "no"
来源：http://kim.nwbrower.top

PHP:  $x > 0 ? "yes" : "no"
来源：http://lcv.havefunace.top

JS:   x > 0 ? "yes" : "no"
来源：http://qfa.yanxiufei.cn

TS:   x > 0 ? "yes" : "no"
来源：http://fiw.nanxuanxn.top

Java: x > 0 ? "yes" : "no"
来源：http://mul.smart0.xyz

Go:   // 无三元运算符，需用 if 语句
来源：http://qkl.jinqigufen.top

Ruby: x > 0 ? "yes" : "no"
来源：http://niz.cheryme.top

C#:   x > 0 ? "yes" : "no"
来源：http://jih.havefunace.top

[A12] 字符串插值 / 格式化
来源：http://mee.smart0.xyz

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://ovt.xingfuxueyuan.xyz

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://igr.jinqigfzy.top

JS:   `Hello, ${name}!`
来源：http://qju.sysykeji.top

TS:   `Hello, ${name}!`
来源：http://pow.vqdsnc.cn

Java: "Hello, %s!".formatted(name)
来源：http://hkh.hysaishi.cn

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://qaf.aibaodan.cn

Ruby: "Hello, #{name}!"
来源：http://zwj.yuanzhike.top

C#:   $"Hello, {name}!"
来源：http://sdk.hnxiangtu.top

[A13] 多行字符串（练习 \n 转义）
来源：http://hgc.sjlbkw.cn

Py:   "第一行\n第二行"
来源：http://eul.feifeiyinyue.top

PHP:  "第一行\n第二行"
来源：http://yfb.dashuyun.cn

JS:   "第一行\n第二行"
来源：http://ebn.yueranfly.top

TS:   "第一行\n第二行"
来源：http://zdo.cucudq.cn

Java: "第一行\n第二行"
来源：http://qwd.yj20258888.top

Go:   "第一行\n第二行"
来源：http://zpw.9152youxi.cn

Ruby: "第一行\n第二行"
来源：http://lno.yonumen.top

C#:   "第一行\n第二行"
来源：http://qzg.yongpay.top

[A14] 注释写法
来源：http://ibu.ivvv.top

Py:   # 单行；三引号字符串可作多行说明
来源：http://hhd.c1oappe.top

PHP:  // 或 # 单行；/* 多行 */
来源：http://wgq.bjfxy.top

JS:   // 单行；/* 多行 */
来源：http://lob.zycfv.cn

TS:   // 单行；/* 多行 */
来源：http://lzi.sysykeji.top

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://wuq.tianlin.xyz

Go:   // 单行；/* 多行 */
来源：http://vaa.jinyuanbaomall.cn

Ruby: # 单行；=begin 多行 =end
来源：http://ekl.fzhhl.top

C#:   // 单行；/* 多行 */
来源：http://ywm.quarkkingdee.top

[A15] 空值判断与默认值
来源：http://jlg.jinyuanbaomall.cn

Py:   value = data or "默认值"
来源：http://cfg.jinqigufen.top

PHP:  $value = $data ?? "默认值";
来源：http://ysn.zhaomingkeji.xyz

JS:   const value = data ?? "默认值";
来源：http://tkl.haohaochexian.top

TS:   const value = data ?? "默认值";
来源：http://xel.yj20258888.top

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://xtv.yj20258888.top

Go:   if data == "" { data = "默认值" }
来源：http://tay.xinyue.icu

Ruby: value = data || "默认值"
来源：http://hzv.andypj.xyz

C#:   var value = data ?? "默认值";
来源：http://qdx.jiagoushi.top

[A16] 真假值判断规则
来源：http://ygn.hywenlv.cn

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://ylx.zhiwuduotai.top

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://klf.yanxiufei.cn

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://kry.cucudq.cn

TS:   if (!x) {}
来源：http://xqy.jqgfzy.top

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://qwj.52xcode.cn

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://rud.jqgufenzy.top

Ruby: unless x            # nil 与 false 为假
来源：http://zhr.uphjek.com

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://ror.xuanzx.com

[A17] 位运算
来源：http://llp.zhiwuduotai.top

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://gkh.jqgufenzy.top

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://xgt.zhiwuduotai.top

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://fje.sxryk.cn

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://kdw.jiagoushi.top

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://lzh.fktsv.cn

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://usp.gaohongyu789.top

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://ehg.tarul.cn

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://oew.fanxiaobao.xyz

[A18] 字符与 ASCII 码互转
来源：http://gci.fktsv.cn

Py:   ord("A"); chr(65)
来源：http://mph.hnqzz.top

PHP:  ord("A"); chr(65)
来源：http://kak.tarul.cn

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://vwo.jinghuilouyu.cn

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://pcm.zhoulong.xyz

Java: (int) 'A'; (char) 65
来源：http://mxn.hnxiangtu.top

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://ppj.hnxiangtu.top

Ruby: "A".ord; 65.chr
来源：http://hit.dashuyun.cn

C#:   (int)'A'; (char)65
来源：http://yts.dashuyun.cn

[A19] 交换两个变量
来源：http://ylq.jqgfzy.top

Py:   a, b = b, a
来源：http://qlb.yueranfly.top

PHP:  [$a, $b] = [$b, $a];
来源：http://wbn.yuxming.cn

JS:   [a, b] = [b, a];
来源：http://yxl.ywan-chungtsiang.top

TS:   [a, b] = [b, a];
来源：http://uop.xinyue.icu

Java: int t = a; a = b; b = t;
来源：http://gkq.tanke756.top

Go:   a, b = b, a
来源：http://kry.shzxlz.cn

Ruby: a, b = b, a
来源：http://gwe.ivvv.top

C#:   (a, b) = (b, a);
来源：http://zgd.sweek.top

[A20] 读取标准输入
来源：http://pkf.chenzaomai.com

Py:   name = input("请输入：")
来源：http://jbk.c1oappe.top

PHP:  $name = trim(fgets(STDIN));
来源：http://hgf.xziqi.cn

JS:   // Node.js：readline 模块或 process.stdin
来源：http://ckj.jqgfzy.top

TS:   // Node.js：readline 模块
来源：http://fcw.yfazqb.com

Java: new Scanner(System.in).nextLine()
来源：http://uua.9152youxi.cn

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://udi.sufxvd.cn

Ruby: gets.chomp
来源：http://tkx.ydzc1.top

C#:   Console.ReadLine();
来源：http://xbo.ivvv.top

[A21] 保留指定小数位输出
来源：http://yjg.yonumen.top

Py:   f"{3.14159:.2f}"
来源：http://xtb.52xcode.cn

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://ptr.bjfxy.top

JS:   (3.14159).toFixed(2)
来源：http://dhi.ybcxt.top

TS:   (3.14159).toFixed(2)
来源：http://yya.jinghuilouyu.cn

Java: String.format("%.2f", 3.14159)
来源：http://xyw.zdbjq.cn

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://vxy.haohaochexian.top

Ruby: format("%.2f", 3.14159)
来源：http://yfh.ivvv.top

C#:   3.14159.ToString("F2")
来源：http://teq.xziqi.cn

[A22] 获取字符串长度
来源：http://gox.cqqwz.cn

Py:   len(s)
来源：http://rru.tian-w.cn

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mdl.cdnleiting.top

JS:   s.length                          # 按 UTF-16 单元计
来源：http://ctp.nanxuanxn.top

TS:   s.length
来源：http://ctx.hammf.cn

Java: s.length()
来源：http://hnu.hywenlv.cn

Go:   len(s); utf8.RuneCountInString(s)
来源：http://ckt.nanxinkj.top

Ruby: s.length
来源：http://ayi.aizwys.cn

C#:   s.Length
来源：http://sky.ctjpmb.com

[A23] 大小写转换
来源：http://tvs.yfazqb.com

Py:   s.upper(); s.lower(); s.title()
来源：http://wad.yvedp.cn

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://ptw.sufxvd.cn

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://rlc.yueranfly.top

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://puw.xinyue.icu

Java: s.toUpperCase(); s.toLowerCase()
来源：http://lmt.fanxiaobao.xyz

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://pql.yangfankeji.com

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://vfy.ybcxt.top

C#:   s.ToUpper(); s.ToLower()
来源：http://kgt.chenjidiqi.icu

[A24] 去除首尾空白
来源：http://zzq.zdqjudy.top

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://dep.ctjpmb.com

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://jyk.epnwcf.com

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://pea.shuidangran.top

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://ujz.yj20258.top

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://gbc.mhx1999.top

Go:   strings.TrimSpace(s)
来源：http://msa.pengpengdd.cyou

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://qzk.yj202588.top

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://oml.svipenyu.cn

[A25] 字符串比较
来源：http://dpw.zycfv.cn

Py:   s1 == s2; s1 != s2
来源：http://vxi.sysykeji.top

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://tca.wangdashe.top

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://izp.c1oappe.top

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://rtk.zhoulong.xyz

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://kjg.52xcode.cn

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://lms.sweek.top

Ruby: s1 == s2; s1 <=> s2
来源：http://ybv.zdbjq.cn

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://rle.jinghuilouyu.cn

[A26] 类型转换总览
来源：http://pjx.zhaomingkeji.xyz

Py:   int() float() str() bool() list() dict() tuple()
来源：http://qrn.fzhhl.top

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://rgg.hesvh.cn

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://gsj.daxiang520.top

TS:   Number() String() Boolean() x as number
来源：http://czc.andypj.xyz

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://igb.jyoumei.cn

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://bzb.jlsjyb.cn

Ruby: to_i to_f to_s to_sym to_a
来源：http://cqj.jinqigufen.top

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://ecc.bjfxy.top

================================================================================
来源：http://aow.yj20258.top

B. 流程控制
来源：http://loz.hammf.cn

================================================================================
来源：http://nzn.cashguo.top

[B01] 条件判断 if / else
来源：http://kll.daria6918.cn

Py:   result = "正" if x > 0 else "非正"
来源：http://hna.smart0.xyz

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://het.jianghu66.top

JS:   const r = x > 0 ? "正" : "非正";
来源：http://yvm.jqgfzy.top

TS:   const r = x > 0 ? "正" : "非正";
来源：http://joz.shanyushiyangkeji.top

Java: String r = x > 0 ? "正" : "非正";
来源：http://ssa.fzhhl.top

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://huv.aizwys.cn

Ruby: r = x > 0 ? "正" : "非正"
来源：http://bno.wangdashe.top

C#:   var r = x > 0 ? "正" : "非正";
来源：http://jjt.ydjk.org.cn

[B02] 多分支 else if / elif
来源：http://lww.yongpay.top

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://shi.feifeiyinyue.top

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://ddb.chenzaomai.com

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hja.zhaomingkeji.xyz

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://neo.hywenlv.cn

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://xtk.gaohongyu789.top

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://fqq.gaohongyu789.top

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mqq.yj202588.top

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://lpb.yueranfly.top

[B03] switch / match / case
来源：http://hff.meibo888.top

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://txo.ctjpmb.com

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://irh.sxryk.cn

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://aps.xinyue.icu

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://gzm.nanxinkj.top

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://doj.yvedp.cn

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://ier.sjlbkw.cn

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://elf.52xcode.cn

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://arn.tanke756.top

[B04] for 计数循环
来源：http://qlv.epnwcf.com

Py:   for i in range(10): print(i)
来源：http://emi.dianchejie.cn

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://twz.tianlin.xyz

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://tgc.hnqzz.top

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://eqc.bjfxy.top

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://vls.dianchejie.cn

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://rws.zhaomingkeji.xyz

Ruby: 10.times { |i| puts i }
来源：http://sjj.sjlbkw.cn

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://fnt.bjfxy.top

[B05] 遍历数组 / 列表
来源：http://lbb.gaohongyu789.top

Py:   for item in arr: print(item)
来源：http://ddq.jinqigfzy.top

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://xjz.shzxlz.cn

JS:   for (const item of arr) { console.log(item); }
来源：http://wpp.sufxvd.cn

TS:   for (const item of arr) { console.log(item); }
来源：http://est.hongshengwenyu.top

Java: for (var item : arr) { System.out.println(item); }
来源：http://vbu.0kj1m.cn

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://xvj.hesvh.cn

Ruby: arr.each { |item| puts item }
来源：http://qnd.hammf.cn

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://xdc.yangfankeji.com

[B06] 遍历字典 / 对象
来源：http://bbx.feifeiyinyue.top

Py:   for k, v in d.items(): print(k, v)
来源：http://ctu.52xcode.cn

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://syf.xingfuxueyuan.xyz

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://rln.gaohongyu789.top

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://vyc.vqdsnc.cn

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://bew.zhoulong.xyz

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://vkj.ybcxt.top

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wpf.zdqjudy.top

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://unn.ehwqpu.com

[B07] while 循环
来源：http://fjt.hfpthk.cn

Py:   while i < 10: i += 1
来源：http://lbh.chenzaomai.com

PHP:  while ($i < 10) { $i++; }
来源：http://onn.fehbvm.com

JS:   while (i < 10) { i++; }
来源：http://hri.zhoulong.xyz

TS:   while (i < 10) { i++; }
来源：http://zav.nanxuanxn.top

Java: while (i < 10) { i++; }
来源：http://xca.yuxming.cn


<!-- 参考信息 -->