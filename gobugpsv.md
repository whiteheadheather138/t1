代发 wailian999

[G02] 构造函数
来源：http://pqz.wangdashe.top

Py:   def __init__(self, name): self.name = name
来源：http://sip.cucudq.cn

PHP:  public function __construct(public string $name) {}
来源：http://iea.bbcook.cn

JS:   constructor(name) { this.name = name; }
来源：http://zyo.hcnkem.com

TS:   constructor(public name: string) {}
来源：http://pvb.fengsongda.top

Java: User(String name) { this.name = name; }
来源：http://cnn.chenjidiqi.icu

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vva.cashguo.top

Ruby: def initialize(name); @name = name; end
来源：http://ftl.fanxiaobao.xyz

C#:   public User(string name) { Name = name; }
来源：http://yky.wangdashe.top

[G03] 实例属性
来源：http://vug.bbcook.cn

Py:   self.name = "x"
来源：http://cci.zhixingplan.top

PHP:  public string $name = "x";
来源：http://gfh.ctjpmb.com

JS:   this.name = "x";
来源：http://uqx.ctjpmb.com

TS:   name: string = "x";
来源：http://wkx.tianlin.xyz

Java: private String name;
来源：http://afs.zhoulong.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qsr.dashuyun.cn

Ruby: @name = "x"
来源：http://yux.birdmap.top

C#:   public string Name { get; set; } = "x";
来源：http://vnl.0kj1m.cn

[G04] 定义方法
来源：http://kdj.hnxiangtu.top

Py:   def greet(self): return self.name
来源：http://xig.andypj.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://bsc.shangyingyoupin.top

JS:   greet() { return this.name; }
来源：http://wok.jqgufenzy.top

TS:   greet(): string { return this.name; }
来源：http://rzg.fanxiaobao.xyz

Java: String greet() { return name; }
来源：http://rfc.shanyushiyangkeji.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://yzz.shzxlz.cn

Ruby: def greet; @name; end
来源：http://wgs.ydjk.org.cn

C#:   public string Greet() => Name;
来源：http://azr.xuetiantiany.cn

[G05] 继承
来源：http://tth.iojbl.cn

Py:   class Admin(User): pass
来源：http://tky.gzhubu.top

PHP:  class Admin extends User {}
来源：http://kcz.316326.xyz

JS:   class Admin extends User {}
来源：http://vkz.shuidangran.top

TS:   class Admin extends User {}
来源：http://vsw.zhaomingkeji.xyz

Java: class Admin extends User {}
来源：http://pjl.redwolf501.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qkq.zhoulong.xyz

Ruby: class Admin < User; end
来源：http://upv.ehwqpu.com

C#:   class Admin : User {}
来源：http://yrq.gaohongyu789.top

[G06] 重写方法
来源：http://yhm.chenlongwang.top

Py:   def greet(self): return "admin"
来源：http://jag.zhiwuduotai.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kqe.yfazqb.com

JS:   greet() { return "admin"; }
来源：http://jcr.meibo888.top

TS:   greet(): string { return "admin"; }
来源：http://bli.gaohongyu789.top

Java: @Override String greet() { return "admin"; }
来源：http://vzw.sjlbkw.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lsg.shuidangran.top

Ruby: def greet; "admin"; end
来源：http://hia.zhixingplan.top

C#:   public override string Greet() => "admin";
来源：http://nbj.jinyuanbaomall.cn

[G07] 调用父类方法
来源：http://ajx.cucudq.cn

Py:   super().greet()
来源：http://uce.9152youxi.cn

PHP:  parent::greet();
来源：http://cjv.shzxlz.cn

JS:   super.greet();
来源：http://hrx.vqdsnc.cn

TS:   super.greet();
来源：http://jzz.fehbvm.com

Java: super.greet();
来源：http://acf.hnxiangtu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lph.sufxvd.cn

Ruby: super
来源：http://cra.yongpay.top

C#:   base.Greet();
来源：http://ufh.0kj1m.cn

[G08] 静态方法与属性
来源：http://zup.yuanzhike.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xvj.aibaodan.cn

PHP:  public static function f() {}
来源：http://qqt.xylfe.cn

JS:   static f() {}
来源：http://xrr.xingfuxueyuan.xyz

TS:   static f(): void {}
来源：http://eme.guannengcc.top

Java: static void f() {}
来源：http://iud.aizwys.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bpw.dianchejie.cn

Ruby: def self.f; end
来源：http://nrd.iojbl.cn

C#:   public static void F() {}
来源：http://dwu.bjfxy.top

