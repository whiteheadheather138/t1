代发 wailian999

JS:   this.name = "x";
来源：http://nie.snrcjt.cn

TS:   name: string = "x";
来源：http://qtc.jianghu66.top

Java: private String name;
来源：http://ytw.gaohongyu789.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ndq.ctjpmb.com

Ruby: @name = "x"
来源：http://bkh.yvedp.cn

C#:   public string Name { get; set; } = "x";
来源：http://rul.ydzc1.top

[G04] 定义方法
来源：http://oqt.nanxuanxn.top

Py:   def greet(self): return self.name
来源：http://bax.pycfn.com

PHP:  public function greet(): string { return $this->name; }
来源：http://vxa.yongpay.top

JS:   greet() { return this.name; }
来源：http://nmn.dashuyun.cn

TS:   greet(): string { return this.name; }
来源：http://ycc.yuanzhike.top

Java: String greet() { return name; }
来源：http://bhv.aizwys.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gxc.zhoulong.xyz

Ruby: def greet; @name; end
来源：http://byg.hnqzz.top

C#:   public string Greet() => Name;
来源：http://bow.shuidangran.top

[G05] 继承
来源：http://prh.jinghuilouyu.cn

Py:   class Admin(User): pass
来源：http://jqj.yueranfly.top

PHP:  class Admin extends User {}
来源：http://bkm.ybcxt.top

JS:   class Admin extends User {}
来源：http://jfw.cheryme.top

TS:   class Admin extends User {}
来源：http://uif.zhoulong.xyz

Java: class Admin extends User {}
来源：http://xam.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kcd.fktsv.cn

Ruby: class Admin < User; end
来源：http://wfw.xinyue.icu

C#:   class Admin : User {}
来源：http://yij.bbcook.cn

[G06] 重写方法
来源：http://klf.xinyue.icu

Py:   def greet(self): return "admin"
来源：http://wcc.nanxuanxn.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kkp.yj202588.top

JS:   greet() { return "admin"; }
来源：http://loc.zhixingplan.top

TS:   greet(): string { return "admin"; }
来源：http://lxy.gaohongyu789.top

Java: @Override String greet() { return "admin"; }
来源：http://qpm.nwbrower.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lsa.tianlin.xyz

Ruby: def greet; "admin"; end
来源：http://mzy.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://yyg.xuetiantiany.cn

[G07] 调用父类方法
来源：http://gwa.shzxlz.cn

Py:   super().greet()
来源：http://kzs.zhaomingkeji.xyz

PHP:  parent::greet();
来源：http://dkm.shangyingyoupin.top

JS:   super.greet();
来源：http://qpt.jinyuanbaomall.cn

TS:   super.greet();
来源：http://yxo.jqgufenzy.top

Java: super.greet();
来源：http://ujd.jinghuilouyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qyj.ivvv.top

Ruby: super
来源：http://dht.yuxming.cn

C#:   base.Greet();
来源：http://xet.dashuyun.cn

[G08] 静态方法与属性
来源：http://yts.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aus.hnxiangtu.top

PHP:  public static function f() {}
来源：http://leo.mhx1999.top

JS:   static f() {}
来源：http://eos.iojbl.cn

TS:   static f(): void {}
来源：http://zix.cashguo.top

Java: static void f() {}
来源：http://mjm.svipenyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kez.sxryk.cn

Ruby: def self.f; end
来源：http://whq.sweek.top

C#:   public static void F() {}
来源：http://opr.yuanzhike.top

[G09] 接口 / 抽象类
来源：http://olo.yueranfly.top

Py:   from abc import ABC, abstractmethod
来源：http://rsk.jinqigfzy.top

PHP:  interface Shape { public function area(): float; }
来源：http://iko.0kj1m.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://owt.gotoacloud.top

TS:   interface Shape { area(): number; }
来源：http://ihx.vehdjk.com

Java: interface Shape { double area(); }
来源：http://ukb.ydjk.org.cn

Go:   type Shape interface { Area() float64 }
来源：http://msr.wangshuangyany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ggs.zhoulong.xyz

C#:   interface IShape { double Area(); }
来源：http://uch.xuanzx.com

[G10] 访问控制
来源：http://wuj.ydjk.org.cn

Py:   约定 _protected / __private（不强制）
来源：http://pld.cheryme.top

