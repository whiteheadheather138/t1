代发 wailian999

TS:   constructor(public name: string) {}
来源：http://phf.hnqzz.top

Java: User(String name) { this.name = name; }
来源：http://mlg.jianghu66.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yfo.hnxiangtu.top

Ruby: def initialize(name); @name = name; end
来源：http://itr.cheryme.top

C#:   public User(string name) { Name = name; }
来源：http://fes.hnqzz.top

[G03] 实例属性
来源：http://rvf.c1oappe.top

Py:   self.name = "x"
来源：http://zof.xylfe.cn

PHP:  public string $name = "x";
来源：http://xdo.bjfxy.top

JS:   this.name = "x";
来源：http://knb.bbcook.cn

TS:   name: string = "x";
来源：http://zck.yuanzhike.top

Java: private String name;
来源：http://wlr.gotoacloud.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fpz.yanxiufei.cn

Ruby: @name = "x"
来源：http://kid.zhijiandao.cn

C#:   public string Name { get; set; } = "x";
来源：http://piu.redwolf501.top

[G04] 定义方法
来源：http://ile.fehbvm.com

Py:   def greet(self): return self.name
来源：http://whj.fanxiaobao.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://fbm.zycfv.cn

JS:   greet() { return this.name; }
来源：http://kpg.iojbl.cn

TS:   greet(): string { return this.name; }
来源：http://kli.haohaochexian.top

Java: String greet() { return name; }
来源：http://tps.yongpay.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://yxo.0kj1m.cn

Ruby: def greet; @name; end
来源：http://abh.jqgufenzy.top

C#:   public string Greet() => Name;
来源：http://ynf.xuetiantiany.cn

[G05] 继承
来源：http://yiw.yonumen.top

Py:   class Admin(User): pass
来源：http://xhh.yuxming.cn

PHP:  class Admin extends User {}
来源：http://swr.cheryme.top

JS:   class Admin extends User {}
来源：http://yhf.wangshuangyany.cn

TS:   class Admin extends User {}
来源：http://wad.xziqi.cn

Java: class Admin extends User {}
来源：http://jaz.ehwqpu.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yqj.xziqi.cn

Ruby: class Admin < User; end
来源：http://ijs.chenlongwang.top

C#:   class Admin : User {}
来源：http://pdj.zhaomingkeji.xyz

[G06] 重写方法
来源：http://jtv.birdmap.top

Py:   def greet(self): return "admin"
来源：http://mhi.meibo888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://gdb.fanxiaobao.xyz

JS:   greet() { return "admin"; }
来源：http://tin.quarkkingdee.top

TS:   greet(): string { return "admin"; }
来源：http://elh.xinyue.icu

Java: @Override String greet() { return "admin"; }
来源：http://nax.nanxinkj.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ong.daria6918.cn

Ruby: def greet; "admin"; end
来源：http://vpo.cheryme.top

C#:   public override string Greet() => "admin";
来源：http://goi.c1oappe.top

[G07] 调用父类方法
来源：http://qbg.haohaochexian.top

Py:   super().greet()
来源：http://mzv.tianlin.xyz

PHP:  parent::greet();
来源：http://qyv.hesvh.cn

JS:   super.greet();
来源：http://rhg.nwbrower.top

TS:   super.greet();
来源：http://jii.sjlbkw.cn

Java: super.greet();
来源：http://jde.guowangkeji.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xqn.jinqigfzy.top

Ruby: super
来源：http://grc.kuanghao11.cn

C#:   base.Greet();
来源：http://rzg.c1oappe.top

[G08] 静态方法与属性
来源：http://wid.yangfankeji.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ggd.aizwys.cn

PHP:  public static function f() {}
来源：http://wvm.hammf.cn

JS:   static f() {}
来源：http://ged.aibaodan.cn

TS:   static f(): void {}
来源：http://chg.zhijiandao.cn

Java: static void f() {}
来源：http://ekk.shanyushiyangtech.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wis.epnwcf.com

Ruby: def self.f; end
来源：http://fez.jqgfzy.top

C#:   public static void F() {}
来源：http://msm.hnxiangtu.top

[G09] 接口 / 抽象类
来源：http://tic.tian-w.cn

Py:   from abc import ABC, abstractmethod
来源：http://tuu.iojbl.cn

PHP:  interface Shape { public function area(): float; }
来源：http://esx.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://aex.guannengcc.top

