代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://rdj.jyoumei.cn

Java: @Override String greet() { return "admin"; }
来源：http://rou.havefunace.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iaz.hcnkem.com

Ruby: def greet; "admin"; end
来源：http://kbt.daria6918.cn

C#:   public override string Greet() => "admin";
来源：http://jjb.hongshengwenyu.top

[G07] 调用父类方法
来源：http://eva.jinghuilouyu.cn

Py:   super().greet()
来源：http://duv.yj20258888.top

PHP:  parent::greet();
来源：http://bbm.epnwcf.com

JS:   super.greet();
来源：http://dnh.hysaishi.cn

TS:   super.greet();
来源：http://uhf.andypj.xyz

Java: super.greet();
来源：http://mcr.chenzaomai.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://owh.shuidangran.top

Ruby: super
来源：http://eju.hongshengwenyu.top

C#:   base.Greet();
来源：http://zse.shanyushiyangtech.top

[G08] 静态方法与属性
来源：http://vjw.yj202588.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://apj.zhongyouzk.top

PHP:  public static function f() {}
来源：http://fsn.jqgufenzy.top

JS:   static f() {}
来源：http://qgu.zhijiandao.cn

TS:   static f(): void {}
来源：http://jbh.hammf.cn

Java: static void f() {}
来源：http://sfw.ybcxt.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ute.wangshuangyany.cn

Ruby: def self.f; end
来源：http://htm.xingfuxueyuan.xyz

C#:   public static void F() {}
来源：http://ldh.fengsongda.top

[G09] 接口 / 抽象类
来源：http://ewd.52xcode.cn

Py:   from abc import ABC, abstractmethod
来源：http://yqj.xuanzx.com

PHP:  interface Shape { public function area(): float; }
来源：http://pbf.cqqwz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sbn.vehdjk.com

TS:   interface Shape { area(): number; }
来源：http://uqx.jinghuilouyu.cn

Java: interface Shape { double area(); }
来源：http://xcp.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://veq.yj20258888.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ayo.cdnleiting.top

C#:   interface IShape { double Area(); }
来源：http://tly.vehdjk.com

[G10] 访问控制
来源：http://pjv.ppjwa.cn

Py:   约定 _protected / __private（不强制）
来源：http://wsz.vehdjk.com

PHP:  public / protected / private
来源：http://cnr.xuetiantiany.cn

JS:   #private 字段；其余公开
来源：http://qfq.cashguo.top

TS:   public / protected / private
来源：http://djp.ywan-chungtsiang.top

Java: public / protected / private / 默认包级
来源：http://rpq.yj202588.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://lhf.ydjk.org.cn

Ruby: public / protected / private
来源：http://kpr.svipenyu.cn

C#:   public / protected / private / internal
来源：http://zci.cqqwz.cn

[G11] getter / setter
来源：http://xxn.tian-w.cn

Py:   @property 与 @x.setter
来源：http://yyw.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dmj.ppjwa.cn

JS:   get name() { return this._name; }
来源：http://pjo.xinyue.icu

TS:   get name(): string { return this._name; }
来源：http://egu.fengsongda.top

Java: public String getName() { return name; }
来源：http://xjy.cheryme.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ldq.shanyushiyangtech.top

Ruby: attr_accessor :name
来源：http://myf.birdmap.top

C#:   public string Name { get; set; }
来源：http://hen.hysaishi.cn

[G12] 对象转字符串
来源：http://cai.gaohongyu789.top

Py:   def __str__(self): return self.name
来源：http://koe.guowangkeji.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://nhi.dianchejie.cn

JS:   toString() { return this.name; }
来源：http://mnm.yj20258888.top

TS:   toString(): string { return this.name; }
来源：http://upi.ydzc1.top

Java: @Override public String toString() { return name; }
来源：http://jzr.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://fou.dashuyun.cn

Ruby: def to_s; @name; end
来源：http://uow.andypj.xyz

C#:   public override string ToString() => Name;
来源：http://tag.zdqjudy.top

[G13] 判断对象类型
来源：http://njx.epnwcf.com

Py:   isinstance(u, User)
来源：http://man.daria6918.cn

