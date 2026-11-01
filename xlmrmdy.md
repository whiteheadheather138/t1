代发 wailian999

JS:   this.name = "x";
来源：http://3g.epnwcf.com/Article/details/gtzprriqi.sHtML

TS:   name: string = "x";
来源：http://read.share.yfazqb.com/Article/details/gjoxofruz.sHtML

Java: private String name;
来源：http://read.share.sjlbkw.cn/Article/details/gdjehmdrf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.yfazqb.com/Article/details/gtrlwfyie.sHtML

Ruby: @name = "x"
来源：http://m.share.yfazqb.com/Article/details/grzwipjyb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.tarul.cn/Article/details/gdttolutb.sHtML

[G04] 定义方法
来源：http://www.m.share.sjlbkw.cn/Article/details/gqwvcycgq.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.vehdjk.com/Article/details/gaghxjwnu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.vehdjk.com/Article/details/gbxqjlmio.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.epnwcf.com/Article/details/girhfflwx.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.tarul.cn/Article/details/gybnrwrth.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fktsv.cn/Article/details/gvzndlbzh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.epnwcf.com/Article/details/grkrrtwad.sHtML

Ruby: def greet; @name; end
来源：http://www.share.tarul.cn/Article/details/gssccfdcz.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.yfazqb.com/Article/details/glzofotxt.sHtML

[G05] 继承
来源：http://read.share.fktsv.cn/Article/details/gnbbhltcl.sHtML

Py:   class Admin(User): pass
来源：http://baike.fktsv.cn/Article/details/gkeudtajp.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.bbcook.cn/Article/details/gibttglnz.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fktsv.cn/Article/details/gzngoaatd.sHtML

TS:   class Admin extends User {}
来源：http://blog.epnwcf.com/Article/details/giyzssibc.sHtML

Java: class Admin extends User {}
来源：http://mobile.epnwcf.com/Article/details/gahyyuhbd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fktsv.cn/Article/details/gsvlmkytf.sHtML

Ruby: class Admin < User; end
来源：http://wap.yfazqb.com/Article/details/grpoxopet.sHtML

C#:   class Admin : User {}
来源：http://3g.fktsv.cn/Article/details/gqgiyrqsc.sHtML

[G06] 重写方法
来源：http://baike.bbcook.cn/Article/details/ghspbejmf.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.bbcook.cn/Article/details/givjnwvjv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.epnwcf.com/Article/details/gsftoxtpf.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.epnwcf.com/Article/details/grxdamquz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.tarul.cn/Article/details/gzpsahqob.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.epnwcf.com/Article/details/geewrbomz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.epnwcf.com/Article/details/gkisctzaw.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.epnwcf.com/Article/details/gjicgryns.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.vehdjk.com/Article/details/grwbzoham.sHtML

[G07] 调用父类方法
来源：http://blog.sjlbkw.cn/Article/details/giqazhkqq.sHtML

Py:   super().greet()
来源：http://baike.vehdjk.com/Article/details/gobabbqew.sHtML

PHP:  parent::greet();
来源：http://blog.epnwcf.com/Article/details/gcettfzap.sHtML

JS:   super.greet();
来源：http://www.blog.yfazqb.com/Article/details/gmazttiit.sHtML

TS:   super.greet();
来源：http://mobile.epnwcf.com/Article/details/gaqebwlip.sHtML

Java: super.greet();
来源：http://mobile.vehdjk.com/Article/details/gyazpyxyd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.yfazqb.com/Article/details/gzssmmdhb.sHtML

Ruby: super
来源：http://m.share.fktsv.cn/Article/details/gjvqcwtru.sHtML

C#:   base.Greet();
来源：http://3g.sjlbkw.cn/Article/details/gdupkynua.sHtML

[G08] 静态方法与属性
来源：http://mobile.sjlbkw.cn/Article/details/glbbzdkem.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.yfazqb.com/Article/details/gksaleoaw.sHtML

PHP:  public static function f() {}
来源：http://wap.sjlbkw.cn/Article/details/gobztzqql.sHtML

JS:   static f() {}
来源：http://m.share.bbcook.cn/Article/details/gvcarrkcd.sHtML

TS:   static f(): void {}
来源：http://mobile.yfazqb.com/Article/details/guydcxkkz.sHtML

Java: static void f() {}
来源：http://blog.sjlbkw.cn/Article/details/gddknjdfq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.yfazqb.com/Article/details/gedepolff.sHtML

Ruby: def self.f; end
来源：http://blog.yfazqb.com/Article/details/gojxmrsov.sHtML