TS:   interface Shape { area(): number; }
来源：http://mdf.shuidangran.top

Java: interface Shape { double area(); }
来源：http://ivb.yj202588.top

Go:   type Shape interface { Area() float64 }
来源：http://geq.jqgfzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lcf.shzxlz.cn

C#:   interface IShape { double Area(); }
来源：http://acb.quarkkingdee.top

[G10] 访问控制
来源：http://gbj.zhijiandao.cn

Py:   约定 _protected / __private（不强制）
来源：http://czw.yj20258888.top

PHP:  public / protected / private
来源：http://vns.yj20258.top

JS:   #private 字段；其余公开
来源：http://akh.ydjk.org.cn

TS:   public / protected / private
来源：http://sfc.iojbl.cn

Java: public / protected / private / 默认包级
来源：http://kvi.havefunace.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dlx.chenjidiqi.icu

Ruby: public / protected / private
来源：http://con.shzxlz.cn

C#:   public / protected / private / internal
来源：http://bsx.wangdashe.top

[G11] getter / setter
来源：http://twz.andypj.xyz

Py:   @property 与 @x.setter
来源：http://hst.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lzv.bjfxy.top

JS:   get name() { return this._name; }
来源：http://qbd.tian-w.cn

TS:   get name(): string { return this._name; }
来源：http://awd.zdqjudy.top

Java: public String getName() { return name; }
来源：http://ush.yanxiufei.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://chi.yj202588.top

Ruby: attr_accessor :name
来源：http://gsk.zdbjq.cn

C#:   public string Name { get; set; }
来源：http://czv.fehbvm.com

[G12] 对象转字符串
来源：http://new.yuanzhike.top

Py:   def __str__(self): return self.name
来源：http://jdy.cdnleiting.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xal.daxiang520.top

JS:   toString() { return this.name; }
来源：http://gro.guannengcc.top

TS:   toString(): string { return this.name; }
来源：http://jhg.jinyuanbaomall.cn

Java: @Override public String toString() { return name; }
来源：http://vjp.wangshuangyany.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hvi.tarul.cn

Ruby: def to_s; @name; end
来源：http://piz.tianlin.xyz

C#:   public override string ToString() => Name;
来源：http://kgn.chenlongwang.top

[G13] 判断对象类型
来源：http://ovh.fktsv.cn

Py:   isinstance(u, User)
来源：http://ngi.dianchejie.cn

PHP:  $u instanceof User
来源：http://elw.52xcode.cn

JS:   u instanceof User
来源：http://bua.zhongyouzk.top

TS:   u instanceof User
来源：http://scw.tarul.cn

Java: u instanceof User
来源：http://ert.dianchejie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pdr.zdqjudy.top

Ruby: u.is_a?(User)
来源：http://ttw.chenjidiqi.icu

C#:   u is User
来源：http://zbe.andypj.xyz

[G14] 数据类 / record
来源：http://wua.birdmap.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ben.zdbjq.cn

PHP:  // 用 readonly 属性模拟
来源：http://fqg.yj20258888.top

JS:   // 无内置：普通类或对象字面量
来源：http://cfo.birdmap.top

TS:   type User = { name: string; age: number };
来源：http://iws.yj20258.top

Java: record User(String name, int age) {}
来源：http://sdg.dianchejie.cn

Go:   type User struct { Name string; Age int }
来源：http://rnl.ydzc1.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rkw.sweek.top

C#:   record User(string Name, int Age);
来源：http://frw.yvedp.cn

[G15] 枚举
来源：http://rsm.aizwys.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qeq.daxiang520.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://apl.jlsjyb.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wsj.ywan-chungtsiang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nzy.aizwys.cn

Java: enum Color { RED, GREEN }
来源：http://tbl.bbcook.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ioc.bjfxy.top

Ruby: Color = %i[red green].freeze
来源：http://rhj.yj20258.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fgs.dianchejie.cn

[G16] 对象转数组 / 字典
来源：http://qve.chenlongwang.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gql.shanyushiyangtech.top

PHP:  get_object_vars($obj);
来源：http://oiy.cucudq.cn

JS:   Object.entries(obj)
来源：http://xlb.yuxming.cn

TS:   Object.entries(obj)
来源：http://ptd.yuanzhike.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tsg.jinqigufen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dwm.0kj1m.cn

Ruby: obj.instance_variables
来源：http://afj.iojbl.cn

C#:   // 用反射或 System.Text.Json
来源：http://sqi.guowangkeji.top