PHP:  public / protected / private
来源：http://vna.jyoumei.cn

JS:   #private 字段；其余公开
来源：http://tnd.ppjwa.cn

TS:   public / protected / private
来源：http://pix.svipenyu.cn

Java: public / protected / private / 默认包级
来源：http://hda.yvedp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hvg.yuxming.cn

Ruby: public / protected / private
来源：http://aiv.zhiwuduotai.top

C#:   public / protected / private / internal
来源：http://arr.yj20258.top

[G11] getter / setter
来源：http://xmf.xuetiantiany.cn

Py:   @property 与 @x.setter
来源：http://upa.kuanghao11.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tzt.zdbjq.cn

JS:   get name() { return this._name; }
来源：http://vuo.cheryme.top

TS:   get name(): string { return this._name; }
来源：http://jyj.daria6918.cn

Java: public String getName() { return name; }
来源：http://fci.ydjk.org.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bjs.jiagoushi.top

Ruby: attr_accessor :name
来源：http://axs.sweek.top

C#:   public string Name { get; set; }
来源：http://qpb.yonumen.top

[G12] 对象转字符串
来源：http://iqg.cdnleiting.top

Py:   def __str__(self): return self.name
来源：http://mpp.tianlin.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://wur.yj20258.top

JS:   toString() { return this.name; }
来源：http://eni.jinyuanbaomall.cn

TS:   toString(): string { return this.name; }
来源：http://wza.yj20258888.top

Java: @Override public String toString() { return name; }
来源：http://zhw.yj20258.top

Go:   func (u User) String() string { return u.Name }
来源：http://fbz.sxryk.cn

Ruby: def to_s; @name; end
来源：http://cct.fktsv.cn

C#:   public override string ToString() => Name;
来源：http://xbg.nwbrower.top

[G13] 判断对象类型
来源：http://wtg.wangshuangyany.cn

Py:   isinstance(u, User)
来源：http://osi.pycfn.com

PHP:  $u instanceof User
来源：http://ztp.shanyushiyangkeji.top

JS:   u instanceof User
来源：http://tze.c1oappe.top

TS:   u instanceof User
来源：http://sfw.cucudq.cn

Java: u instanceof User
来源：http://dxi.xylfe.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kcy.sysykeji.top

Ruby: u.is_a?(User)
来源：http://yus.ydzc1.top

C#:   u is User
来源：http://wtl.vqdsnc.cn

[G14] 数据类 / record
来源：http://mzx.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kds.jqgfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://ire.ydjk.org.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bva.sysykeji.top

TS:   type User = { name: string; age: number };
来源：http://lrk.xuetiantiany.cn

Java: record User(String name, int age) {}
来源：http://bvn.hnqzz.top

Go:   type User struct { Name string; Age int }
来源：http://ibd.chenzaomai.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cyk.aizwys.cn

C#:   record User(string Name, int Age);
来源：http://ywv.xylfe.cn

[G15] 枚举
来源：http://zyc.hcnkem.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rcz.fzhhl.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ldw.birdmap.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mvp.jlsjyb.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://saa.kuanghao11.cn

Java: enum Color { RED, GREEN }
来源：http://mza.shanyushiyangtech.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rjq.ctjpmb.com

Ruby: Color = %i[red green].freeze
来源：http://cwh.redwolf501.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://upz.jyoumei.cn

[G16] 对象转数组 / 字典
来源：http://bgd.yvedp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qja.jlsjyb.cn

PHP:  get_object_vars($obj);
来源：http://pyd.shuidangran.top

JS:   Object.entries(obj)
来源：http://xte.fzhhl.top

TS:   Object.entries(obj)
来源：http://hya.yfazqb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xvx.vqdsnc.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jjv.sjlbkw.cn

Ruby: obj.instance_variables
来源：http://jci.gzhubu.top

C#:   // 用反射或 System.Text.Json
来源：http://sls.quarkkingdee.top

================================================================================
来源：http://rdk.jinqigufen.top

H. 异常与错误处理
来源：http://yps.ctjpmb.com

================================================================================
来源：http://cph.hfpthk.cn

[H01] try / catch 基础
来源：http://rbi.yanxiufei.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cbp.tian-w.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wwq.jlsjyb.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ajn.xuanzx.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mzv.daria6918.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oea.pengpengdd.cyou

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xuj.daxiang520.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jmt.yj20258.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vym.jqgfzy.top

