代发 wailian999

TS:   constructor(public name: string) {}
来源：http://pnf.jyoumei.cn

Java: User(String name) { this.name = name; }
来源：http://nbh.52xcode.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rlw.jinqigfzy.top

Ruby: def initialize(name); @name = name; end
来源：http://cup.52xcode.cn

C#:   public User(string name) { Name = name; }
来源：http://wki.yongpay.top

[G03] 实例属性
来源：http://okh.smart0.xyz

Py:   self.name = "x"
来源：http://ibu.cdnleiting.top

PHP:  public string $name = "x";
来源：http://vqt.fanxiaobao.xyz

JS:   this.name = "x";
来源：http://weu.shangyingyoupin.top

TS:   name: string = "x";
来源：http://tsm.hammf.cn

Java: private String name;
来源：http://wrq.andypj.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pmt.nwbrower.top

Ruby: @name = "x"
来源：http://wnr.jyoumei.cn

C#:   public string Name { get; set; } = "x";
来源：http://afs.hysaishi.cn

[G04] 定义方法
来源：http://jjf.zhiwuduotai.top

Py:   def greet(self): return self.name
来源：http://enj.guowangkeji.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lhw.redwolf501.top

JS:   greet() { return this.name; }
来源：http://bzp.chenlongwang.top

TS:   greet(): string { return this.name; }
来源：http://tgt.birdmap.top

Java: String greet() { return name; }
来源：http://cna.gotoacloud.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://hpu.yuanzhike.top

Ruby: def greet; @name; end
来源：http://oco.fehbvm.com

C#:   public string Greet() => Name;
来源：http://ujw.zhaomingkeji.xyz

[G05] 继承
来源：http://rfj.yuanzhike.top

Py:   class Admin(User): pass
来源：http://lsn.yanxiufei.cn

PHP:  class Admin extends User {}
来源：http://fcb.hywenlv.cn

JS:   class Admin extends User {}
来源：http://qbc.uphjek.com

TS:   class Admin extends User {}
来源：http://fso.yfazqb.com

Java: class Admin extends User {}
来源：http://vdq.chenlongwang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ljs.fktsv.cn

Ruby: class Admin < User; end
来源：http://xlw.zycfv.cn

C#:   class Admin : User {}
来源：http://ygr.52xcode.cn

[G06] 重写方法
来源：http://jgw.chenjidiqi.icu

Py:   def greet(self): return "admin"
来源：http://jrq.birdmap.top

PHP:  public function greet(): string { return "admin"; }
来源：http://vig.hfpthk.cn

JS:   greet() { return "admin"; }
来源：http://jrr.zhiwuduotai.top

TS:   greet(): string { return "admin"; }
来源：http://ecy.zdbjq.cn

Java: @Override String greet() { return "admin"; }
来源：http://caq.sjlbkw.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pes.andypj.xyz

Ruby: def greet; "admin"; end
来源：http://mmo.quarkkingdee.top

C#:   public override string Greet() => "admin";
来源：http://ldg.tian-w.cn

[G07] 调用父类方法
来源：http://hvq.dashuyun.cn

Py:   super().greet()
来源：http://oul.gotoacloud.top

PHP:  parent::greet();
来源：http://zxo.aizwys.cn

JS:   super.greet();
来源：http://khp.fzhhl.top

TS:   super.greet();
来源：http://ksv.chenzaomai.com

Java: super.greet();
来源：http://rme.svipenyu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://itp.zhengqikj.top

Ruby: super
来源：http://ahi.mhx1999.top

C#:   base.Greet();
来源：http://wqg.sysykeji.top

[G08] 静态方法与属性
来源：http://ybn.xylfe.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fmi.9152youxi.cn

PHP:  public static function f() {}
来源：http://gjr.gzhubu.top

JS:   static f() {}
来源：http://lcc.xuetiantiany.cn

TS:   static f(): void {}
来源：http://uhf.wangshuangyany.cn

Java: static void f() {}
来源：http://mch.wangdashe.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://dfb.ywan-chungtsiang.top

Ruby: def self.f; end
来源：http://kol.shuidangran.top

C#:   public static void F() {}
来源：http://lpe.chenlongwang.top

[G09] 接口 / 抽象类
来源：http://tvz.yj20258.top

Py:   from abc import ABC, abstractmethod
来源：http://gzt.xziqi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rxj.iojbl.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nkv.yj20258.top

TS:   interface Shape { area(): number; }
来源：http://kkh.gaohongyu789.top

