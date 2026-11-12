代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://rrh.chenzaomai.com

[G03] 实例属性
来源：http://wkh.ctjpmb.com

Py:   self.name = "x"
来源：http://cda.bbcook.cn

PHP:  public string $name = "x";
来源：http://zdp.fktsv.cn

JS:   this.name = "x";
来源：http://ogg.meibo888.top

TS:   name: string = "x";
来源：http://dfo.yuxming.cn

Java: private String name;
来源：http://cnq.ybcxt.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xga.nanxuanxn.top

Ruby: @name = "x"
来源：http://xwb.xinyue.icu

C#:   public string Name { get; set; } = "x";
来源：http://tkw.zdqjudy.top

[G04] 定义方法
来源：http://bwq.jinghuilouyu.cn

Py:   def greet(self): return self.name
来源：http://aqk.shzxlz.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tgm.vqdsnc.cn

JS:   greet() { return this.name; }
来源：http://snt.ctjpmb.com

TS:   greet(): string { return this.name; }
来源：http://sst.guowangkeji.top

Java: String greet() { return name; }
来源：http://exm.bjfxy.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://pdw.nanxinkj.top

Ruby: def greet; @name; end
来源：http://orp.cheryme.top

C#:   public string Greet() => Name;
来源：http://wkl.vehdjk.com

[G05] 继承
来源：http://whj.vehdjk.com

Py:   class Admin(User): pass
来源：http://pve.snrcjt.cn

PHP:  class Admin extends User {}
来源：http://jpp.sxryk.cn

JS:   class Admin extends User {}
来源：http://ssy.zdqjudy.top

TS:   class Admin extends User {}
来源：http://zqb.chenlongwang.top

Java: class Admin extends User {}
来源：http://rbm.chenjidiqi.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lzs.quarkkingdee.top

Ruby: class Admin < User; end
来源：http://jjs.shuidangran.top

C#:   class Admin : User {}
来源：http://olo.jiagoushi.top

[G06] 重写方法
来源：http://ddr.hcnkem.com

Py:   def greet(self): return "admin"
来源：http://hbc.sweek.top

PHP:  public function greet(): string { return "admin"; }
来源：http://fnm.jinyuanbaomall.cn

JS:   greet() { return "admin"; }
来源：http://mgp.yonumen.top

TS:   greet(): string { return "admin"; }
来源：http://cyn.gzhubu.top

Java: @Override String greet() { return "admin"; }
来源：http://jdc.0kj1m.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://suh.chenlongwang.top

Ruby: def greet; "admin"; end
来源：http://ajw.yj20258.top

C#:   public override string Greet() => "admin";
来源：http://nmz.yj20258.top

[G07] 调用父类方法
来源：http://ujq.nanxuanxn.top

Py:   super().greet()
来源：http://hqc.fehbvm.com

PHP:  parent::greet();
来源：http://eeo.kuanghao11.cn

JS:   super.greet();
来源：http://iuv.iojbl.cn

TS:   super.greet();
来源：http://jdw.hammf.cn

Java: super.greet();
来源：http://ykd.fengsongda.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cer.yvedp.cn

Ruby: super
来源：http://phy.gzhubu.top

C#:   base.Greet();
来源：http://uss.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://blj.cqqwz.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zdf.yongpay.top

PHP:  public static function f() {}
来源：http://ryp.ywan-chungtsiang.top

JS:   static f() {}
来源：http://nee.jinghuilouyu.cn

TS:   static f(): void {}
来源：http://nfi.316326.xyz

Java: static void f() {}
来源：http://hex.sysykeji.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://she.tian-w.cn

Ruby: def self.f; end
来源：http://mee.fzhhl.top

C#:   public static void F() {}
来源：http://ffe.yangfankeji.com

[G09] 接口 / 抽象类
来源：http://mvj.ppjwa.cn

Py:   from abc import ABC, abstractmethod
来源：http://djx.yj20258.top

PHP:  interface Shape { public function area(): float; }
来源：http://pxj.feifeiyinyue.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://jec.zhaomingkeji.xyz

TS:   interface Shape { area(): number; }
来源：http://xwr.smart0.xyz

Java: interface Shape { double area(); }
来源：http://ids.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://zna.fzhhl.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vyi.jinghuilouyu.cn

C#:   interface IShape { double Area(); }
来源：http://cqv.bbcook.cn