[H02] finally / ensure 收尾
来源：http://azn.gzhubu.top

Py:   try: f()⏎finally: cleanup()
来源：http://dma.hongshengwenyu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://hak.havefunace.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qwd.gaohongyu789.top

TS:   try { f(); } finally { cleanup(); }
来源：http://nyv.vqdsnc.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fwi.smart0.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://jdd.nwbrower.top

Ruby: begin; f; ensure; cleanup; end
来源：http://xeq.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mvk.sxryk.cn

[H03] 主动抛出异常
来源：http://qxk.yangfankeji.com

Py:   raise ValueError("错误信息")
来源：http://dnf.svipenyu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wum.ywan-chungtsiang.top

JS:   throw new Error("错误信息");
来源：http://kkn.sweek.top

TS:   throw new Error("错误信息");
来源：http://yqh.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://slg.vehdjk.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jkf.tarul.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://arg.xuetiantiany.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rwo.gogol.net.cn

[H04] 自定义异常类型
来源：http://pnv.yangfankeji.com

Py:   class MyError(Exception): pass
来源：http://bbq.epnwcf.com

PHP:  class MyError extends RuntimeException {}
来源：http://ops.xinyue.icu

JS:   class MyError extends Error {}
来源：http://wii.hesvh.cn

TS:   class MyError extends Error {}
来源：http://gsh.birdmap.top

Java: class MyException extends RuntimeException {}
来源：http://vwr.sysykeji.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ctq.nwbrower.top

Ruby: class MyError < StandardError; end
来源：http://lkt.jqgfzy.top

C#:   class MyException : Exception {}
来源：http://rjr.fzhhl.top

[H05] 捕获特定类型
来源：http://wuk.sufxvd.cn

Py:   except ValueError as e:
来源：http://zqa.yj202588.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zga.sxryk.cn

JS:   if (e instanceof TypeError) {}
来源：http://jwq.hfpthk.cn

TS:   if (e instanceof TypeError) {}
来源：http://wfi.shangyingyoupin.top

Java: catch (IOException | SQLException e) {}
来源：http://fym.fengsongda.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fqq.daxiang520.top

Ruby: rescue ArgumentError => e
来源：http://qne.zdqjudy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hks.yueranfly.top

[H06] 可选值 / 空值安全访问
来源：http://clh.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://tux.shuidangran.top

PHP:  $v = $d["k"] ?? null;
来源：http://wzx.zycfv.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uzn.sweek.top

TS:   obj?.a?.b;  d ?? default
来源：http://kni.mhx1999.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xew.yj20258.top

Go:   if v, ok := m["k"]; ok { }
来源：http://uhe.svipenyu.cn

Ruby: d&.dig(:a, :b)
来源：http://aqw.feifeiyinyue.top

C#:   obj?.A?.B ?? default
来源：http://qqw.ybcxt.top

[H07] 断言
来源：http://evx.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://zio.guannengcc.top

PHP:  assert($x > 0);
来源：http://bla.snrcjt.cn

JS:   console.assert(x > 0);
来源：http://nql.yonumen.top

TS:   console.assert(x > 0);
来源：http://luw.yangfankeji.com

Java: assert x > 0 : "必须为正";
来源：http://fuu.xuetiantiany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://swd.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://dzh.guowangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://gxx.daxiang520.top

[H08] 获取错误信息与堆栈
来源：http://ldn.xuetiantiany.cn

Py:   str(e);  traceback.format_exc()
来源：http://hkl.guowangkeji.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yzd.havefunace.top

JS:   e.message;  e.stack
来源：http://hxc.chenjidiqi.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://fig.nanxuanxn.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ilp.ppjwa.cn

Go:   err.Error()
来源：http://pln.wangdashe.top

Ruby: e.message;  e.backtrace
来源：http://wmn.mhx1999.top

C#:   e.Message;  e.StackTrace
来源：http://vda.tanke756.top

[H09] 带错误码的异常
来源：http://inp.xuanzx.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://evq.zdbjq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nbn.gaohongyu789.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mba.ppjwa.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zwj.ehwqpu.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zlj.xziqi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iqt.yj202588.top

Ruby: raise MyError.new("fail", 500)
来源：http://wao.dashuyun.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jzo.cqqwz.cn