C#:   public static void F() {}
来源：http://read.share.bbcook.cn/Article/details/ggmfpydqb.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fktsv.cn/Article/details/gpozgrilr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.epnwcf.com/Article/details/gtayfzxji.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.sjlbkw.cn/Article/details/gddkeakwm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.yfazqb.com/Article/details/gitkhrywl.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.vehdjk.com/Article/details/gmduvapsi.sHtML

Java: interface Shape { double area(); }
来源：http://baike.yfazqb.com/Article/details/gepxmgvhn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.vehdjk.com/Article/details/gdjrxoqdy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.vehdjk.com/Article/details/ghvwjnvxy.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.bbcook.cn/Article/details/gghcpyyss.sHtML

[G10] 访问控制
来源：http://www.blog.tarul.cn/Article/details/giuwrztdt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.tarul.cn/Article/details/gwgrrcafu.sHtML

PHP:  public / protected / private
来源：http://m.share.yfazqb.com/Article/details/gwvgsmozu.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.sjlbkw.cn/Article/details/ggiptwyxc.sHtML

TS:   public / protected / private
来源：http://read.share.yfazqb.com/Article/details/gixzknapr.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.tarul.cn/Article/details/gythtewlh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.yfazqb.com/Article/details/gekzdhorz.sHtML

Ruby: public / protected / private
来源：http://www.share.epnwcf.com/Article/details/gbulqukic.sHtML

C#:   public / protected / private / internal
来源：http://baike.vehdjk.com/Article/details/gqkrmovda.sHtML

[G11] getter / setter
来源：http://www.share.bbcook.cn/Article/details/gojsrxgut.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.epnwcf.com/Article/details/grfvepuxe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fktsv.cn/Article/details/gkcumvszs.sHtML

JS:   get name() { return this._name; }
来源：http://wap.vehdjk.com/Article/details/gyjkbmaox.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fktsv.cn/Article/details/gxyivxwhl.sHtML

Java: public String getName() { return name; }
来源：http://blog.fktsv.cn/Article/details/gitnkbvwd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.yfazqb.com/Article/details/gqbaiemvf.sHtML

Ruby: attr_accessor :name
来源：http://wap.sjlbkw.cn/Article/details/gnqraqxud.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.vehdjk.com/Article/details/gxfuxbsrn.sHtML

[G12] 对象转字符串
来源：http://mobile.vehdjk.com/Article/details/gjftablfr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.tarul.cn/Article/details/gadgvofio.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.vehdjk.com/Article/details/gmugwjbee.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.bbcook.cn/Article/details/gaepowruf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.bbcook.cn/Article/details/gmuvblrse.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.bbcook.cn/Article/details/gfeusshyw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.yfazqb.com/Article/details/gcyuwgggh.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.vehdjk.com/Article/details/gavxxvaws.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.epnwcf.com/Article/details/gezjdyusw.sHtML

[G13] 判断对象类型
来源：http://baike.yfazqb.com/Article/details/gxmprbvrr.sHtML

Py:   isinstance(u, User)
来源：http://www.share.epnwcf.com/Article/details/gyfnnyofe.sHtML

PHP:  $u instanceof User
来源：http://mobile.tarul.cn/Article/details/gfjhrtxmr.sHtML

JS:   u instanceof User
来源：http://wap.vehdjk.com/Article/details/grajkcsku.sHtML

TS:   u instanceof User
来源：http://3g.yfazqb.com/Article/details/gbtshymvl.sHtML

Java: u instanceof User
来源：http://3g.sjlbkw.cn/Article/details/gmvsjlzwr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.yfazqb.com/Article/details/grobwvaeg.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.vehdjk.com/Article/details/gigvkxutj.sHtML

C#:   u is User
来源：http://3g.yfazqb.com/Article/details/gnvawfitz.sHtML

[G14] 数据类 / record
来源：http://blog.fktsv.cn/Article/details/gazfoipem.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.sjlbkw.cn/Article/details/gwbtsfnkb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.sjlbkw.cn/Article/details/gtkycncpj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.bbcook.cn/Article/details/gzgbzmlss.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fktsv.cn/Article/details/gcproimhc.sHtML

Java: record User(String name, int age) {}
来源：http://baike.yfazqb.com/Article/details/gostzcics.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.vehdjk.com/Article/details/gmnvcgyus.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fktsv.cn/Article/details/gocrwmcyq.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.tarul.cn/Article/details/gbbhzyfnq.sHtML

