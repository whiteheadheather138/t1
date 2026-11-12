代发 wailian999

Py:   class User: pass
来源：http://hkv.gotoacloud.top

PHP:  class User {}
来源：http://wja.yueranfly.top

JS:   class User {}
来源：http://eyd.yuanzhike.top

TS:   class User { name: string = ""; }
来源：http://hqg.ctjpmb.com

Java: class User {}
来源：http://dol.sufxvd.cn

Go:   type User struct { Name string }
来源：http://zod.smart0.xyz

Ruby: class User; end
来源：http://acf.zhijiandao.cn

C#:   class User {}
来源：http://xmh.hnqzz.top

[G02] 构造函数
来源：http://cdh.xinyue.icu

Py:   def __init__(self, name): self.name = name
来源：http://qec.haohaochexian.top

PHP:  public function __construct(public string $name) {}
来源：http://sdw.yj20258888.top

JS:   constructor(name) { this.name = name; }
来源：http://irh.pycfn.com

TS:   constructor(public name: string) {}
来源：http://app.ybcxt.top

Java: User(String name) { this.name = name; }
来源：http://lgx.jqgufenzy.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ilt.jianghu66.top

Ruby: def initialize(name); @name = name; end
来源：http://mts.xziqi.cn

C#:   public User(string name) { Name = name; }
来源：http://hgj.hongshengwenyu.top

[G03] 实例属性
来源：http://pdl.mhx1999.top

Py:   self.name = "x"
来源：http://sss.nanxuanxn.top

PHP:  public string $name = "x";
来源：http://chn.kuanghao11.cn

JS:   this.name = "x";
来源：http://vrr.fanxiaobao.xyz

TS:   name: string = "x";
来源：http://ogk.tanke756.top

Java: private String name;
来源：http://nhr.gaohongyu789.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kcw.zhaomingkeji.xyz

Ruby: @name = "x"
来源：http://kqw.hnqzz.top

C#:   public string Name { get; set; } = "x";
来源：http://gej.0kj1m.cn

[G04] 定义方法
来源：http://jct.xziqi.cn

Py:   def greet(self): return self.name
来源：http://diu.zdbjq.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://eum.yj20258888.top

JS:   greet() { return this.name; }
来源：http://atn.daria6918.cn

TS:   greet(): string { return this.name; }
来源：http://lsw.gzhubu.top

Java: String greet() { return name; }
来源：http://cbn.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://sld.svipenyu.cn

Ruby: def greet; @name; end
来源：http://rvz.xylfe.cn

C#:   public string Greet() => Name;
来源：http://cib.jinqigfzy.top

[G05] 继承
来源：http://thu.uphjek.com

Py:   class Admin(User): pass
来源：http://ect.hysaishi.cn

PHP:  class Admin extends User {}
来源：http://gga.gogol.net.cn

JS:   class Admin extends User {}
来源：http://ytt.nwbrower.top

TS:   class Admin extends User {}
来源：http://hne.quarkkingdee.top

Java: class Admin extends User {}
来源：http://iho.shzxlz.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mln.dianchejie.cn

Ruby: class Admin < User; end
来源：http://cgg.gzhubu.top

C#:   class Admin : User {}
来源：http://kzq.zhongyouzk.top

[G06] 重写方法
来源：http://pdy.yuanzhike.top

Py:   def greet(self): return "admin"
来源：http://rwn.c1oappe.top

PHP:  public function greet(): string { return "admin"; }
来源：http://lkz.zdbjq.cn

JS:   greet() { return "admin"; }
来源：http://itm.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://vcn.nanxuanxn.top

Java: @Override String greet() { return "admin"; }
来源：http://ril.gotoacloud.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://khc.sysykeji.top

Ruby: def greet; "admin"; end
来源：http://cns.ywan-chungtsiang.top

C#:   public override string Greet() => "admin";
来源：http://pbr.fengsongda.top

[G07] 调用父类方法
来源：http://tmo.uphjek.com

Py:   super().greet()
来源：http://fal.nanxinkj.top

PHP:  parent::greet();
来源：http://ccg.tarul.cn

JS:   super.greet();
来源：http://ggp.ctjpmb.com

TS:   super.greet();
来源：http://pjh.tianlin.xyz

Java: super.greet();
来源：http://csg.fktsv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uhc.c1oappe.top

Ruby: super
来源：http://ssb.nwbrower.top

C#:   base.Greet();
来源：http://khx.jianghu66.top

[G08] 静态方法与属性
来源：http://xec.smart0.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jga.chenjidiqi.icu