[H10] 资源自动释放
来源：http://phe.fktsv.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://srz.daria6918.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tvr.nanxuanxn.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zvd.guannengcc.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://egx.hnxiangtu.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kmq.pengpengdd.cyou

Go:   defer f.Close()
来源：http://gam.hysaishi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tdk.0kj1m.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bxn.pycfn.com

================================================================================
来源：http://bcd.haohaochexian.top

I. 正则表达式
来源：http://bsw.dianchejie.cn

================================================================================
来源：http://ldy.yangfankeji.com

[I01] 判断是否匹配
来源：http://zej.shzxlz.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vwg.yj20258888.top

PHP:  preg_match('/\d+/', $s);
来源：http://ucv.0kj1m.cn

JS:   /\d+/.test(s)
来源：http://kqd.zhengqikj.top

TS:   /\d+/.test(s)
来源：http://trs.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ddb.0kj1m.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uaq.sweek.top

Ruby: s.match?(/\d+/)
来源：http://ibe.fktsv.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eik.uphjek.com

[I02] 提取所有匹配
来源：http://mtq.fehbvm.com

Py:   re.findall(r"\d+", s)
来源：http://zgl.jqgufenzy.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://osx.jqgufenzy.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jhc.ehwqpu.com

TS:   s.match(/\d+/g)
来源：http://ehh.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gyp.jlsjyb.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jmy.dashuyun.cn

Ruby: s.scan(/\d+/)
来源：http://lwn.yueranfly.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wur.zhixingplan.top

[I03] 提取捕获分组
来源：http://qrp.ydjk.org.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dag.gotoacloud.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ayz.jinqigfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://btx.hongshengwenyu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://arf.shanyushiyangkeji.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zay.ydjk.org.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dqg.ydjk.org.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lqz.fengsongda.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://olz.jinyuanbaomall.cn

[I04] 正则替换
来源：http://wza.jinqigufen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://aqc.cheryme.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gjk.chenlongwang.top

JS:   s.replace(/\d+/g, "#")
来源：http://crn.uphjek.com

TS:   s.replace(/\d+/g, "#")
来源：http://trv.jqgfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://ohm.hesvh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fxj.jinqigfzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zru.316326.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ieb.316326.xyz

[I05] 按正则拆分
来源：http://qvj.yj202588.top

Py:   re.split(r"\s*,\s*", s)
来源：http://rjg.tianlin.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xez.zhixingplan.top

JS:   s.split(/\s*,\s*/)
来源：http://dyn.jlsjyb.cn

TS:   s.split(/\s*,\s*/)
来源：http://spx.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://wiq.haohaochexian.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pvo.0kj1m.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qhk.fzhhl.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://izj.nanxinkj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rwf.jqgfzy.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ngc.bbcook.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kyv.ydjk.org.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sll.bbcook.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ydb.svipenyu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rqc.shuidangran.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qub.ywan-chungtsiang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hvs.yuanzhike.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qqg.fengsongda.top

[I07] 忽略大小写与多行模式
来源：http://jix.hongshengwenyu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ihk.ppjwa.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://igm.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lwb.yanxiufei.cn

TS:   /error/gim
来源：http://inl.guowangkeji.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://phq.hnxiangtu.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ddk.snrcjt.cn

Ruby: s.scan(/error/i)
来源：http://rbn.jyoumei.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gve.52xcode.cn

[I08] 贪婪与非贪婪匹配
来源：http://tlo.sufxvd.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hlq.hysaishi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oys.mhx1999.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mmq.vqdsnc.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://axm.pengpengdd.cyou

Java: Pattern.compile("<b>.*?</b>")
来源：http://txm.mhx1999.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ymx.fzhhl.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://boc.316326.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ryj.pengpengdd.cyou

================================================================================
来源：http://upo.hysaishi.cn

J. 日期与时间
来源：http://lez.jqgufenzy.top

================================================================================
来源：http://jch.dashuyun.cn

[J01] 获取当前时间
来源：http://kwe.hysaishi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mcc.zdbjq.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nmn.ydzc1.top

JS:   new Date();  Date.now()
来源：http://fjx.shuidangran.top

TS:   new Date();  Date.now()
来源：http://dyh.yvedp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://adg.gotoacloud.top


<!-- 参考信息 -->