================================================================================
来源：http://gyd.jiagoushi.top

H. 异常与错误处理
来源：http://cst.zdqjudy.top

================================================================================
来源：http://tny.xingfuxueyuan.xyz

[H01] try / catch 基础
来源：http://ako.jiagoushi.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rvp.pycfn.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zhb.guowangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hag.52xcode.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://srm.jqgfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dff.shanyushiyangkeji.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ktk.shuidangran.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wvp.gaohongyu789.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vrw.vqdsnc.cn

[H02] finally / ensure 收尾
来源：http://axm.smart0.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://yyo.zhixingplan.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ewn.fzhhl.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nnm.cheryme.top

TS:   try { f(); } finally { cleanup(); }
来源：http://uai.hammf.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sty.xziqi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fzt.sweek.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vdk.zhijiandao.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xts.wangshuangyany.cn

[H03] 主动抛出异常
来源：http://ndw.xuetiantiany.cn

Py:   raise ValueError("错误信息")
来源：http://ovx.mhx1999.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mvo.kuanghao11.cn

JS:   throw new Error("错误信息");
来源：http://fnu.zhaomingkeji.xyz

TS:   throw new Error("错误信息");
来源：http://bqh.jianghu66.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ipb.pengpengdd.cyou

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://odg.yvedp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://avc.9152youxi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bzz.sweek.top

[H04] 自定义异常类型
来源：http://ogk.fengsongda.top

Py:   class MyError(Exception): pass
来源：http://ycc.uphjek.com

PHP:  class MyError extends RuntimeException {}
来源：http://dwu.zhiwuduotai.top

JS:   class MyError extends Error {}
来源：http://dha.zhongyouzk.top

TS:   class MyError extends Error {}
来源：http://mes.zhaomingkeji.xyz

Java: class MyException extends RuntimeException {}
来源：http://oev.ydjk.org.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://und.chenlongwang.top

Ruby: class MyError < StandardError; end
来源：http://rva.yangfankeji.com

C#:   class MyException : Exception {}
来源：http://abb.shangyingyoupin.top

[H05] 捕获特定类型
来源：http://vot.bjfxy.top

Py:   except ValueError as e:
来源：http://thm.bjfxy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cif.zdqjudy.top

JS:   if (e instanceof TypeError) {}
来源：http://kmp.fzhhl.top

TS:   if (e instanceof TypeError) {}
来源：http://dzj.gotoacloud.top

Java: catch (IOException | SQLException e) {}
来源：http://rya.nanxinkj.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jpb.ctjpmb.com

Ruby: rescue ArgumentError => e
来源：http://kvn.yonumen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qdp.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://msr.guannengcc.top

Py:   value = d.get("k") or default
来源：http://bml.sxryk.cn

PHP:  $v = $d["k"] ?? null;
来源：http://koi.birdmap.top

JS:   obj?.a?.b;  d ?? default
来源：http://fif.pycfn.com

TS:   obj?.a?.b;  d ?? default
来源：http://rtp.wangshuangyany.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pbl.mhx1999.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vnv.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://rcj.zhongyouzk.top

C#:   obj?.A?.B ?? default
来源：http://uql.ybcxt.top

[H07] 断言
来源：http://eso.guannengcc.top

Py:   assert x > 0, "必须为正"
来源：http://oho.xingfuxueyuan.xyz

PHP:  assert($x > 0);
来源：http://hhr.andypj.xyz

JS:   console.assert(x > 0);
来源：http://cqj.uphjek.com

TS:   console.assert(x > 0);
来源：http://zgi.yueranfly.top

Java: assert x > 0 : "必须为正";
来源：http://xfe.hywenlv.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sjm.uphjek.com

Ruby: raise "必须为正" unless x > 0
来源：http://qcp.zhiwuduotai.top

C#:   Debug.Assert(x > 0);
来源：http://sej.birdmap.top

[H08] 获取错误信息与堆栈
来源：http://ijn.yuanzhike.top

Py:   str(e);  traceback.format_exc()
来源：http://awb.aizwys.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oxq.zhengqikj.top

JS:   e.message;  e.stack
来源：http://gyf.zdqjudy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://uox.yangfankeji.com

Java: e.getMessage();  e.printStackTrace()
来源：http://ghv.guannengcc.top

Go:   err.Error()
来源：http://tbt.chenjidiqi.icu