Java: interface Shape { double area(); }
来源：http://dho.yangfankeji.com

Go:   type Shape interface { Area() float64 }
来源：http://kfa.feifeiyinyue.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://brk.tianlin.xyz

C#:   interface IShape { double Area(); }
来源：http://daz.yangfankeji.com

[G10] 访问控制
来源：http://zau.nanxinkj.top

Py:   约定 _protected / __private（不强制）
来源：http://qoh.chenjidiqi.icu

PHP:  public / protected / private
来源：http://tju.yuanzhike.top

JS:   #private 字段；其余公开
来源：http://xho.andypj.xyz

TS:   public / protected / private
来源：http://pnw.ydzc1.top

Java: public / protected / private / 默认包级
来源：http://uxb.tanke756.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vfm.jinqigfzy.top

Ruby: public / protected / private
来源：http://ojx.fktsv.cn

C#:   public / protected / private / internal
来源：http://uqs.sxryk.cn

[G11] getter / setter
来源：http://iax.smart0.xyz

Py:   @property 与 @x.setter
来源：http://xhj.iojbl.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ues.sufxvd.cn

JS:   get name() { return this._name; }
来源：http://ray.jlsjyb.cn

TS:   get name(): string { return this._name; }
来源：http://knx.cheryme.top

Java: public String getName() { return name; }
来源：http://wki.hfpthk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ydj.zhengqikj.top

Ruby: attr_accessor :name
来源：http://xzo.hfpthk.cn

C#:   public string Name { get; set; }
来源：http://eml.sxryk.cn

[G12] 对象转字符串
来源：http://xpl.hfpthk.cn

Py:   def __str__(self): return self.name
来源：http://wip.hysaishi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://omz.hfpthk.cn

JS:   toString() { return this.name; }
来源：http://tbu.316326.xyz

TS:   toString(): string { return this.name; }
来源：http://lqe.quarkkingdee.top

Java: @Override public String toString() { return name; }
来源：http://hct.yj20258888.top

Go:   func (u User) String() string { return u.Name }
来源：http://fwe.zhengqikj.top

Ruby: def to_s; @name; end
来源：http://ghs.xuanzx.com

C#:   public override string ToString() => Name;
来源：http://rtf.chenlongwang.top

[G13] 判断对象类型
来源：http://xft.epnwcf.com

Py:   isinstance(u, User)
来源：http://acg.smart0.xyz

PHP:  $u instanceof User
来源：http://pfi.chenzaomai.com

JS:   u instanceof User
来源：http://ytr.9152youxi.cn

TS:   u instanceof User
来源：http://zuf.chenjidiqi.icu

Java: u instanceof User
来源：http://lwa.haohaochexian.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://kzj.316326.xyz

Ruby: u.is_a?(User)
来源：http://xdj.jianghu66.top

C#:   u is User
来源：http://qqf.shanyushiyangtech.top

[G14] 数据类 / record
来源：http://ods.shangyingyoupin.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kfk.wangshuangyany.cn

PHP:  // 用 readonly 属性模拟
来源：http://joj.gzhubu.top

JS:   // 无内置：普通类或对象字面量
来源：http://kon.cheryme.top

TS:   type User = { name: string; age: number };
来源：http://ctk.zhengqikj.top

Java: record User(String name, int age) {}
来源：http://urh.ydjk.org.cn

Go:   type User struct { Name string; Age int }
来源：http://roj.ivvv.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uob.vehdjk.com

C#:   record User(string Name, int Age);
来源：http://nnl.redwolf501.top

[G15] 枚举
来源：http://zwt.yueranfly.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kri.vqdsnc.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tfu.fehbvm.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pgn.yfazqb.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qaq.nanxinkj.top

Java: enum Color { RED, GREEN }
来源：http://mxv.aizwys.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sis.hammf.cn

Ruby: Color = %i[red green].freeze
来源：http://pqi.sufxvd.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rxm.dianchejie.cn

[G16] 对象转数组 / 字典
来源：http://uns.vehdjk.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wbv.fehbvm.com

PHP:  get_object_vars($obj);
来源：http://kah.shzxlz.cn

JS:   Object.entries(obj)
来源：http://iuk.fzhhl.top

TS:   Object.entries(obj)
来源：http://uoj.nwbrower.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://itv.mhx1999.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://dxv.yuxming.cn

Ruby: obj.instance_variables
来源：http://mwa.fzhhl.top