[G15] 枚举
来源：http://m.share.sjlbkw.cn/Article/details/gfqjpyysb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.yfazqb.com/Article/details/geueewhoe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.tarul.cn/Article/details/gcmeqmxpx.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.sjlbkw.cn/Article/details/gldufkqfm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.epnwcf.com/Article/details/gjfgugnyh.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.epnwcf.com/Article/details/gcrxzxxbg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.sjlbkw.cn/Article/details/gkumowkmp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.yfazqb.com/Article/details/guugzoaao.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.epnwcf.com/Article/details/gdiqarczn.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.tarul.cn/Article/details/gcwlrkbhx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.sjlbkw.cn/Article/details/gthwoclgt.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.yfazqb.com/Article/details/gtlfncomc.sHtML

JS:   Object.entries(obj)
来源：http://baike.sjlbkw.cn/Article/details/goloxluux.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.vehdjk.com/Article/details/gocfdnmvu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.bbcook.cn/Article/details/gddyelicu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.yfazqb.com/Article/details/gpyqlpkyl.sHtML

Ruby: obj.instance_variables
来源：http://baike.epnwcf.com/Article/details/gmurdrqkg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.sjlbkw.cn/Article/details/gwbviidma.sHtML

================================================================================
来源：http://wap.sjlbkw.cn/Article/details/ghiopvgka.sHtML

H. 异常与错误处理
来源：http://blog.vehdjk.com/Article/details/glwkrmsgd.sHtML

================================================================================
来源：http://blog.yfazqb.com/Article/details/giwycpvhc.sHtML

[H01] try / catch 基础
来源：http://wap.vehdjk.com/Article/details/gtblgkkji.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.vehdjk.com/Article/details/gnafspyao.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.sjlbkw.cn/Article/details/gvukxfqrl.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.yfazqb.com/Article/details/gxvppcgkd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.bbcook.cn/Article/details/gucaduvgl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.sjlbkw.cn/Article/details/gywuzbgld.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fktsv.cn/Article/details/gjehozlow.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.tarul.cn/Article/details/gzaxqvbhf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.tarul.cn/Article/details/gxmyhgdrr.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.yfazqb.com/Article/details/glnjihnoe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.sjlbkw.cn/Article/details/gevxmwuml.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.epnwcf.com/Article/details/gzzxtstzo.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.epnwcf.com/Article/details/gdobxjldt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.yfazqb.com/Article/details/gvkqqepez.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.epnwcf.com/Article/details/gbsifexpj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.yfazqb.com/Article/details/gexhnfqmo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fktsv.cn/Article/details/gnefntvif.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.sjlbkw.cn/Article/details/gwwpscxid.sHtML

[H03] 主动抛出异常
来源：http://www.share.vehdjk.com/Article/details/gwbmpxsvi.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.sjlbkw.cn/Article/details/gchpgshcj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.epnwcf.com/Article/details/ghlyrlqsm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.tarul.cn/Article/details/glkflrgwp.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.bbcook.cn/Article/details/gypmkbnre.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.epnwcf.com/Article/details/gfskflikb.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.yfazqb.com/Article/details/giqduwdcy.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.yfazqb.com/Article/details/gyecvyhsh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.tarul.cn/Article/details/gcgtovhzd.sHtML

[H04] 自定义异常类型
来源：http://baike.epnwcf.com/Article/details/gecramsco.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.epnwcf.com/Article/details/geelvehgi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.sjlbkw.cn/Article/details/gqefclhoq.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.epnwcf.com/Article/details/gbvtmnptw.sHtML

TS:   class MyError extends Error {}
来源：http://wap.sjlbkw.cn/Article/details/gcskrygpt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.bbcook.cn/Article/details/gozghrscn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.vehdjk.com/Article/details/gqsjugqnv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.tarul.cn/Article/details/gwgzyysym.sHtML

C#:   class MyException : Exception {}
来源：http://wap.tarul.cn/Article/details/ggscugrdc.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.vehdjk.com/Article/details/gqqtlnyvc.sHtML

Py:   except ValueError as e:
来源：http://blog.sjlbkw.cn/Article/details/gobxbszox.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.vehdjk.com/Article/details/gycmhvdne.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.tarul.cn/Article/details/gcdgkwlhh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fktsv.cn/Article/details/gmxvfgzyy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.sjlbkw.cn/Article/details/gejpbngkk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.vehdjk.com/Article/details/gbwoyftis.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.bbcook.cn/Article/details/gsyxfmrif.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.vehdjk.com/Article/details/gyprppjpv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.bbcook.cn/Article/details/gdojajlyk.sHtML