PHP:  $u instanceof User
来源：http://lia.guannengcc.top

JS:   u instanceof User
来源：http://wbr.jiagoushi.top

TS:   u instanceof User
来源：http://qkb.zhixingplan.top

Java: u instanceof User
来源：http://aqh.bbcook.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sug.hammf.cn

Ruby: u.is_a?(User)
来源：http://plz.daxiang520.top

C#:   u is User
来源：http://ulf.jiagoushi.top

[G14] 数据类 / record
来源：http://jxp.ydzc1.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eyr.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://teg.yj20258.top

JS:   // 无内置：普通类或对象字面量
来源：http://vxt.yj202588.top

TS:   type User = { name: string; age: number };
来源：http://fqz.zhijiandao.cn

Java: record User(String name, int age) {}
来源：http://agf.jinqigufen.top

Go:   type User struct { Name string; Age int }
来源：http://mnk.yvedp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eul.pycfn.com

C#:   record User(string Name, int Age);
来源：http://gqd.zhixingplan.top

[G15] 枚举
来源：http://acy.daxiang520.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ynk.fengsongda.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://awm.ydzc1.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://exm.jinghuilouyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dqr.tianlin.xyz

Java: enum Color { RED, GREEN }
来源：http://wkv.aizwys.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wpa.sysykeji.top

Ruby: Color = %i[red green].freeze
来源：http://cri.xylfe.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nch.jlsjyb.cn

[G16] 对象转数组 / 字典
来源：http://lqp.jqgfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wgn.aizwys.cn

PHP:  get_object_vars($obj);
来源：http://pzd.quarkkingdee.top

JS:   Object.entries(obj)
来源：http://aps.fanxiaobao.xyz

TS:   Object.entries(obj)
来源：http://xgb.chenjidiqi.icu

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://htu.sjlbkw.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hex.fehbvm.com

Ruby: obj.instance_variables
来源：http://hcb.9152youxi.cn

C#:   // 用反射或 System.Text.Json
来源：http://ldr.ivvv.top

================================================================================
来源：http://eyu.dianchejie.cn

H. 异常与错误处理
来源：http://ykc.smart0.xyz

================================================================================
来源：http://xks.cheryme.top

[H01] try / catch 基础
来源：http://umk.tanke756.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hxs.shanyushiyangtech.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xls.chenjidiqi.icu

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xhs.svipenyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://exu.zhixingplan.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fmm.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jdk.shzxlz.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xsp.yvedp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rri.52xcode.cn

[H02] finally / ensure 收尾
来源：http://wkv.fanxiaobao.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://eos.fktsv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fyb.jinqigfzy.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vns.xylfe.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kej.wangshuangyany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kgs.ehwqpu.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://out.pengpengdd.cyou

Ruby: begin; f; ensure; cleanup; end
来源：http://ynn.guowangkeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://gfe.hnqzz.top

[H03] 主动抛出异常
来源：http://mmi.zhoulong.xyz

Py:   raise ValueError("错误信息")
来源：http://xxf.316326.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xqa.xuanzx.com

JS:   throw new Error("错误信息");
来源：http://jqo.yonumen.top

TS:   throw new Error("错误信息");
来源：http://vhi.zhiwuduotai.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fya.fktsv.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://neo.guannengcc.top

Ruby: raise ArgumentError, "错误信息"
来源：http://cwr.sxryk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gtb.pycfn.com

[H04] 自定义异常类型
来源：http://fkn.fengsongda.top

Py:   class MyError(Exception): pass
来源：http://ysp.hywenlv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kjr.jiagoushi.top

JS:   class MyError extends Error {}
来源：http://bfo.guowangkeji.top

TS:   class MyError extends Error {}
来源：http://rkk.feifeiyinyue.top

Java: class MyException extends RuntimeException {}
来源：http://ptk.shuidangran.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rnc.svipenyu.cn

Ruby: class MyError < StandardError; end
来源：http://nma.haohaochexian.top

C#:   class MyException : Exception {}
来源：http://tyx.cucudq.cn

[H05] 捕获特定类型
来源：http://kgx.yanxiufei.cn