PHP:  public static function f() {}
来源：http://mua.wangdashe.top

JS:   static f() {}
来源：http://gli.jqgufenzy.top

TS:   static f(): void {}
来源：http://jml.sweek.top

Java: static void f() {}
来源：http://nev.gaohongyu789.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://kpj.sweek.top

Ruby: def self.f; end
来源：http://mkv.shangyingyoupin.top

C#:   public static void F() {}
来源：http://qla.hnqzz.top

[G09] 接口 / 抽象类
来源：http://lsa.cheryme.top

Py:   from abc import ABC, abstractmethod
来源：http://uan.daria6918.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fcv.dashuyun.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qwf.cucudq.cn

TS:   interface Shape { area(): number; }
来源：http://joc.zhengqikj.top

Java: interface Shape { double area(); }
来源：http://qet.dashuyun.cn

Go:   type Shape interface { Area() float64 }
来源：http://jnd.birdmap.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tfm.ywan-chungtsiang.top

C#:   interface IShape { double Area(); }
来源：http://fsr.xuetiantiany.cn

[G10] 访问控制
来源：http://hrh.sxryk.cn

Py:   约定 _protected / __private（不强制）
来源：http://esl.zhongyouzk.top

PHP:  public / protected / private
来源：http://qip.fzhhl.top

JS:   #private 字段；其余公开
来源：http://fcf.yangfankeji.com

TS:   public / protected / private
来源：http://xvf.uphjek.com

Java: public / protected / private / 默认包级
来源：http://uip.andypj.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://swn.tarul.cn

Ruby: public / protected / private
来源：http://bei.vqdsnc.cn

C#:   public / protected / private / internal
来源：http://gwp.sjlbkw.cn

[G11] getter / setter
来源：http://vnr.316326.xyz

Py:   @property 与 @x.setter
来源：http://gke.jianghu66.top

PHP:  public function getName(): string { return $this->name; }
来源：http://kvi.fehbvm.com

JS:   get name() { return this._name; }
来源：http://ima.nanxuanxn.top

TS:   get name(): string { return this._name; }
来源：http://kvx.hnqzz.top

Java: public String getName() { return name; }
来源：http://adi.hnqzz.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://ixu.chenzaomai.com

Ruby: attr_accessor :name
来源：http://lis.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://ycz.jinqigufen.top

[G12] 对象转字符串
来源：http://tss.hnqzz.top

Py:   def __str__(self): return self.name
来源：http://nfb.andypj.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://rpy.yueranfly.top

JS:   toString() { return this.name; }
来源：http://dhp.zhengqikj.top

TS:   toString(): string { return this.name; }
来源：http://lsj.meibo888.top

Java: @Override public String toString() { return name; }
来源：http://eaq.sysykeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://fbh.yj202588.top

Ruby: def to_s; @name; end
来源：http://sdl.jyoumei.cn

C#:   public override string ToString() => Name;
来源：http://hoh.tanke756.top

[G13] 判断对象类型
来源：http://eih.jinghuilouyu.cn

Py:   isinstance(u, User)
来源：http://syc.tanke756.top

PHP:  $u instanceof User
来源：http://cqk.fzhhl.top

JS:   u instanceof User
来源：http://jhp.smart0.xyz

TS:   u instanceof User
来源：http://ehz.daxiang520.top

Java: u instanceof User
来源：http://cas.jinqigufen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://feu.ydjk.org.cn

Ruby: u.is_a?(User)
来源：http://gnh.zhongyouzk.top

C#:   u is User
来源：http://qsz.mhx1999.top

[G14] 数据类 / record
来源：http://hyg.xuanzx.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cwa.xziqi.cn

PHP:  // 用 readonly 属性模拟
来源：http://pwd.cheryme.top

JS:   // 无内置：普通类或对象字面量
来源：http://wpf.redwolf501.top

TS:   type User = { name: string; age: number };
来源：http://hsw.sxryk.cn

Java: record User(String name, int age) {}
来源：http://dtw.hysaishi.cn

Go:   type User struct { Name string; Age int }
来源：http://oaw.zycfv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yzz.daria6918.cn

C#:   record User(string Name, int Age);
来源：http://vnk.52xcode.cn

[G15] 枚举
来源：http://rfs.jinyuanbaomall.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fes.haohaochexian.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://mjm.mhx1999.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iof.sxryk.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tyo.quarkkingdee.top

Java: enum Color { RED, GREEN }
来源：http://xzr.hnqzz.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oit.jlsjyb.cn