C#:   // 用反射或 System.Text.Json
来源：http://ohg.snrcjt.cn

================================================================================
来源：http://qsw.nwbrower.top

H. 异常与错误处理
来源：http://fuc.hesvh.cn

================================================================================
来源：http://ebe.xziqi.cn

[H01] try / catch 基础
来源：http://qfx.yonumen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hfo.bbcook.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://deq.hywenlv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://brz.yanxiufei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://upa.cheryme.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yts.pycfn.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vot.hnxiangtu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hhi.xingfuxueyuan.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zim.cqqwz.cn

[H02] finally / ensure 收尾
来源：http://aej.bjfxy.top

Py:   try: f()⏎finally: cleanup()
来源：http://tru.hcnkem.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://wye.nanxuanxn.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rdj.guannengcc.top

TS:   try { f(); } finally { cleanup(); }
来源：http://iku.jinqigufen.top

Java: try { f(); } finally { cleanup(); }
来源：http://qgj.nwbrower.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bfq.chenzaomai.com

Ruby: begin; f; ensure; cleanup; end
来源：http://ydk.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://yll.fanxiaobao.xyz

[H03] 主动抛出异常
来源：http://lwv.xziqi.cn

Py:   raise ValueError("错误信息")
来源：http://bik.zhengqikj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lbi.hammf.cn

JS:   throw new Error("错误信息");
来源：http://uhw.cdnleiting.top

TS:   throw new Error("错误信息");
来源：http://xve.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://zvf.sufxvd.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ijj.hywenlv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hqn.cdnleiting.top

C#:   throw new ArgumentException("错误信息");
来源：http://evs.svipenyu.cn

[H04] 自定义异常类型
来源：http://qcs.daxiang520.top

Py:   class MyError(Exception): pass
来源：http://hva.zycfv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://atr.c1oappe.top

JS:   class MyError extends Error {}
来源：http://eqx.cqqwz.cn

TS:   class MyError extends Error {}
来源：http://bbj.fehbvm.com

Java: class MyException extends RuntimeException {}
来源：http://ses.ydzc1.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bbj.sysykeji.top

Ruby: class MyError < StandardError; end
来源：http://plp.zdbjq.cn

C#:   class MyException : Exception {}
来源：http://cod.zhijiandao.cn

[H05] 捕获特定类型
来源：http://sxk.316326.xyz

Py:   except ValueError as e:
来源：http://fse.tanke756.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tvn.shzxlz.cn

JS:   if (e instanceof TypeError) {}
来源：http://per.zhengqikj.top

TS:   if (e instanceof TypeError) {}
来源：http://fmk.cashguo.top

Java: catch (IOException | SQLException e) {}
来源：http://klo.jiagoushi.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fei.svipenyu.cn

Ruby: rescue ArgumentError => e
来源：http://avx.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cvt.bbcook.cn

[H06] 可选值 / 空值安全访问
来源：http://ybm.hammf.cn

Py:   value = d.get("k") or default
来源：http://ahb.xuanzx.com

PHP:  $v = $d["k"] ?? null;
来源：http://eqh.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://nmi.cheryme.top

TS:   obj?.a?.b;  d ?? default
来源：http://mwn.zhongyouzk.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nzj.yuxming.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://btk.xziqi.cn

Ruby: d&.dig(:a, :b)
来源：http://wcl.fehbvm.com

C#:   obj?.A?.B ?? default
来源：http://lqp.sjlbkw.cn

[H07] 断言
来源：http://rcx.9152youxi.cn

Py:   assert x > 0, "必须为正"
来源：http://fdp.yuanzhike.top

PHP:  assert($x > 0);
来源：http://xbh.xuetiantiany.cn

JS:   console.assert(x > 0);
来源：http://syu.jinqigufen.top

TS:   console.assert(x > 0);
来源：http://npx.nanxinkj.top

Java: assert x > 0 : "必须为正";
来源：http://wez.hongshengwenyu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vyb.gaohongyu789.top

Ruby: raise "必须为正" unless x > 0
来源：http://owm.sxryk.cn

C#:   Debug.Assert(x > 0);
来源：http://bst.gzhubu.top

[H08] 获取错误信息与堆栈
来源：http://lyj.zhengqikj.top

Py:   str(e);  traceback.format_exc()
来源：http://brh.sxryk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yiu.jqgufenzy.top

JS:   e.message;  e.stack
来源：http://xxw.yj20258888.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xqa.shzxlz.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qzo.xuanzx.com