[G09] 接口 / 抽象类
来源：http://por.yuanzhike.top

Py:   from abc import ABC, abstractmethod
来源：http://cfl.pengpengdd.cyou

PHP:  interface Shape { public function area(): float; }
来源：http://okw.ybcxt.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://zog.jlsjyb.cn

TS:   interface Shape { area(): number; }
来源：http://eyr.hammf.cn

Java: interface Shape { double area(); }
来源：http://oqc.cqqwz.cn

Go:   type Shape interface { Area() float64 }
来源：http://tmt.jianghu66.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hnu.yvedp.cn

C#:   interface IShape { double Area(); }
来源：http://ufi.shangyingyoupin.top

[G10] 访问控制
来源：http://cql.gotoacloud.top

Py:   约定 _protected / __private（不强制）
来源：http://uls.hysaishi.cn

PHP:  public / protected / private
来源：http://pzx.yongpay.top

JS:   #private 字段；其余公开
来源：http://imk.gzhubu.top

TS:   public / protected / private
来源：http://xsg.ywan-chungtsiang.top

Java: public / protected / private / 默认包级
来源：http://hkl.feifeiyinyue.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qfa.xziqi.cn

Ruby: public / protected / private
来源：http://aoz.nanxuanxn.top

C#:   public / protected / private / internal
来源：http://bcr.quarkkingdee.top

[G11] getter / setter
来源：http://vwx.cashguo.top

Py:   @property 与 @x.setter
来源：http://eia.dashuyun.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jeh.hnqzz.top

JS:   get name() { return this._name; }
来源：http://bst.zhengqikj.top

TS:   get name(): string { return this._name; }
来源：http://spu.hnqzz.top

Java: public String getName() { return name; }
来源：http://npf.jyoumei.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gbj.xinyue.icu

Ruby: attr_accessor :name
来源：http://oqe.xylfe.cn

C#:   public string Name { get; set; }
来源：http://rnt.dashuyun.cn

[G12] 对象转字符串
来源：http://gic.tian-w.cn

Py:   def __str__(self): return self.name
来源：http://myq.0kj1m.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nvg.zhoulong.xyz

JS:   toString() { return this.name; }
来源：http://idg.yonumen.top

TS:   toString(): string { return this.name; }
来源：http://cep.52xcode.cn

Java: @Override public String toString() { return name; }
来源：http://xcm.bjfxy.top

Go:   func (u User) String() string { return u.Name }
来源：http://eef.cucudq.cn

Ruby: def to_s; @name; end
来源：http://axn.sweek.top

C#:   public override string ToString() => Name;
来源：http://fqm.zhoulong.xyz

[G13] 判断对象类型
来源：http://vau.hcnkem.com

Py:   isinstance(u, User)
来源：http://jlx.chenjidiqi.icu

PHP:  $u instanceof User
来源：http://ydv.andypj.xyz

JS:   u instanceof User
来源：http://grh.zhongyouzk.top

TS:   u instanceof User
来源：http://fod.haohaochexian.top

Java: u instanceof User
来源：http://lxm.zhijiandao.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://avy.gaohongyu789.top

Ruby: u.is_a?(User)
来源：http://saw.jinqigfzy.top

C#:   u is User
来源：http://rch.zhongyouzk.top

[G14] 数据类 / record
来源：http://opq.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kwz.fengsongda.top

PHP:  // 用 readonly 属性模拟
来源：http://dfb.shanyushiyangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://ohc.zhiwuduotai.top

TS:   type User = { name: string; age: number };
来源：http://gmb.smart0.xyz

Java: record User(String name, int age) {}
来源：http://kip.kuanghao11.cn

Go:   type User struct { Name string; Age int }
来源：http://uju.xylfe.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vga.jinyuanbaomall.cn

C#:   record User(string Name, int Age);
来源：http://tfk.zhiwuduotai.top

[G15] 枚举
来源：http://qqr.shanyushiyangkeji.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zws.yj20258.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ngr.xuetiantiany.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://asg.hcnkem.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qlp.birdmap.top

Java: enum Color { RED, GREEN }
来源：http://qae.zhaomingkeji.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wau.0kj1m.cn

Ruby: Color = %i[red green].freeze
来源：http://ldb.hesvh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fsi.mhx1999.top

[G16] 对象转数组 / 字典
来源：http://cke.yj20258888.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dri.dianchejie.cn

PHP:  get_object_vars($obj);
来源：http://uey.chenjidiqi.icu

