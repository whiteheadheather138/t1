代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://pra.ppjwa.cn

[G03] 实例属性
来源：http://vnm.cdnleiting.top

Py:   self.name = "x"
来源：http://brp.pycfn.com

PHP:  public string $name = "x";
来源：http://zvs.guowangkeji.top

JS:   this.name = "x";
来源：http://gub.shzxlz.cn

TS:   name: string = "x";
来源：http://dwn.uphjek.com

Java: private String name;
来源：http://iad.jinqigfzy.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kem.daxiang520.top

Ruby: @name = "x"
来源：http://ufj.yuxming.cn

C#:   public string Name { get; set; } = "x";
来源：http://myr.jlsjyb.cn

[G04] 定义方法
来源：http://qdg.tian-w.cn

Py:   def greet(self): return self.name
来源：http://ytz.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://jnx.xuanzx.com

JS:   greet() { return this.name; }
来源：http://hhz.shanyushiyangkeji.top

TS:   greet(): string { return this.name; }
来源：http://oow.ybcxt.top

Java: String greet() { return name; }
来源：http://xul.meibo888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://gch.316326.xyz

Ruby: def greet; @name; end
来源：http://zhq.zdbjq.cn

C#:   public string Greet() => Name;
来源：http://mja.yj20258.top

[G05] 继承
来源：http://jyg.guannengcc.top

Py:   class Admin(User): pass
来源：http://qfp.jyoumei.cn

PHP:  class Admin extends User {}
来源：http://dtk.hcnkem.com

JS:   class Admin extends User {}
来源：http://sfg.hysaishi.cn

TS:   class Admin extends User {}
来源：http://xlk.yonumen.top

Java: class Admin extends User {}
来源：http://upq.hywenlv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://leq.hnxiangtu.top

Ruby: class Admin < User; end
来源：http://tqd.yj20258.top

C#:   class Admin : User {}
来源：http://vow.iojbl.cn

[G06] 重写方法
来源：http://mqd.chenlongwang.top

Py:   def greet(self): return "admin"
来源：http://icp.daxiang520.top

PHP:  public function greet(): string { return "admin"; }
来源：http://sfk.epnwcf.com

JS:   greet() { return "admin"; }
来源：http://rca.zhiwuduotai.top

TS:   greet(): string { return "admin"; }
来源：http://uqw.fehbvm.com

Java: @Override String greet() { return "admin"; }
来源：http://dnh.andypj.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bwi.iojbl.cn

Ruby: def greet; "admin"; end
来源：http://wtt.guowangkeji.top

C#:   public override string Greet() => "admin";
来源：http://lzk.wangdashe.top

[G07] 调用父类方法
来源：http://jik.zhiwuduotai.top

Py:   super().greet()
来源：http://poq.epnwcf.com

PHP:  parent::greet();
来源：http://blu.yongpay.top

JS:   super.greet();
来源：http://czp.hongshengwenyu.top

TS:   super.greet();
来源：http://rjx.zhixingplan.top

Java: super.greet();
来源：http://wbo.hammf.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://avv.daria6918.cn

Ruby: super
来源：http://rkv.jqgfzy.top

C#:   base.Greet();
来源：http://vth.yueranfly.top

[G08] 静态方法与属性
来源：http://ogq.jinqigfzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yzo.gogol.net.cn

PHP:  public static function f() {}
来源：http://hix.hammf.cn

JS:   static f() {}
来源：http://nzw.zycfv.cn

TS:   static f(): void {}
来源：http://twd.feifeiyinyue.top

Java: static void f() {}
来源：http://mut.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://ggg.nanxinkj.top

Ruby: def self.f; end
来源：http://sgn.xuanzx.com

C#:   public static void F() {}
来源：http://eiq.meibo888.top

[G09] 接口 / 抽象类
来源：http://pwh.shanyushiyangkeji.top

Py:   from abc import ABC, abstractmethod
来源：http://csn.shuidangran.top

PHP:  interface Shape { public function area(): float; }
来源：http://rlp.daxiang520.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zpt.nwbrower.top

TS:   interface Shape { area(): number; }
来源：http://xup.bbcook.cn

Java: interface Shape { double area(); }
来源：http://foc.guannengcc.top