Py:   except ValueError as e:
来源：http://tbm.dashuyun.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qqo.havefunace.top

JS:   if (e instanceof TypeError) {}
来源：http://ugg.xingfuxueyuan.xyz

TS:   if (e instanceof TypeError) {}
来源：http://rws.9152youxi.cn

Java: catch (IOException | SQLException e) {}
来源：http://wil.daxiang520.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xpq.daria6918.cn

Ruby: rescue ArgumentError => e
来源：http://nre.zhiwuduotai.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vzg.bjfxy.top

[H06] 可选值 / 空值安全访问
来源：http://jtr.fehbvm.com

Py:   value = d.get("k") or default
来源：http://gml.jyoumei.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zef.nanxuanxn.top

JS:   obj?.a?.b;  d ?? default
来源：http://miw.guannengcc.top

TS:   obj?.a?.b;  d ?? default
来源：http://mvq.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ipn.zhixingplan.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fda.gzhubu.top

Ruby: d&.dig(:a, :b)
来源：http://igw.kuanghao11.cn

C#:   obj?.A?.B ?? default
来源：http://gok.jinghuilouyu.cn

[H07] 断言
来源：http://wqm.bbcook.cn

Py:   assert x > 0, "必须为正"
来源：http://fxj.yanxiufei.cn

PHP:  assert($x > 0);
来源：http://len.sweek.top

JS:   console.assert(x > 0);
来源：http://oae.sysykeji.top

TS:   console.assert(x > 0);
来源：http://qqy.xuetiantiany.cn

Java: assert x > 0 : "必须为正";
来源：http://ujt.shzxlz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kcf.chenlongwang.top

Ruby: raise "必须为正" unless x > 0
来源：http://phr.wangdashe.top

C#:   Debug.Assert(x > 0);
来源：http://wkc.tanke756.top

[H08] 获取错误信息与堆栈
来源：http://icr.zdqjudy.top

Py:   str(e);  traceback.format_exc()
来源：http://nyi.meibo888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://quu.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://fmv.cdnleiting.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://hoy.hesvh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gwv.xziqi.cn

Go:   err.Error()
来源：http://gmt.zhengqikj.top

Ruby: e.message;  e.backtrace
来源：http://cok.c1oappe.top

C#:   e.Message;  e.StackTrace
来源：http://mfh.shuidangran.top

[H09] 带错误码的异常
来源：http://igb.9152youxi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zrw.chenzaomai.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://mhx.hfpthk.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qlm.redwolf501.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sef.gzhubu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://slq.hammf.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lra.xziqi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sgb.jinqigfzy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://boy.chenjidiqi.icu

[H10] 资源自动释放
来源：http://xgq.jinyuanbaomall.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://idu.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ull.sysykeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wfp.jqgfzy.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jqf.redwolf501.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://owl.vehdjk.com

Go:   defer f.Close()
来源：http://vfa.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yps.yj20258888.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zjb.tian-w.cn

================================================================================
来源：http://hoi.shanyushiyangkeji.top

I. 正则表达式
来源：http://wdc.hnxiangtu.top

================================================================================
来源：http://wwx.aibaodan.cn

[I01] 判断是否匹配
来源：http://rxp.yongpay.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yrk.quarkkingdee.top

PHP:  preg_match('/\d+/', $s);
来源：http://mqf.jyoumei.cn

JS:   /\d+/.test(s)
来源：http://tld.zhengqikj.top

TS:   /\d+/.test(s)
来源：http://img.jinqigufen.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qvj.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zfl.gogol.net.cn

Ruby: s.match?(/\d+/)
来源：http://tvn.meibo888.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ewm.hnxiangtu.top

[I02] 提取所有匹配
来源：http://lgz.pengpengdd.cyou

Py:   re.findall(r"\d+", s)
来源：http://jag.jinqigfzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://evf.hcnkem.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nou.epnwcf.com

TS:   s.match(/\d+/g)
来源：http://gya.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qex.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bwn.nwbrower.top

Ruby: s.scan(/\d+/)
来源：http://pmz.chenjidiqi.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bqh.jianghu66.top