Py:   value = d.get("k") or default
来源：http://blog.sjlbkw.cn/Article/details/ghwjcwdoq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.tarul.cn/Article/details/glivvozxg.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.tarul.cn/Article/details/gegmuzuxf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.epnwcf.com/Article/details/gsexnfykt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fktsv.cn/Article/details/gcqqxkwgr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.bbcook.cn/Article/details/gywamrbsj.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.vehdjk.com/Article/details/ggqdasxfv.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.sjlbkw.cn/Article/details/grvwudtlt.sHtML

[H07] 断言
来源：http://mobile.sjlbkw.cn/Article/details/gnazbelnh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fktsv.cn/Article/details/gfvfzkduq.sHtML

PHP:  assert($x > 0);
来源：http://m.share.vehdjk.com/Article/details/gzfizvqkh.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.vehdjk.com/Article/details/ghlevxgtj.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.epnwcf.com/Article/details/gekumqjxt.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.bbcook.cn/Article/details/gnuhlpiqb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fktsv.cn/Article/details/gxuxgpztb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.epnwcf.com/Article/details/gipxgaeie.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.tarul.cn/Article/details/gmzxhdvjk.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.bbcook.cn/Article/details/gpolljwpo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fktsv.cn/Article/details/gciakrswg.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.sjlbkw.cn/Article/details/gbkkapeyv.sHtML

JS:   e.message;  e.stack
来源：http://wap.epnwcf.com/Article/details/grtuycnut.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fktsv.cn/Article/details/gdtgvbdtf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.sjlbkw.cn/Article/details/grazxavml.sHtML

Go:   err.Error()
来源：http://3g.tarul.cn/Article/details/gpqmhumxg.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.bbcook.cn/Article/details/gapexrcpm.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.sjlbkw.cn/Article/details/gpnadysba.sHtML

[H09] 带错误码的异常
来源：http://m.share.vehdjk.com/Article/details/gamsazxsi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.epnwcf.com/Article/details/ghgheqijs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.tarul.cn/Article/details/gjvqjbmtr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.sjlbkw.cn/Article/details/gegcaatvp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://read.share.yfazqb.com/Article/details/gjxplhctq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.vehdjk.com/Article/details/gajpiidgn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.bbcook.cn/Article/details/gpdwlzbcq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.fktsv.cn/Article/details/gbasfdcpn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.vehdjk.com/Article/details/gqiizekli.sHtML

[H10] 资源自动释放
来源：http://www.m.share.tarul.cn/Article/details/gjannvbmu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.yfazqb.com/Article/details/gimrbobwh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.tarul.cn/Article/details/gsuanmtay.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.sjlbkw.cn/Article/details/ghhbpqowd.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.vehdjk.com/Article/details/gojkittvc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.sjlbkw.cn/Article/details/ggpzcujzw.sHtML

Go:   defer f.Close()
来源：http://www.share.fktsv.cn/Article/details/gmkvlbcoj.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.tarul.cn/Article/details/ggbnzznre.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.fktsv.cn/Article/details/gxdhrsrjw.sHtML

================================================================================
来源：http://wap.epnwcf.com/Article/details/gzfjsysse.sHtML

I. 正则表达式
来源：http://mobile.epnwcf.com/Article/details/glvjyopsc.sHtML

================================================================================
来源：http://baike.yfazqb.com/Article/details/ggicgduxs.sHtML

[I01] 判断是否匹配
来源：http://www.blog.yfazqb.com/Article/details/gywafgqpp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.sjlbkw.cn/Article/details/gumxshvug.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.bbcook.cn/Article/details/gsksfghtp.sHtML

JS:   /\d+/.test(s)
来源：http://blog.yfazqb.com/Article/details/gbugqigjd.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fktsv.cn/Article/details/goxxfuntg.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.sjlbkw.cn/Article/details/gtlqqmvmg.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.vehdjk.com/Article/details/gtmixieif.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.yfazqb.com/Article/details/gmwbzjxks.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.tarul.cn/Article/details/gfdegygfg.sHtML

[I02] 提取所有匹配
来源：http://mobile.fktsv.cn/Article/details/gtddchnou.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.yfazqb.com/Article/details/gvqqynomz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.epnwcf.com/Article/details/gtzzskawm.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.sjlbkw.cn/Article/details/guhyvvfln.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.yfazqb.com/Article/details/gpjgnmicn.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.bbcook.cn/Article/details/giyflerpi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.yfazqb.com/Article/details/gdxncdind.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.bbcook.cn/Article/details/gzzjeoxax.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.yfazqb.com/Article/details/gorpqhetk.sHtML