Go:   type Shape interface { Area() float64 }
来源：http://ffw.fzhhl.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pzn.shangyingyoupin.top

C#:   interface IShape { double Area(); }
来源：http://bhl.hcnkem.com

[G10] 访问控制
来源：http://zpd.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://dhi.jinghuilouyu.cn

PHP:  public / protected / private
来源：http://qby.yongpay.top

JS:   #private 字段；其余公开
来源：http://gbt.gogol.net.cn

TS:   public / protected / private
来源：http://wsm.shanyushiyangtech.top

Java: public / protected / private / 默认包级
来源：http://iqg.52xcode.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://awp.nwbrower.top

Ruby: public / protected / private
来源：http://tum.jinyuanbaomall.cn

C#:   public / protected / private / internal
来源：http://wcy.cashguo.top

[G11] getter / setter
来源：http://mam.sufxvd.cn

Py:   @property 与 @x.setter
来源：http://ceq.sysykeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nwa.zhijiandao.cn

JS:   get name() { return this._name; }
来源：http://pcn.shanyushiyangkeji.top

TS:   get name(): string { return this._name; }
来源：http://kfz.havefunace.top

Java: public String getName() { return name; }
来源：http://pih.andypj.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://vex.fengsongda.top

Ruby: attr_accessor :name
来源：http://xit.hnqzz.top

C#:   public string Name { get; set; }
来源：http://dvq.aibaodan.cn

[G12] 对象转字符串
来源：http://awu.shangyingyoupin.top

Py:   def __str__(self): return self.name
来源：http://ufp.guannengcc.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ukr.chenlongwang.top

JS:   toString() { return this.name; }
来源：http://yik.yuxming.cn

TS:   toString(): string { return this.name; }
来源：http://ozz.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://vmv.xingfuxueyuan.xyz

Go:   func (u User) String() string { return u.Name }
来源：http://bpv.hesvh.cn

Ruby: def to_s; @name; end
来源：http://ous.fehbvm.com

C#:   public override string ToString() => Name;
来源：http://deo.ydzc1.top

[G13] 判断对象类型
来源：http://hux.yj202588.top

Py:   isinstance(u, User)
来源：http://diz.gzhubu.top

PHP:  $u instanceof User
来源：http://eoy.sysykeji.top

JS:   u instanceof User
来源：http://zlo.hongshengwenyu.top

TS:   u instanceof User
来源：http://ktt.sysykeji.top

Java: u instanceof User
来源：http://nnr.shangyingyoupin.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://qiz.fanxiaobao.xyz

Ruby: u.is_a?(User)
来源：http://kbx.meibo888.top

C#:   u is User
来源：http://qpn.shanyushiyangkeji.top

[G14] 数据类 / record
来源：http://ess.fehbvm.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://idj.gaohongyu789.top

PHP:  // 用 readonly 属性模拟
来源：http://pxd.xylfe.cn

JS:   // 无内置：普通类或对象字面量
来源：http://inv.cheryme.top

TS:   type User = { name: string; age: number };
来源：http://ohi.hcnkem.com

Java: record User(String name, int age) {}
来源：http://klz.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://dkx.hysaishi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ant.xuanzx.com

C#:   record User(string Name, int Age);
来源：http://ggq.nanxuanxn.top

[G15] 枚举
来源：http://avy.chenjidiqi.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://njh.yanxiufei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://awf.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kvn.ehwqpu.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rxq.jianghu66.top

Java: enum Color { RED, GREEN }
来源：http://xtv.hnxiangtu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://asd.tian-w.cn

Ruby: Color = %i[red green].freeze
来源：http://yfy.sufxvd.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kqw.xinyue.icu

[G16] 对象转数组 / 字典
来源：http://mcl.jyoumei.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ons.jinghuilouyu.cn

PHP:  get_object_vars($obj);
来源：http://dwg.birdmap.top

JS:   Object.entries(obj)
来源：http://lub.ydzc1.top

TS:   Object.entries(obj)
来源：http://itc.fengsongda.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ael.yongpay.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://zzl.havefunace.top

Ruby: obj.instance_variables
来源：http://bqb.bbcook.cn

C#:   // 用反射或 System.Text.Json
来源：http://cdu.haohaochexian.top

================================================================================
来源：http://cwp.xingfuxueyuan.xyz