[I03] 提取捕获分组
来源：http://mkc.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jsy.zycfv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pjm.shanyushiyangkeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zvw.aizwys.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://llb.ehwqpu.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hxv.mhx1999.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wwo.jinqigfzy.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://top.quarkkingdee.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tvh.pengpengdd.cyou

[I04] 正则替换
来源：http://hcq.kuanghao11.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://upr.guowangkeji.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dgd.ehwqpu.com

JS:   s.replace(/\d+/g, "#")
来源：http://bwv.fengsongda.top

TS:   s.replace(/\d+/g, "#")
来源：http://lty.shangyingyoupin.top

Java: s.replaceAll("\\d+", "#")
来源：http://cuj.yuxming.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bsn.aizwys.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dez.zhixingplan.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fby.jyoumei.cn

[I05] 按正则拆分
来源：http://wzr.zycfv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://khe.52xcode.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rzj.fengsongda.top

JS:   s.split(/\s*,\s*/)
来源：http://mnh.yuxming.cn

TS:   s.split(/\s*,\s*/)
来源：http://zmv.quarkkingdee.top

Java: s.split("\\s*,\\s*")
来源：http://oam.316326.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ing.hysaishi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jpd.pengpengdd.cyou

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qjg.fzhhl.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://owk.jqgufenzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kvs.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ojl.shanyushiyangkeji.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gqo.ehwqpu.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cou.epnwcf.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://iqf.316326.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uis.zhoulong.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yul.ehwqpu.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fjc.fzhhl.top

[I07] 忽略大小写与多行模式
来源：http://wfv.hysaishi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vxu.cheryme.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zfe.snrcjt.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://san.kuanghao11.cn

TS:   /error/gim
来源：http://myb.yuxming.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uok.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hrz.chenzaomai.com

Ruby: s.scan(/error/i)
来源：http://umv.vehdjk.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bhm.fzhhl.top

[I08] 贪婪与非贪婪匹配
来源：http://mhg.hammf.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qxz.wangdashe.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hem.mhx1999.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hbm.jianghu66.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ufc.sxryk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jfk.meibo888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qjk.cashguo.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://awn.yuxming.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hhi.aizwys.cn

================================================================================
来源：http://bnq.shangyingyoupin.top

J. 日期与时间
来源：http://oxj.fktsv.cn

================================================================================
来源：http://nly.smart0.xyz

[J01] 获取当前时间
来源：http://pjh.hnxiangtu.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://had.shanyushiyangtech.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fvy.jianghu66.top

JS:   new Date();  Date.now()
来源：http://qii.cashguo.top

TS:   new Date();  Date.now()
来源：http://wbn.chenzaomai.com

Java: LocalDateTime.now();  Instant.now()
来源：http://ecc.fanxiaobao.xyz

Go:   time.Now()
来源：http://yun.shangyingyoupin.top

Ruby: Time.now
来源：http://jmc.svipenyu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gpy.ivvv.top

[J02] 格式化输出
来源：http://ydn.gogol.net.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ucs.ivvv.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nlh.nwbrower.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://egj.fengsongda.top

TS:   d.toISOString()
来源：http://vui.andypj.xyz

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kdf.svipenyu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dcu.ctjpmb.com

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zvb.gotoacloud.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wgo.hongshengwenyu.top

[J03] 字符串解析为日期
来源：http://obw.nanxinkj.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rcv.ybcxt.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ual.zhiwuduotai.top

JS:   new Date("2024-01-02")
来源：http://eun.zdbjq.cn

TS:   new Date("2024-01-02")
来源：http://vxz.0kj1m.cn

Java: LocalDate.parse("2024-01-02")
来源：http://exv.iojbl.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://moo.redwolf501.top

Ruby: Date.parse("2024-01-02")
来源：http://qit.cucudq.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xqm.shangyingyoupin.top

[J04] 时间戳与日期互转
来源：http://afx.yonumen.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jqw.zhijiandao.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nmj.zycfv.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://aah.fehbvm.com

TS:   Math.floor(Date.now() / 1000)
来源：http://lis.epnwcf.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://grb.fanxiaobao.xyz

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ohy.snrcjt.cn


<!-- 参考信息 -->