[G10] 访问控制
来源：http://psp.fanxiaobao.xyz

Py:   约定 _protected / __private（不强制）
来源：http://hyk.fzhhl.top

PHP:  public / protected / private
来源：http://auq.hfpthk.cn

JS:   #private 字段；其余公开
来源：http://yvz.kuanghao11.cn

TS:   public / protected / private
来源：http://rdj.yvedp.cn

Java: public / protected / private / 默认包级
来源：http://mqi.andypj.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://bzk.yanxiufei.cn

Ruby: public / protected / private
来源：http://syg.jqgfzy.top

C#:   public / protected / private / internal
来源：http://muj.xingfuxueyuan.xyz

[G11] getter / setter
来源：http://ypu.xingfuxueyuan.xyz

Py:   @property 与 @x.setter
来源：http://zkw.yonumen.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cfa.tian-w.cn

JS:   get name() { return this._name; }
来源：http://woa.cucudq.cn

TS:   get name(): string { return this._name; }
来源：http://ohx.jqgufenzy.top

Java: public String getName() { return name; }
来源：http://ewc.tanke756.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ffa.ybcxt.top

Ruby: attr_accessor :name
来源：http://wpm.yvedp.cn

C#:   public string Name { get; set; }
来源：http://sry.zhengqikj.top

[G12] 对象转字符串
来源：http://vxq.haohaochexian.top

Py:   def __str__(self): return self.name
来源：http://itg.zycfv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jdi.zhaomingkeji.xyz

JS:   toString() { return this.name; }
来源：http://ynn.xuanzx.com

TS:   toString(): string { return this.name; }
来源：http://son.wangshuangyany.cn

Java: @Override public String toString() { return name; }
来源：http://pmj.pycfn.com

Go:   func (u User) String() string { return u.Name }
来源：http://wkf.9152youxi.cn

Ruby: def to_s; @name; end
来源：http://hqz.sysykeji.top

C#:   public override string ToString() => Name;
来源：http://upi.hcnkem.com

[G13] 判断对象类型
来源：http://qji.yuanzhike.top

Py:   isinstance(u, User)
来源：http://hqu.fanxiaobao.xyz

PHP:  $u instanceof User
来源：http://alt.cashguo.top

JS:   u instanceof User
来源：http://orq.xuetiantiany.cn

TS:   u instanceof User
来源：http://uhm.cucudq.cn

Java: u instanceof User
来源：http://vcl.haohaochexian.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ybs.hysaishi.cn

Ruby: u.is_a?(User)
来源：http://cue.gogol.net.cn

C#:   u is User
来源：http://hdt.fzhhl.top

[G14] 数据类 / record
来源：http://olc.ybcxt.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bqm.gogol.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://ihy.shanyushiyangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://ohg.yvedp.cn

TS:   type User = { name: string; age: number };
来源：http://vbf.yueranfly.top

Java: record User(String name, int age) {}
来源：http://ran.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://dru.yfazqb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ytl.316326.xyz

C#:   record User(string Name, int Age);
来源：http://rey.haohaochexian.top

[G15] 枚举
来源：http://isu.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aqm.316326.xyz

PHP:  enum Color: string { case Red = "red"; }
来源：http://hkw.9152youxi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://teh.jqgfzy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://snx.zhongyouzk.top

Java: enum Color { RED, GREEN }
来源：http://glc.jinqigfzy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pmm.pengpengdd.cyou

Ruby: Color = %i[red green].freeze
来源：http://flm.zhoulong.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cst.yangfankeji.com

[G16] 对象转数组 / 字典
来源：http://nyy.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dab.hcnkem.com

PHP:  get_object_vars($obj);
来源：http://izr.wangshuangyany.cn

JS:   Object.entries(obj)
来源：http://mtw.hysaishi.cn

TS:   Object.entries(obj)
来源：http://ygu.fktsv.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://izd.sufxvd.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kug.yvedp.cn

Ruby: obj.instance_variables
来源：http://ydm.fanxiaobao.xyz

C#:   // 用反射或 System.Text.Json
来源：http://csk.yanxiufei.cn

================================================================================
来源：http://tnx.316326.xyz

H. 异常与错误处理
来源：http://cmm.aibaodan.cn

================================================================================
来源：http://ygm.hnqzz.top