JS:   Object.entries(obj)
来源：http://fwl.xinyue.icu

TS:   Object.entries(obj)
来源：http://yub.ywan-chungtsiang.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zlq.aibaodan.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gnc.dianchejie.cn

Ruby: obj.instance_variables
来源：http://jck.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://xeh.zhongyouzk.top

================================================================================
来源：http://uws.yvedp.cn

H. 异常与错误处理
来源：http://hci.jlsjyb.cn

================================================================================
来源：http://wlh.zhengqikj.top

[H01] try / catch 基础
来源：http://ywv.nanxuanxn.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://awd.yueranfly.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sad.cdnleiting.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ydb.sjlbkw.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jjn.haohaochexian.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vvj.yj20258888.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fhc.sweek.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fnw.aizwys.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bgz.jqgfzy.top

[H02] finally / ensure 收尾
来源：http://egm.feifeiyinyue.top

Py:   try: f()⏎finally: cleanup()
来源：http://zjg.haohaochexian.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://dgw.aizwys.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iqu.jinyuanbaomall.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://euq.yj202588.top

Java: try { f(); } finally { cleanup(); }
来源：http://llc.zhongyouzk.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://oca.meibo888.top

Ruby: begin; f; ensure; cleanup; end
来源：http://olr.sxryk.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ote.pycfn.com

[H03] 主动抛出异常
来源：http://txa.9152youxi.cn

Py:   raise ValueError("错误信息")
来源：http://qcg.daria6918.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://few.fktsv.cn

JS:   throw new Error("错误信息");
来源：http://gyi.jinghuilouyu.cn

TS:   throw new Error("错误信息");
来源：http://kwa.ybcxt.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://yxk.ybcxt.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xxm.ybcxt.top

Ruby: raise ArgumentError, "错误信息"
来源：http://vxa.ehwqpu.com

C#:   throw new ArgumentException("错误信息");
来源：http://vyn.zdqjudy.top

[H04] 自定义异常类型
来源：http://tac.chenzaomai.com

Py:   class MyError(Exception): pass
来源：http://ciz.xuetiantiany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bwe.bjfxy.top

JS:   class MyError extends Error {}
来源：http://wxo.chenlongwang.top

TS:   class MyError extends Error {}
来源：http://ems.meibo888.top

Java: class MyException extends RuntimeException {}
来源：http://wbr.shanyushiyangtech.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://niq.ppjwa.cn

Ruby: class MyError < StandardError; end
来源：http://xps.shuidangran.top

C#:   class MyException : Exception {}
来源：http://tdn.gotoacloud.top

[H05] 捕获特定类型
来源：http://hlc.shanyushiyangkeji.top

Py:   except ValueError as e:
来源：http://fon.jinqigufen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dld.vehdjk.com

JS:   if (e instanceof TypeError) {}
来源：http://dio.xuanzx.com

TS:   if (e instanceof TypeError) {}
来源：http://ibl.yfazqb.com

Java: catch (IOException | SQLException e) {}
来源：http://dpx.mhx1999.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gpq.tanke756.top

Ruby: rescue ArgumentError => e
来源：http://jto.zdqjudy.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lns.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://gjb.zhoulong.xyz

Py:   value = d.get("k") or default
来源：http://blf.ppjwa.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nqz.ppjwa.cn

JS:   obj?.a?.b;  d ?? default
来源：http://unu.0kj1m.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qat.tianlin.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://spp.tarul.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tew.vqdsnc.cn

Ruby: d&.dig(:a, :b)
来源：http://lmy.cashguo.top

C#:   obj?.A?.B ?? default
来源：http://vlx.mhx1999.top

[H07] 断言
来源：http://hns.yangfankeji.com

Py:   assert x > 0, "必须为正"
来源：http://vzq.bjfxy.top

PHP:  assert($x > 0);
来源：http://gyq.ydjk.org.cn

JS:   console.assert(x > 0);
来源：http://vmy.iojbl.cn

TS:   console.assert(x > 0);
来源：http://ezy.kuanghao11.cn

Java: assert x > 0 : "必须为正";
来源：http://hpv.yongpay.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vrw.jqgfzy.top

Ruby: raise "必须为正" unless x > 0
来源：http://ciw.cdnleiting.top

C#:   Debug.Assert(x > 0);
来源：http://czp.zycfv.cn

[H08] 获取错误信息与堆栈
来源：http://mtz.feifeiyinyue.top

Py:   str(e);  traceback.format_exc()
来源：http://fad.fktsv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://efj.yuanzhike.top