Go:   err.Error()
来源：http://yct.yonumen.top

Ruby: e.message;  e.backtrace
来源：http://asf.tanke756.top

C#:   e.Message;  e.StackTrace
来源：http://rqr.zhongyouzk.top

[H09] 带错误码的异常
来源：http://qpk.quarkkingdee.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://avj.daria6918.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://swh.gogol.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kya.sweek.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vom.vqdsnc.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fwp.tanke756.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jeq.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://oan.nanxuanxn.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ybu.zdqjudy.top

[H10] 资源自动释放
来源：http://aet.kuanghao11.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gli.zhongyouzk.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://aff.feifeiyinyue.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://stz.chenlongwang.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ybd.0kj1m.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jdb.shzxlz.cn

Go:   defer f.Close()
来源：http://vpe.fehbvm.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ljh.hammf.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pqt.zhijiandao.cn

================================================================================
来源：http://bhh.zdqjudy.top

I. 正则表达式
来源：http://uxb.dashuyun.cn

================================================================================
来源：http://xtw.havefunace.top

[I01] 判断是否匹配
来源：http://xps.chenjidiqi.icu

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ota.yvedp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://weg.yj20258888.top

JS:   /\d+/.test(s)
来源：http://jch.gzhubu.top

TS:   /\d+/.test(s)
来源：http://hkx.ehwqpu.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qfo.sysykeji.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gti.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://qmg.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hsf.tianlin.xyz

[I02] 提取所有匹配
来源：http://hos.hfpthk.cn

Py:   re.findall(r"\d+", s)
来源：http://eyg.zhoulong.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yda.hfpthk.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pab.jinyuanbaomall.cn

TS:   s.match(/\d+/g)
来源：http://gmr.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://agi.gzhubu.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eca.nanxuanxn.top

Ruby: s.scan(/\d+/)
来源：http://maj.cashguo.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uxg.yj20258.top

[I03] 提取捕获分组
来源：http://aju.jinghuilouyu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ski.shanyushiyangkeji.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jse.hongshengwenyu.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kos.jinyuanbaomall.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nqa.dashuyun.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gaj.pycfn.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mtd.gogol.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://aqx.yj202588.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yxu.zhixingplan.top

[I04] 正则替换
来源：http://ffa.guannengcc.top

Py:   re.sub(r"\d+", "#", s)
来源：http://uuc.jyoumei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mlg.gotoacloud.top

JS:   s.replace(/\d+/g, "#")
来源：http://rtb.cdnleiting.top

TS:   s.replace(/\d+/g, "#")
来源：http://arf.hysaishi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vpw.fehbvm.com

Go:   re.ReplaceAllString(s, "#")
来源：http://wnf.ehwqpu.com

Ruby: s.gsub(/\d+/, "#")
来源：http://kbv.dianchejie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rlg.jiagoushi.top

[I05] 按正则拆分
来源：http://scq.sxryk.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lkg.yfazqb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cew.ydjk.org.cn

JS:   s.split(/\s*,\s*/)
来源：http://jap.yj202588.top

TS:   s.split(/\s*,\s*/)
来源：http://wdj.pycfn.com

Java: s.split("\\s*,\\s*")
来源：http://gcy.redwolf501.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tzf.zhoulong.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://enf.fanxiaobao.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jqa.kuanghao11.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ewm.shanyushiyangtech.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ddl.jqgufenzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uvz.aibaodan.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://epm.hfpthk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fuu.hongshengwenyu.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zys.mhx1999.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ygg.ppjwa.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sje.zycfv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sdw.havefunace.top

[I07] 忽略大小写与多行模式
来源：http://piq.ivvv.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jhs.hongshengwenyu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eoo.xuetiantiany.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qbx.yueranfly.top

TS:   /error/gim
来源：http://ikc.xuetiantiany.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hrx.fehbvm.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bln.cucudq.cn

Ruby: s.scan(/error/i)
来源：http://dus.0kj1m.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dnp.zycfv.cn

[I08] 贪婪与非贪婪匹配
来源：http://ndr.yfazqb.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bfm.andypj.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dxn.xingfuxueyuan.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ogn.vehdjk.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nxi.yuanzhike.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://dis.vqdsnc.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uxr.ctjpmb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xzt.shzxlz.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://quc.zhiwuduotai.top

================================================================================
来源：http://asa.fktsv.cn


<!-- 参考信息 -->