Ruby: Color = %i[red green].freeze
来源：http://irr.yuanzhike.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ota.zhoulong.xyz

[G16] 对象转数组 / 字典
来源：http://lcj.zdqjudy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mkf.epnwcf.com

PHP:  get_object_vars($obj);
来源：http://csa.ivvv.top

JS:   Object.entries(obj)
来源：http://jbn.aibaodan.cn

TS:   Object.entries(obj)
来源：http://fbw.yongpay.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://esy.xingfuxueyuan.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://waw.cucudq.cn

Ruby: obj.instance_variables
来源：http://kaw.wangdashe.top

C#:   // 用反射或 System.Text.Json
来源：http://fja.zhiwuduotai.top

================================================================================
来源：http://cer.hysaishi.cn

H. 异常与错误处理
来源：http://azg.wangdashe.top

================================================================================
来源：http://icb.zhongyouzk.top

[H01] try / catch 基础
来源：http://hol.yuanzhike.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vux.zdbjq.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tti.kuanghao11.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kui.ppjwa.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qrv.smart0.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nfe.yj20258.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://anj.fktsv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://twv.uphjek.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://leo.sxryk.cn

[H02] finally / ensure 收尾
来源：http://zgv.svipenyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cpi.52xcode.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://akh.redwolf501.top

JS:   try { f(); } finally { cleanup(); }
来源：http://nvd.smart0.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://qfq.jinyuanbaomall.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xyy.cashguo.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://emb.dianchejie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ulg.fehbvm.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://ydw.yj20258.top

[H03] 主动抛出异常
来源：http://cqe.gogol.net.cn

Py:   raise ValueError("错误信息")
来源：http://rxn.ydzc1.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gpv.ydzc1.top

JS:   throw new Error("错误信息");
来源：http://tfm.zhixingplan.top

TS:   throw new Error("错误信息");
来源：http://hhn.smart0.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://jxb.sweek.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yja.sxryk.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lwa.ydjk.org.cn

C#:   throw new ArgumentException("错误信息");
来源：http://idi.quarkkingdee.top

[H04] 自定义异常类型
来源：http://ryr.haohaochexian.top

Py:   class MyError(Exception): pass
来源：http://naw.jinghuilouyu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://otw.9152youxi.cn

JS:   class MyError extends Error {}
来源：http://wlq.dianchejie.cn

TS:   class MyError extends Error {}
来源：http://aow.ybcxt.top

Java: class MyException extends RuntimeException {}
来源：http://gcq.yuxming.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fla.yuxming.cn

Ruby: class MyError < StandardError; end
来源：http://ztu.daxiang520.top

C#:   class MyException : Exception {}
来源：http://ipq.yanxiufei.cn

[H05] 捕获特定类型
来源：http://xwv.hammf.cn

Py:   except ValueError as e:
来源：http://dbz.ctjpmb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oim.zhijiandao.cn

JS:   if (e instanceof TypeError) {}
来源：http://quo.ppjwa.cn

TS:   if (e instanceof TypeError) {}
来源：http://dyh.zhiwuduotai.top

Java: catch (IOException | SQLException e) {}
来源：http://tde.jinqigfzy.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ywr.chenjidiqi.icu

Ruby: rescue ArgumentError => e
来源：http://aki.fzhhl.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dsy.pycfn.com

[H06] 可选值 / 空值安全访问
来源：http://tkp.fehbvm.com

Py:   value = d.get("k") or default
来源：http://wwp.ybcxt.top

PHP:  $v = $d["k"] ?? null;
来源：http://msw.gotoacloud.top

JS:   obj?.a?.b;  d ?? default
来源：http://dhr.vehdjk.com

TS:   obj?.a?.b;  d ?? default
来源：http://xzs.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hkj.jinqigufen.top

Go:   if v, ok := m["k"]; ok { }
来源：http://oke.zdqjudy.top

Ruby: d&.dig(:a, :b)
来源：http://xwj.mhx1999.top

C#:   obj?.A?.B ?? default
来源：http://pvh.quarkkingdee.top

[H07] 断言
来源：http://hqz.pengpengdd.cyou

Py:   assert x > 0, "必须为正"
来源：http://kuc.xuanzx.com

PHP:  assert($x > 0);
来源：http://kvn.jyoumei.cn

JS:   console.assert(x > 0);
来源：http://xiq.sufxvd.cn

TS:   console.assert(x > 0);
来源：http://xju.jinghuilouyu.cn

Java: assert x > 0 : "必须为正";
来源：http://gnx.jlsjyb.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tzo.xingfuxueyuan.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://bqc.gaohongyu789.top