JS:   e.message;  e.stack
来源：http://vih.chenjidiqi.icu

TS:   e instanceof Error ? e.message : String(e)
来源：http://hwt.quarkkingdee.top

Java: e.getMessage();  e.printStackTrace()
来源：http://phz.hfpthk.cn

Go:   err.Error()
来源：http://ddw.ehwqpu.com

Ruby: e.message;  e.backtrace
来源：http://zym.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://qjh.hywenlv.cn

[H09] 带错误码的异常
来源：http://nte.zhaomingkeji.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gfk.yvedp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zty.pengpengdd.cyou

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fwz.9152youxi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mdv.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fkx.fehbvm.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xgj.jinqigfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://ian.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://ril.sxryk.cn

[H10] 资源自动释放
来源：http://edb.andypj.xyz

Py:   with open("a.txt") as f: data = f.read()
来源：http://tku.ybcxt.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://imi.hnqzz.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oaj.shuidangran.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://olz.fehbvm.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nlv.hfpthk.cn

Go:   defer f.Close()
来源：http://lem.nwbrower.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qri.ybcxt.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cep.sweek.top

================================================================================
来源：http://rwm.pengpengdd.cyou

I. 正则表达式
来源：http://gms.jqgufenzy.top

================================================================================
来源：http://hda.gaohongyu789.top

[I01] 判断是否匹配
来源：http://lzs.gogol.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kbm.yongpay.top

PHP:  preg_match('/\d+/', $s);
来源：http://ihm.ivvv.top

JS:   /\d+/.test(s)
来源：http://hpc.wangdashe.top

TS:   /\d+/.test(s)
来源：http://sfm.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fos.sufxvd.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://udd.zdbjq.cn

Ruby: s.match?(/\d+/)
来源：http://kuf.vehdjk.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fyx.fengsongda.top

[I02] 提取所有匹配
来源：http://egz.shanyushiyangkeji.top

Py:   re.findall(r"\d+", s)
来源：http://mkq.cheryme.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qce.dashuyun.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xby.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://eez.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zxr.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://skp.birdmap.top

Ruby: s.scan(/\d+/)
来源：http://tpb.sjlbkw.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cjd.zdbjq.cn

[I03] 提取捕获分组
来源：http://kyj.9152youxi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rlj.quarkkingdee.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://waj.yvedp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fln.pengpengdd.cyou

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://soe.ehwqpu.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yaa.jlsjyb.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rvi.cqqwz.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tlm.jinqigfzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xue.c1oappe.top

[I04] 正则替换
来源：http://bqx.jqgufenzy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://tee.guannengcc.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jxh.mhx1999.top

JS:   s.replace(/\d+/g, "#")
来源：http://nqz.redwolf501.top

TS:   s.replace(/\d+/g, "#")
来源：http://juc.xinyue.icu

Java: s.replaceAll("\\d+", "#")
来源：http://qyz.kuanghao11.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dmt.jqgufenzy.top

Ruby: s.gsub(/\d+/, "#")
来源：http://nyv.cucudq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dcp.hywenlv.cn

[I05] 按正则拆分
来源：http://rlp.cucudq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ptk.pycfn.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://acq.birdmap.top

JS:   s.split(/\s*,\s*/)
来源：http://ehp.zhoulong.xyz

TS:   s.split(/\s*,\s*/)
来源：http://eiv.ydzc1.top

Java: s.split("\\s*,\\s*")
来源：http://fji.cdnleiting.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sjg.hongshengwenyu.top

Ruby: s.split(/\s*,\s*/)
来源：http://zqz.vehdjk.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ojl.chenlongwang.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nuc.sjlbkw.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pqe.ehwqpu.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lks.gogol.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://czm.fengsongda.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hlp.aibaodan.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cfv.tianlin.xyz

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://isu.xylfe.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qxj.yj20258888.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vmn.guannengcc.top

[I07] 忽略大小写与多行模式
来源：http://dxf.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rfl.jinghuilouyu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gwl.shangyingyoupin.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zzp.hnqzz.top

TS:   /error/gim
来源：http://yuy.ehwqpu.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rsi.c1oappe.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mmt.fktsv.cn

Ruby: s.scan(/error/i)
来源：http://ehj.xuanzx.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ztx.gaohongyu789.top

[I08] 贪婪与非贪婪匹配
来源：http://sfr.vqdsnc.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gmy.nanxuanxn.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ngy.redwolf501.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sqz.jinyuanbaomall.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lxv.c1oappe.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://jds.zycfv.cn


<!-- 参考信息 -->