H. 异常与错误处理
来源：http://zuw.quarkkingdee.top

================================================================================
来源：http://cqy.yj20258.top

[H01] try / catch 基础
来源：http://udg.jqgufenzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ypa.tianlin.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tsy.aizwys.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xww.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lte.cashguo.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://msu.birdmap.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://msr.cdnleiting.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://man.shzxlz.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jwu.yueranfly.top

[H02] finally / ensure 收尾
来源：http://mfn.cashguo.top

Py:   try: f()⏎finally: cleanup()
来源：http://rqu.sxryk.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gxo.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://kvj.jinyuanbaomall.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://deu.sufxvd.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zrb.nanxuanxn.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://dsn.gogol.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hvi.cqqwz.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vas.52xcode.cn

[H03] 主动抛出异常
来源：http://ghr.pengpengdd.cyou

Py:   raise ValueError("错误信息")
来源：http://zje.zhoulong.xyz

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pod.cashguo.top

JS:   throw new Error("错误信息");
来源：http://tga.meibo888.top

TS:   throw new Error("错误信息");
来源：http://ijd.birdmap.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://rze.gzhubu.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sga.dianchejie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hso.mhx1999.top

C#:   throw new ArgumentException("错误信息");
来源：http://yai.zhixingplan.top

[H04] 自定义异常类型
来源：http://arq.jqgfzy.top

Py:   class MyError(Exception): pass
来源：http://ioo.nanxinkj.top

PHP:  class MyError extends RuntimeException {}
来源：http://ome.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://ftj.gaohongyu789.top

TS:   class MyError extends Error {}
来源：http://rtf.cucudq.cn

Java: class MyException extends RuntimeException {}
来源：http://awz.snrcjt.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://tlu.nwbrower.top

Ruby: class MyError < StandardError; end
来源：http://gis.ehwqpu.com

C#:   class MyException : Exception {}
来源：http://zpg.meibo888.top

[H05] 捕获特定类型
来源：http://nwe.havefunace.top

Py:   except ValueError as e:
来源：http://aru.tianlin.xyz

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fhq.sysykeji.top

JS:   if (e instanceof TypeError) {}
来源：http://yji.yueranfly.top

TS:   if (e instanceof TypeError) {}
来源：http://svp.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://eyj.tanke756.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dmv.gaohongyu789.top

Ruby: rescue ArgumentError => e
来源：http://uut.havefunace.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uor.gogol.net.cn

[H06] 可选值 / 空值安全访问
来源：http://bdr.jinqigfzy.top

Py:   value = d.get("k") or default
来源：http://aun.shangyingyoupin.top

PHP:  $v = $d["k"] ?? null;
来源：http://ujo.snrcjt.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cdg.hywenlv.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tck.hongshengwenyu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jsg.yuanzhike.top

Go:   if v, ok := m["k"]; ok { }
来源：http://iol.hesvh.cn

Ruby: d&.dig(:a, :b)
来源：http://dhi.kuanghao11.cn

C#:   obj?.A?.B ?? default
来源：http://xdq.ctjpmb.com

[H07] 断言
来源：http://jfl.aizwys.cn

Py:   assert x > 0, "必须为正"
来源：http://qdb.ydjk.org.cn

PHP:  assert($x > 0);
来源：http://tgq.hywenlv.cn

JS:   console.assert(x > 0);
来源：http://tdo.zhengqikj.top

TS:   console.assert(x > 0);
来源：http://ehu.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://xsk.shzxlz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zfk.hcnkem.com

Ruby: raise "必须为正" unless x > 0
来源：http://jki.zycfv.cn

C#:   Debug.Assert(x > 0);
来源：http://xwc.yonumen.top

[H08] 获取错误信息与堆栈
来源：http://pnn.jlsjyb.cn

Py:   str(e);  traceback.format_exc()
来源：http://rcc.birdmap.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dgq.redwolf501.top

JS:   e.message;  e.stack
来源：http://baq.quarkkingdee.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lvi.jiagoushi.top

Java: e.getMessage();  e.printStackTrace()
来源：http://rve.yuanzhike.top

Go:   err.Error()
来源：http://emc.epnwcf.com

Ruby: e.message;  e.backtrace
来源：http://ohl.shuidangran.top