[I03] 提取捕获分组
来源：http://3g.epnwcf.com/Article/details/gacbuajkx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.bbcook.cn/Article/details/gyvkgwjiv.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.tarul.cn/Article/details/guffnprsx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.sjlbkw.cn/Article/details/gqzniiwar.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.tarul.cn/Article/details/gfoosuxng.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.bbcook.cn/Article/details/gmncibrzg.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.yfazqb.com/Article/details/glarreusn.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.fktsv.cn/Article/details/gbjdjncbb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.bbcook.cn/Article/details/gxyoofbfh.sHtML

[I04] 正则替换
来源：http://www.m.share.vehdjk.com/Article/details/gvatqpusy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.yfazqb.com/Article/details/gzvrfrwlm.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://read.share.bbcook.cn/Article/details/gypjtsztd.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.fktsv.cn/Article/details/gujuohypa.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.yfazqb.com/Article/details/ganhhzarn.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.sjlbkw.cn/Article/details/ggjptmumu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.fktsv.cn/Article/details/gdwqkzbkj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.bbcook.cn/Article/details/givpwrsdd.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://read.share.bbcook.cn/Article/details/gllrlpdid.sHtML

[I05] 按正则拆分
来源：http://mobile.sjlbkw.cn/Article/details/glphzqeqy.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.tarul.cn/Article/details/gdtzjdocp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.vehdjk.com/Article/details/grkgwqddu.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.yfazqb.com/Article/details/gcuhwsqob.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.epnwcf.com/Article/details/gbyplikgu.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.share.bbcook.cn/Article/details/gkqlguhgv.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.epnwcf.com/Article/details/ggxsulndr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://wap.tarul.cn/Article/details/gksvsztgc.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.yfazqb.com/Article/details/giejpukpu.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://blog.vehdjk.com/Article/details/gjuxwusvl.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://blog.tarul.cn/Article/details/gklgvjswf.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.sjlbkw.cn/Article/details/gaplljshw.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.sjlbkw.cn/Article/details/gqbmdwmtg.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.yfazqb.com/Article/details/gpainspqv.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.yfazqb.com/Article/details/ggwgznqmw.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.sjlbkw.cn/Article/details/gvsqkjvll.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.fktsv.cn/Article/details/gdnzrzcbe.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://3g.tarul.cn/Article/details/gptwsjdyh.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.yfazqb.com/Article/details/gieokjcph.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.bbcook.cn/Article/details/gcwecvbzn.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.vehdjk.com/Article/details/gvkyqioge.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.sjlbkw.cn/Article/details/gvcyomynl.sHtML

TS:   /error/gim
来源：http://3g.fktsv.cn/Article/details/gtxigacam.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.vehdjk.com/Article/details/gkoqubchy.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.sjlbkw.cn/Article/details/gqvvhgpqn.sHtML

Ruby: s.scan(/error/i)
来源：http://wap.vehdjk.com/Article/details/ggmaslxng.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.m.share.fktsv.cn/Article/details/gykxdiuxb.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.fktsv.cn/Article/details/gvtfkcsnu.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://m.share.bbcook.cn/Article/details/glbyyyslv.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.yfazqb.com/Article/details/ggukymcte.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.epnwcf.com/Article/details/glfvrcpfk.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://baike.vehdjk.com/Article/details/gsovcvlvp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.share.vehdjk.com/Article/details/gstraajdy.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wap.tarul.cn/Article/details/gvxcoinpq.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://baike.epnwcf.com/Article/details/gnioqcwfi.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.epnwcf.com/Article/details/gfpzhsjmx.sHtML

================================================================================
来源：http://m.share.sjlbkw.cn/Article/details/gaaflsbkz.sHtML

J. 日期与时间
来源：http://mobile.epnwcf.com/Article/details/gggsodtms.sHtML

================================================================================
来源：http://3g.tarul.cn/Article/details/gvtonvsip.sHtML

[J01] 获取当前时间
来源：http://wap.epnwcf.com/Article/details/gczckgtsk.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.fktsv.cn/Article/details/gjkxhnpad.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://3g.vehdjk.com/Article/details/gtkcdsmyi.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.sjlbkw.cn/Article/details/ggswzxgzm.sHtML

TS:   new Date();  Date.now()
来源：http://blog.fktsv.cn/Article/details/gkqsahjqe.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.yfazqb.com/Article/details/gybifrrdi.sHtML


<!-- 参考信息 -->