[H01] try / catch 基础
来源：http://vjx.zycfv.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rle.sweek.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zge.jinqigfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nvz.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vrk.tanke756.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uvy.hesvh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rjn.daria6918.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oos.fzhhl.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hbb.ctjpmb.com

[H02] finally / ensure 收尾
来源：http://lpy.hnxiangtu.top

Py:   try: f()⏎finally: cleanup()
来源：http://spa.cashguo.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://qzz.zhijiandao.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yzy.jqgufenzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://bjx.dashuyun.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vng.ydjk.org.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://iqh.jinghuilouyu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uuj.snrcjt.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cup.quarkkingdee.top

[H03] 主动抛出异常
来源：http://lgw.zhongyouzk.top

Py:   raise ValueError("错误信息")
来源：http://gis.haohaochexian.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lex.bbcook.cn

JS:   throw new Error("错误信息");
来源：http://ocf.feifeiyinyue.top

TS:   throw new Error("错误信息");
来源：http://uig.pengpengdd.cyou

Java: throw new IllegalArgumentException("错误信息");
来源：http://wat.quarkkingdee.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xnc.yuxming.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pol.guannengcc.top

C#:   throw new ArgumentException("错误信息");
来源：http://yef.gaohongyu789.top

[H04] 自定义异常类型
来源：http://pee.tarul.cn

Py:   class MyError(Exception): pass
来源：http://jir.hysaishi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://iqv.snrcjt.cn

JS:   class MyError extends Error {}
来源：http://dcd.ydjk.org.cn

TS:   class MyError extends Error {}
来源：http://wzb.shzxlz.cn

Java: class MyException extends RuntimeException {}
来源：http://sup.svipenyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ooq.fehbvm.com

Ruby: class MyError < StandardError; end
来源：http://lgn.epnwcf.com

C#:   class MyException : Exception {}
来源：http://xut.tarul.cn

[H05] 捕获特定类型
来源：http://scq.hesvh.cn

Py:   except ValueError as e:
来源：http://fxp.gotoacloud.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yjk.bbcook.cn

JS:   if (e instanceof TypeError) {}
来源：http://tau.gzhubu.top

TS:   if (e instanceof TypeError) {}
来源：http://yvm.guannengcc.top

Java: catch (IOException | SQLException e) {}
来源：http://jqn.ppjwa.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xwz.yvedp.cn

Ruby: rescue ArgumentError => e
来源：http://lkb.tianlin.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nsw.yanxiufei.cn

[H06] 可选值 / 空值安全访问
来源：http://qqb.hcnkem.com

Py:   value = d.get("k") or default
来源：http://ili.pycfn.com

PHP:  $v = $d["k"] ?? null;
来源：http://wgv.dianchejie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dsr.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://ujs.ppjwa.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lch.iojbl.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://joa.uphjek.com

Ruby: d&.dig(:a, :b)
来源：http://dlu.yanxiufei.cn

C#:   obj?.A?.B ?? default
来源：http://ehv.svipenyu.cn

[H07] 断言
来源：http://hha.zhengqikj.top

Py:   assert x > 0, "必须为正"
来源：http://bsb.yongpay.top

PHP:  assert($x > 0);
来源：http://kac.yuanzhike.top

JS:   console.assert(x > 0);
来源：http://jou.hesvh.cn

TS:   console.assert(x > 0);
来源：http://weg.gaohongyu789.top

Java: assert x > 0 : "必须为正";
来源：http://fvm.uphjek.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jbs.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://psc.shzxlz.cn

C#:   Debug.Assert(x > 0);
来源：http://zdm.fzhhl.top

[H08] 获取错误信息与堆栈
来源：http://awf.ppjwa.cn

Py:   str(e);  traceback.format_exc()
来源：http://kni.yj202588.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://flv.guannengcc.top

JS:   e.message;  e.stack
来源：http://mfj.xuanzx.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://rgg.yuxming.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nzm.jinqigfzy.top

Go:   err.Error()
来源：http://xns.52xcode.cn

Ruby: e.message;  e.backtrace
来源：http://svv.sjlbkw.cn

C#:   e.Message;  e.StackTrace
来源：http://yus.bjfxy.top

[H09] 带错误码的异常
来源：http://rop.hcnkem.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pyn.chenjidiqi.icu