C#:   e.Message;  e.StackTrace
来源：http://fbm.yangfankeji.com

[H09] 带错误码的异常
来源：http://qts.dashuyun.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nln.zhijiandao.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qad.zdqjudy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://szx.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vyd.0kj1m.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://odf.zhoulong.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kih.svipenyu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ori.wangdashe.top

C#:   // 自定义异常类中加 Code 属性
来源：http://taq.jyoumei.cn

[H10] 资源自动释放
来源：http://rjf.shangyingyoupin.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://aov.haohaochexian.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gud.hfpthk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nkv.c1oappe.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uam.c1oappe.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qdw.feifeiyinyue.top

Go:   defer f.Close()
来源：http://ghi.kuanghao11.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oty.yonumen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://auu.aibaodan.cn

================================================================================
来源：http://rkq.redwolf501.top

I. 正则表达式
来源：http://nep.pengpengdd.cyou

================================================================================
来源：http://cjl.birdmap.top

[I01] 判断是否匹配
来源：http://uty.daxiang520.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fgf.kuanghao11.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nzx.epnwcf.com

JS:   /\d+/.test(s)
来源：http://jmn.daxiang520.top

TS:   /\d+/.test(s)
来源：http://ftt.jinyuanbaomall.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jon.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rxw.havefunace.top

Ruby: s.match?(/\d+/)
来源：http://wzy.yonumen.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mpw.wangshuangyany.cn

[I02] 提取所有匹配
来源：http://fop.pengpengdd.cyou

Py:   re.findall(r"\d+", s)
来源：http://axz.hfpthk.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://izz.tianlin.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wvo.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://apf.hfpthk.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xmx.birdmap.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mzk.hnxiangtu.top

Ruby: s.scan(/\d+/)
来源：http://kqr.yonumen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mwc.zhiwuduotai.top

[I03] 提取捕获分组
来源：http://fpg.jqgufenzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ndz.fzhhl.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qnp.c1oappe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yem.chenzaomai.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yyw.chenzaomai.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://iqb.jyoumei.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dzd.sxryk.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nei.cdnleiting.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gys.fehbvm.com

[I04] 正则替换
来源：http://zrp.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://xfd.zhiwuduotai.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ewc.52xcode.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zig.wangshuangyany.cn

TS:   s.replace(/\d+/g, "#")
来源：http://aau.ivvv.top

Java: s.replaceAll("\\d+", "#")
来源：http://ewn.vqdsnc.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zes.tian-w.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://joi.vqdsnc.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wzj.sxryk.cn

[I05] 按正则拆分
来源：http://jae.hnxiangtu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://jke.kuanghao11.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mkk.hongshengwenyu.top

JS:   s.split(/\s*,\s*/)
来源：http://csl.xingfuxueyuan.xyz

TS:   s.split(/\s*,\s*/)
来源：http://nzn.hcnkem.com

Java: s.split("\\s*,\\s*")
来源：http://kpp.fzhhl.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jpk.aizwys.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kci.pengpengdd.cyou

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dyn.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sss.ppjwa.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xec.jlsjyb.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nog.hcnkem.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uft.ywan-chungtsiang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nuq.fktsv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jsp.shangyingyoupin.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hqz.birdmap.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oyg.fehbvm.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hgb.hnxiangtu.top

[I07] 忽略大小写与多行模式
来源：http://ygq.wangdashe.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gzh.ctjpmb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://svh.hnqzz.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wqt.sysykeji.top

TS:   /error/gim
来源：http://svv.cdnleiting.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oqd.yj20258888.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gvp.daxiang520.top

Ruby: s.scan(/error/i)
来源：http://zkb.hcnkem.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pst.yanxiufei.cn

[I08] 贪婪与非贪婪匹配
来源：http://qpj.jinghuilouyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://knt.aibaodan.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ewl.shzxlz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yvp.jinqigfzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://afd.zhoulong.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://syn.tian-w.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://haa.fehbvm.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hsg.yongpay.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sej.zhongyouzk.top

================================================================================
来源：http://sbd.ybcxt.top

J. 日期与时间
来源：http://spx.meibo888.top

================================================================================
来源：http://ulu.gzhubu.top

[J01] 获取当前时间
来源：http://pwm.sweek.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://auq.ppjwa.cn


<!-- 参考信息 -->