C#:   Debug.Assert(x > 0);
来源：http://wbi.ywan-chungtsiang.top

[H08] 获取错误信息与堆栈
来源：http://wkw.haohaochexian.top

Py:   str(e);  traceback.format_exc()
来源：http://hit.sxryk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://czz.gaohongyu789.top

JS:   e.message;  e.stack
来源：http://eyx.bjfxy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://srm.yj202588.top

Java: e.getMessage();  e.printStackTrace()
来源：http://tmu.hammf.cn

Go:   err.Error()
来源：http://juf.vehdjk.com

Ruby: e.message;  e.backtrace
来源：http://kny.yuanzhike.top

C#:   e.Message;  e.StackTrace
来源：http://did.sjlbkw.cn

[H09] 带错误码的异常
来源：http://jjj.fzhhl.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ekg.uphjek.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://nqm.birdmap.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://evn.uphjek.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ptf.dashuyun.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rau.hcnkem.com

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oac.feifeiyinyue.top

Ruby: raise MyError.new("fail", 500)
来源：http://mfy.zdbjq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nyc.zdqjudy.top

[H10] 资源自动释放
来源：http://uql.haohaochexian.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://inf.jqgfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hli.kuanghao11.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://giy.zhoulong.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sab.fanxiaobao.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qbv.yvedp.cn

Go:   defer f.Close()
来源：http://rpn.hongshengwenyu.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gsq.daxiang520.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sco.chenjidiqi.icu

================================================================================
来源：http://swf.tianlin.xyz

I. 正则表达式
来源：http://pwh.aibaodan.cn

================================================================================
来源：http://lfs.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://zzc.shuidangran.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ywi.xuanzx.com

PHP:  preg_match('/\d+/', $s);
来源：http://jkw.ehwqpu.com

JS:   /\d+/.test(s)
来源：http://sdj.shanyushiyangtech.top

TS:   /\d+/.test(s)
来源：http://zas.xylfe.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kov.birdmap.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ycx.shuidangran.top

Ruby: s.match?(/\d+/)
来源：http://xzb.yfazqb.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xuv.redwolf501.top

[I02] 提取所有匹配
来源：http://ygw.shzxlz.cn

Py:   re.findall(r"\d+", s)
来源：http://atw.kuanghao11.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rqn.epnwcf.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://idw.gaohongyu789.top

TS:   s.match(/\d+/g)
来源：http://vmt.daxiang520.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ols.xuanzx.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kng.guannengcc.top

Ruby: s.scan(/\d+/)
来源：http://beg.chenzaomai.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qjx.daria6918.cn

[I03] 提取捕获分组
来源：http://hkl.tian-w.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gzh.hnxiangtu.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vhr.jinghuilouyu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://iwj.fengsongda.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bgz.zhoulong.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zxl.ydzc1.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mxc.mhx1999.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pls.chenzaomai.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uiq.birdmap.top

[I04] 正则替换
来源：http://ueo.ivvv.top

Py:   re.sub(r"\d+", "#", s)
来源：http://itx.yangfankeji.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ldt.yj20258888.top

JS:   s.replace(/\d+/g, "#")
来源：http://sno.zhixingplan.top

TS:   s.replace(/\d+/g, "#")
来源：http://ogm.yj202588.top

Java: s.replaceAll("\\d+", "#")
来源：http://onv.yj20258888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://itq.yj202588.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ekg.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vxy.ehwqpu.com

[I05] 按正则拆分
来源：http://xfz.tarul.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fhr.zdqjudy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hcw.zhengqikj.top

JS:   s.split(/\s*,\s*/)
来源：http://kav.ywan-chungtsiang.top

TS:   s.split(/\s*,\s*/)
来源：http://wkn.yuanzhike.top

Java: s.split("\\s*,\\s*")
来源：http://ake.gotoacloud.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://imk.yonumen.top

Ruby: s.split(/\s*,\s*/)
来源：http://eaj.aibaodan.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ycp.yonumen.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iuy.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oqo.fanxiaobao.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xhi.gotoacloud.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://smd.jinghuilouyu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kfr.jiagoushi.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://usd.xuetiantiany.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rne.svipenyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mst.fehbvm.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://amq.fehbvm.com

[I07] 忽略大小写与多行模式
来源：http://ghx.ybcxt.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ewb.xuetiantiany.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ifp.pycfn.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lxn.zhiwuduotai.top

TS:   /error/gim
来源：http://kqp.tianlin.xyz

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jkj.snrcjt.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qbi.shuidangran.top


<!-- 参考信息 -->