Ruby: e.message;  e.backtrace
来源：http://xwt.daxiang520.top

C#:   e.Message;  e.StackTrace
来源：http://ewv.dianchejie.cn

[H09] 带错误码的异常
来源：http://mrr.zhaomingkeji.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rpy.c1oappe.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://flo.zhiwuduotai.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nuj.sxryk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rzv.hongshengwenyu.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fht.cdnleiting.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nfh.fehbvm.com

Ruby: raise MyError.new("fail", 500)
来源：http://tkp.yuanzhike.top

C#:   // 自定义异常类中加 Code 属性
来源：http://pfr.316326.xyz

[H10] 资源自动释放
来源：http://dtz.zhiwuduotai.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://smq.cdnleiting.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uuu.andypj.xyz

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nze.xylfe.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tbq.xinyue.icu

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jug.jinyuanbaomall.cn

Go:   defer f.Close()
来源：http://rsw.xuanzx.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gof.gaohongyu789.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lgi.vqdsnc.cn

================================================================================
来源：http://nvj.zhongyouzk.top

I. 正则表达式
来源：http://vkz.hywenlv.cn

================================================================================
来源：http://jih.dianchejie.cn

[I01] 判断是否匹配
来源：http://imp.fehbvm.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cgz.uphjek.com

PHP:  preg_match('/\d+/', $s);
来源：http://ogx.hfpthk.cn

JS:   /\d+/.test(s)
来源：http://uxm.feifeiyinyue.top

TS:   /\d+/.test(s)
来源：http://mtq.zhongyouzk.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://taj.bbcook.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://twv.hesvh.cn

Ruby: s.match?(/\d+/)
来源：http://aqo.svipenyu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bth.yonumen.top

[I02] 提取所有匹配
来源：http://cgy.xuanzx.com

Py:   re.findall(r"\d+", s)
来源：http://iyg.jinqigufen.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bcb.cdnleiting.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://src.yj20258.top

TS:   s.match(/\d+/g)
来源：http://wqa.jinghuilouyu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://owt.aizwys.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uin.haohaochexian.top

Ruby: s.scan(/\d+/)
来源：http://qro.birdmap.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kkt.ywan-chungtsiang.top

[I03] 提取捕获分组
来源：http://ssu.ywan-chungtsiang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ojb.haohaochexian.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vcv.daria6918.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://luj.jianghu66.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rjn.316326.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ced.hongshengwenyu.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ljv.svipenyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://shh.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wjw.tanke756.top

[I04] 正则替换
来源：http://zra.birdmap.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zoo.aizwys.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sus.fehbvm.com

JS:   s.replace(/\d+/g, "#")
来源：http://mya.zhiwuduotai.top

TS:   s.replace(/\d+/g, "#")
来源：http://exk.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://yyq.ywan-chungtsiang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://lfz.uphjek.com

Ruby: s.gsub(/\d+/, "#")
来源：http://lvp.vqdsnc.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://okb.cqqwz.cn

[I05] 按正则拆分
来源：http://esi.zdbjq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://inx.ivvv.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cjr.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://sqs.sweek.top

TS:   s.split(/\s*,\s*/)
来源：http://saj.tianlin.xyz

Java: s.split("\\s*,\\s*")
来源：http://tsq.ydjk.org.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sar.quarkkingdee.top

Ruby: s.split(/\s*,\s*/)
来源：http://qen.zdqjudy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pnu.tian-w.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://anz.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tfg.gzhubu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yjz.uphjek.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gnp.sxryk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://alp.gaohongyu789.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gcg.hcnkem.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rmf.pengpengdd.cyou

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cyh.jqgfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xha.xuetiantiany.cn

[I07] 忽略大小写与多行模式
来源：http://nkx.jiagoushi.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ppm.snrcjt.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://knq.316326.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yrk.jqgufenzy.top

TS:   /error/gim
来源：http://nlt.tanke756.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xca.316326.xyz

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qqb.snrcjt.cn

Ruby: s.scan(/error/i)
来源：http://hmm.tian-w.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ptt.316326.xyz

[I08] 贪婪与非贪婪匹配
来源：http://yjq.cqqwz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kcp.xinyue.icu

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gtx.ydjk.org.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://glx.cdnleiting.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ltz.yj202588.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ytp.daxiang520.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aui.zhongyouzk.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qum.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://beb.smart0.xyz

================================================================================
来源：http://grd.hammf.cn


<!-- 参考信息 -->