PHP:  throw new RuntimeException("fail", 500);
来源：http://ijo.fktsv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bxt.jyoumei.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uod.vqdsnc.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mmk.9152youxi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://axx.0kj1m.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gca.0kj1m.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fuf.cdnleiting.top

[H10] 资源自动释放
来源：http://sby.pycfn.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://ujz.zdqjudy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://khu.xylfe.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vzc.yongpay.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gma.gaohongyu789.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mns.316326.xyz

Go:   defer f.Close()
来源：http://gvz.yj20258.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rwt.chenlongwang.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hiv.aibaodan.cn

================================================================================
来源：http://hdc.hywenlv.cn

I. 正则表达式
来源：http://gaa.vqdsnc.cn

================================================================================
来源：http://wcv.ehwqpu.com

[I01] 判断是否匹配
来源：http://dhs.jqgfzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zcr.ctjpmb.com

PHP:  preg_match('/\d+/', $s);
来源：http://jzl.jinqigfzy.top

JS:   /\d+/.test(s)
来源：http://vsw.chenjidiqi.icu

TS:   /\d+/.test(s)
来源：http://swa.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mgi.havefunace.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kty.zhijiandao.cn

Ruby: s.match?(/\d+/)
来源：http://taz.chenlongwang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nvs.wangdashe.top

[I02] 提取所有匹配
来源：http://ali.jinyuanbaomall.cn

Py:   re.findall(r"\d+", s)
来源：http://xpq.fehbvm.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zzf.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ucz.zhijiandao.cn

TS:   s.match(/\d+/g)
来源：http://kfd.tian-w.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gyp.vqdsnc.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uaj.yueranfly.top

Ruby: s.scan(/\d+/)
来源：http://eaq.hysaishi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://frj.fehbvm.com

[I03] 提取捕获分组
来源：http://vau.yuanzhike.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eip.jqgufenzy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yjv.ppjwa.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://quu.ydzc1.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hho.zhaomingkeji.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gwf.fengsongda.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gvj.dianchejie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://azb.aizwys.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kyb.tianlin.xyz

[I04] 正则替换
来源：http://zlx.hesvh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ppz.jiagoushi.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zjc.zhiwuduotai.top

JS:   s.replace(/\d+/g, "#")
来源：http://wik.haohaochexian.top

TS:   s.replace(/\d+/g, "#")
来源：http://oai.nanxinkj.top

Java: s.replaceAll("\\d+", "#")
来源：http://duj.ybcxt.top

Go:   re.ReplaceAllString(s, "#")
来源：http://dlj.cqqwz.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qvl.aibaodan.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fsb.yj20258888.top

[I05] 按正则拆分
来源：http://thm.zycfv.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qfl.tanke756.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ymk.zdqjudy.top

JS:   s.split(/\s*,\s*/)
来源：http://wqg.c1oappe.top

TS:   s.split(/\s*,\s*/)
来源：http://qkk.xziqi.cn

Java: s.split("\\s*,\\s*")
来源：http://tvs.hnxiangtu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dcy.hnxiangtu.top

Ruby: s.split(/\s*,\s*/)
来源：http://uae.hnxiangtu.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pon.hywenlv.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ivo.ywan-chungtsiang.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eog.vehdjk.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lpr.smart0.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sdo.kuanghao11.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ktx.zhiwuduotai.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vnu.xinyue.icu

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ihl.ybcxt.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kvg.yonumen.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cwr.hfpthk.cn

[I07] 忽略大小写与多行模式
来源：http://iky.kuanghao11.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://muz.smart0.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vwq.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zlx.epnwcf.com

TS:   /error/gim
来源：http://weo.ybcxt.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ait.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://smn.sufxvd.cn

Ruby: s.scan(/error/i)
来源：http://cwy.jiagoushi.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nah.yanxiufei.cn

[I08] 贪婪与非贪婪匹配
来源：http://uak.fengsongda.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tcg.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jgb.xingfuxueyuan.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zta.sjlbkw.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cqx.316326.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://ceu.feifeiyinyue.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bto.fzhhl.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kls.gaohongyu789.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://myp.shanyushiyangtech.top

================================================================================
来源：http://nbu.sweek.top

J. 日期与时间
来源：http://jss.gotoacloud.top

================================================================================
来源：http://lad.xylfe.cn

[J01] 获取当前时间
来源：http://gcw.tanke756.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://iso.tian-w.cn


<!-- 参考信息 -->