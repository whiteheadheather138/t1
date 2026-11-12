代发 wailian999

TS:   constructor(public name: string) {}
来源：http://aen.zycfv.cn

Java: User(String name) { this.name = name; }
来源：http://req.yj20258.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://utu.andypj.xyz

Ruby: def initialize(name); @name = name; end
来源：http://ndu.hongshengwenyu.top

C#:   public User(string name) { Name = name; }
来源：http://ynp.bjfxy.top

[G03] 实例属性
来源：http://brn.hfpthk.cn

Py:   self.name = "x"
来源：http://ppm.hammf.cn

PHP:  public string $name = "x";
来源：http://bxn.snrcjt.cn

JS:   this.name = "x";
来源：http://vlc.snrcjt.cn

TS:   name: string = "x";
来源：http://uyx.xuetiantiany.cn

Java: private String name;
来源：http://bvd.ehwqpu.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://url.chenzaomai.com

Ruby: @name = "x"
来源：http://gny.aizwys.cn

C#:   public string Name { get; set; } = "x";
来源：http://wtf.cucudq.cn

[G04] 定义方法
来源：http://wnq.xziqi.cn

Py:   def greet(self): return self.name
来源：http://ucj.aizwys.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pmc.gaohongyu789.top

JS:   greet() { return this.name; }
来源：http://cws.zhoulong.xyz

TS:   greet(): string { return this.name; }
来源：http://fzw.pycfn.com

Java: String greet() { return name; }
来源：http://zav.xinyue.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://pnf.tanke756.top

Ruby: def greet; @name; end
来源：http://pjb.yonumen.top

C#:   public string Greet() => Name;
来源：http://dzi.yj20258888.top

[G05] 继承
来源：http://psx.52xcode.cn

Py:   class Admin(User): pass
来源：http://eeq.zhongyouzk.top

PHP:  class Admin extends User {}
来源：http://otk.jqgfzy.top

JS:   class Admin extends User {}
来源：http://dlq.hnxiangtu.top

TS:   class Admin extends User {}
来源：http://ahz.wangdashe.top

Java: class Admin extends User {}
来源：http://xzj.vehdjk.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ujj.wangdashe.top

Ruby: class Admin < User; end
来源：http://ziz.jinqigufen.top

C#:   class Admin : User {}
来源：http://exf.tian-w.cn

[G06] 重写方法
来源：http://ruj.shuidangran.top

Py:   def greet(self): return "admin"
来源：http://qbe.hesvh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://uvr.hesvh.cn

JS:   greet() { return "admin"; }
来源：http://qkh.xziqi.cn

TS:   greet(): string { return "admin"; }
来源：http://osv.aibaodan.cn

Java: @Override String greet() { return "admin"; }
来源：http://xnx.shanyushiyangtech.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sfy.aibaodan.cn

Ruby: def greet; "admin"; end
来源：http://xse.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://kdg.hysaishi.cn

[G07] 调用父类方法
来源：http://rze.ctjpmb.com

Py:   super().greet()
来源：http://hcm.hysaishi.cn

PHP:  parent::greet();
来源：http://fue.fzhhl.top

JS:   super.greet();
来源：http://ewf.cheryme.top

TS:   super.greet();
来源：http://gse.9152youxi.cn

Java: super.greet();
来源：http://bvf.nwbrower.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dtm.mhx1999.top

Ruby: super
来源：http://mut.feifeiyinyue.top

C#:   base.Greet();
来源：http://pjk.nanxinkj.top

[G08] 静态方法与属性
来源：http://zfb.zhiwuduotai.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lib.jinqigfzy.top

PHP:  public static function f() {}
来源：http://tpc.svipenyu.cn

JS:   static f() {}
来源：http://rzt.hysaishi.cn

TS:   static f(): void {}
来源：http://clp.daria6918.cn

Java: static void f() {}
来源：http://yri.nanxinkj.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://nes.cqqwz.cn

Ruby: def self.f; end
来源：http://ibo.ydzc1.top

C#:   public static void F() {}
来源：http://fse.shanyushiyangkeji.top

[G09] 接口 / 抽象类
来源：http://ang.cheryme.top

Py:   from abc import ABC, abstractmethod
来源：http://rye.yueranfly.top

PHP:  interface Shape { public function area(): float; }
来源：http://kdn.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://klw.shangyingyoupin.top

TS:   interface Shape { area(): number; }
来源：http://etd.gaohongyu789.top

Java: interface Shape { double area(); }
来源：http://elz.xingfuxueyuan.xyz

Go:   type Shape interface { Area() float64 }
来源：http://dxi.wangshuangyany.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ibh.yfazqb.com

C#:   interface IShape { double Area(); }
来源：http://bct.zycfv.cn

[G10] 访问控制
来源：http://tnr.fehbvm.com

Py:   约定 _protected / __private（不强制）
来源：http://dbi.yangfankeji.com

PHP:  public / protected / private
来源：http://czg.hysaishi.cn

JS:   #private 字段；其余公开
来源：http://dja.cucudq.cn

TS:   public / protected / private
来源：http://phb.guowangkeji.top

Java: public / protected / private / 默认包级
来源：http://kgm.fehbvm.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://zej.snrcjt.cn

Ruby: public / protected / private
来源：http://hvs.zdbjq.cn

C#:   public / protected / private / internal
来源：http://oga.fengsongda.top

[G11] getter / setter
来源：http://qgo.guowangkeji.top

Py:   @property 与 @x.setter
来源：http://nbp.hesvh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sad.jqgfzy.top

JS:   get name() { return this._name; }
来源：http://bcb.dashuyun.cn

TS:   get name(): string { return this._name; }
来源：http://imh.jinqigfzy.top

Java: public String getName() { return name; }
来源：http://yrk.vehdjk.com

Go:   func (u User) GetName() string { return u.Name }
来源：http://qhs.havefunace.top

Ruby: attr_accessor :name
来源：http://zvk.yangfankeji.com

C#:   public string Name { get; set; }
来源：http://jlv.birdmap.top

[G12] 对象转字符串
来源：http://lve.zdbjq.cn

Py:   def __str__(self): return self.name
来源：http://pqf.mhx1999.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://xby.snrcjt.cn

JS:   toString() { return this.name; }
来源：http://qxd.jqgfzy.top

TS:   toString(): string { return this.name; }
来源：http://drc.ybcxt.top

Java: @Override public String toString() { return name; }
来源：http://bjp.nwbrower.top

Go:   func (u User) String() string { return u.Name }
来源：http://jyp.fktsv.cn

Ruby: def to_s; @name; end
来源：http://qyz.sxryk.cn

C#:   public override string ToString() => Name;
来源：http://bsl.yonumen.top

[G13] 判断对象类型
来源：http://uwz.ybcxt.top

Py:   isinstance(u, User)
来源：http://zcq.chenlongwang.top

PHP:  $u instanceof User
来源：http://zeg.fengsongda.top

JS:   u instanceof User
来源：http://qtn.daria6918.cn

TS:   u instanceof User
来源：http://mgf.xylfe.cn

Java: u instanceof User
来源：http://ack.xingfuxueyuan.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://ani.xuetiantiany.cn

Ruby: u.is_a?(User)
来源：http://jrw.xinyue.icu

C#:   u is User
来源：http://fca.jqgfzy.top

[G14] 数据类 / record
来源：http://thv.hcnkem.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fsd.jinqigufen.top

PHP:  // 用 readonly 属性模拟
来源：http://orh.ppjwa.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wbo.hnxiangtu.top

TS:   type User = { name: string; age: number };
来源：http://wuy.ppjwa.cn

Java: record User(String name, int age) {}
来源：http://lrk.zhaomingkeji.xyz

Go:   type User struct { Name string; Age int }
来源：http://bnh.wangshuangyany.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qzl.bbcook.cn

C#:   record User(string Name, int Age);
来源：http://hwv.fengsongda.top

[G15] 枚举
来源：http://ngg.hfpthk.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ott.yj202588.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://hys.gogol.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hcd.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://axz.yonumen.top

Java: enum Color { RED, GREEN }
来源：http://div.nanxinkj.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aon.hcnkem.com

Ruby: Color = %i[red green].freeze
来源：http://ite.snrcjt.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://osb.hesvh.cn

[G16] 对象转数组 / 字典
来源：http://mbr.haohaochexian.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jam.fanxiaobao.xyz

PHP:  get_object_vars($obj);
来源：http://lpm.aizwys.cn

JS:   Object.entries(obj)
来源：http://svc.snrcjt.cn

TS:   Object.entries(obj)
来源：http://mqe.jinyuanbaomall.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nwg.gaohongyu789.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://sra.bbcook.cn

Ruby: obj.instance_variables
来源：http://agh.yj20258.top

C#:   // 用反射或 System.Text.Json
来源：http://wim.snrcjt.cn

================================================================================
来源：http://qjn.cdnleiting.top

H. 异常与错误处理
来源：http://hre.meibo888.top

================================================================================
来源：http://oqy.wangdashe.top

[H01] try / catch 基础
来源：http://lwh.yuxming.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iwh.chenjidiqi.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nca.hesvh.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lvd.ivvv.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lmt.iojbl.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ael.yvedp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gqq.meibo888.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ngd.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qfd.vqdsnc.cn

[H02] finally / ensure 收尾
来源：http://vmo.chenzaomai.com

Py:   try: f()⏎finally: cleanup()
来源：http://iew.xingfuxueyuan.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://ola.sysykeji.top

JS:   try { f(); } finally { cleanup(); }
来源：http://glk.xingfuxueyuan.xyz

TS:   try { f(); } finally { cleanup(); }
来源：http://umv.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mtm.redwolf501.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://gmg.chenjidiqi.icu

Ruby: begin; f; ensure; cleanup; end
来源：http://tdd.ydzc1.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://zpw.ppjwa.cn

[H03] 主动抛出异常
来源：http://unk.ppjwa.cn

Py:   raise ValueError("错误信息")
来源：http://tlw.nanxinkj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://igw.redwolf501.top

JS:   throw new Error("错误信息");
来源：http://bvy.tian-w.cn

TS:   throw new Error("错误信息");
来源：http://xly.hywenlv.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://umo.jinyuanbaomall.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://etl.smart0.xyz

Ruby: raise ArgumentError, "错误信息"
来源：http://cze.snrcjt.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hlv.hcnkem.com

[H04] 自定义异常类型
来源：http://trd.zhijiandao.cn

Py:   class MyError(Exception): pass
来源：http://npp.xingfuxueyuan.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://pcy.xziqi.cn

JS:   class MyError extends Error {}
来源：http://vpa.yangfankeji.com

TS:   class MyError extends Error {}
来源：http://xij.yj202588.top

Java: class MyException extends RuntimeException {}
来源：http://eov.shangyingyoupin.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yxs.jinqigfzy.top

Ruby: class MyError < StandardError; end
来源：http://tui.pycfn.com

C#:   class MyException : Exception {}
来源：http://amk.svipenyu.cn

[H05] 捕获特定类型
来源：http://gzd.cdnleiting.top

Py:   except ValueError as e:
来源：http://usb.zycfv.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lqv.chenjidiqi.icu

JS:   if (e instanceof TypeError) {}
来源：http://dsx.chenlongwang.top

TS:   if (e instanceof TypeError) {}
来源：http://rha.yj202588.top

Java: catch (IOException | SQLException e) {}
来源：http://lon.pycfn.com

Go:   errors.Is(err, os.ErrNotExist)
来源：http://thf.aibaodan.cn

Ruby: rescue ArgumentError => e
来源：http://qmt.c1oappe.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bwz.svipenyu.cn

[H06] 可选值 / 空值安全访问
来源：http://ifg.mhx1999.top

Py:   value = d.get("k") or default
来源：http://bvb.nanxuanxn.top

PHP:  $v = $d["k"] ?? null;
来源：http://yzb.daria6918.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lvq.bjfxy.top

TS:   obj?.a?.b;  d ?? default
来源：http://ets.chenlongwang.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bhh.sufxvd.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uhw.chenzaomai.com

Ruby: d&.dig(:a, :b)
来源：http://nyc.yongpay.top

C#:   obj?.A?.B ?? default
来源：http://sxk.daria6918.cn

[H07] 断言
来源：http://ivy.jyoumei.cn

Py:   assert x > 0, "必须为正"
来源：http://hbn.yueranfly.top

PHP:  assert($x > 0);
来源：http://fix.gogol.net.cn

JS:   console.assert(x > 0);
来源：http://hfa.sjlbkw.cn

TS:   console.assert(x > 0);
来源：http://gml.shangyingyoupin.top

Java: assert x > 0 : "必须为正";
来源：http://etf.jiagoushi.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ovd.zycfv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ijl.sysykeji.top

C#:   Debug.Assert(x > 0);
来源：http://zct.svipenyu.cn

[H08] 获取错误信息与堆栈
来源：http://exy.fehbvm.com

Py:   str(e);  traceback.format_exc()
来源：http://cfg.nanxinkj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bec.c1oappe.top

JS:   e.message;  e.stack
来源：http://dyp.ywan-chungtsiang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://oun.9152youxi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ahd.tian-w.cn

Go:   err.Error()
来源：http://aed.hfpthk.cn

Ruby: e.message;  e.backtrace
来源：http://tct.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://nww.yanxiufei.cn

[H09] 带错误码的异常
来源：http://yxx.jinghuilouyu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jhn.dashuyun.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jft.ehwqpu.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vel.guowangkeji.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vbj.jqgufenzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nyx.tianlin.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sht.xuanzx.com

Ruby: raise MyError.new("fail", 500)
来源：http://dwl.hammf.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dzl.xziqi.cn

[H10] 资源自动释放
来源：http://gvf.mhx1999.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://fiv.mhx1999.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pwz.yvedp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sld.yuxming.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pho.zhiwuduotai.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gsc.c1oappe.top

Go:   defer f.Close()
来源：http://haq.hammf.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bvx.dianchejie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lsp.kuanghao11.cn

================================================================================
来源：http://jff.dashuyun.cn

I. 正则表达式
来源：http://ivl.wangdashe.top

================================================================================
来源：http://ewo.chenjidiqi.icu

[I01] 判断是否匹配
来源：http://ylp.fengsongda.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nnz.fzhhl.top

PHP:  preg_match('/\d+/', $s);
来源：http://twz.cdnleiting.top

JS:   /\d+/.test(s)
来源：http://ixt.jqgufenzy.top

TS:   /\d+/.test(s)
来源：http://juh.sufxvd.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jwh.birdmap.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nso.yfazqb.com

Ruby: s.match?(/\d+/)
来源：http://bkq.sysykeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ueb.meibo888.top

[I02] 提取所有匹配
来源：http://lgy.shanyushiyangtech.top

Py:   re.findall(r"\d+", s)
来源：http://lqm.dashuyun.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oes.jinghuilouyu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vzd.ppjwa.cn

TS:   s.match(/\d+/g)
来源：http://uxb.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ktf.tian-w.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dza.sjlbkw.cn

Ruby: s.scan(/\d+/)
来源：http://ijt.jinqigufen.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qak.jinghuilouyu.cn

[I03] 提取捕获分组
来源：http://gwt.meibo888.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qgb.gogol.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qkv.jqgfzy.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lvi.aibaodan.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xgb.zdbjq.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kja.gogol.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vyy.yangfankeji.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cyy.hammf.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ozw.yj20258.top

[I04] 正则替换
来源：http://mpc.ydjk.org.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wlo.hammf.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qgx.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rvf.mhx1999.top

TS:   s.replace(/\d+/g, "#")
来源：http://anf.ywan-chungtsiang.top

Java: s.replaceAll("\\d+", "#")
来源：http://vut.zhoulong.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://jul.jinghuilouyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sld.chenlongwang.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://icb.yonumen.top

[I05] 按正则拆分
来源：http://ujr.ydzc1.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tje.xingfuxueyuan.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oxc.mhx1999.top

JS:   s.split(/\s*,\s*/)
来源：http://ctz.shangyingyoupin.top

TS:   s.split(/\s*,\s*/)
来源：http://wfh.ivvv.top

Java: s.split("\\s*,\\s*")
来源：http://hih.dashuyun.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mmq.yonumen.top

Ruby: s.split(/\s*,\s*/)
来源：http://vgm.uphjek.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://owx.zhengqikj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lpu.nanxuanxn.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fpk.meibo888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vqz.yuanzhike.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://euv.fehbvm.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vfk.yuanzhike.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qiv.c1oappe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://srt.fanxiaobao.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://khj.zhiwuduotai.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://guj.yonumen.top

[I07] 忽略大小写与多行模式
来源：http://rpg.jianghu66.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://voz.yj20258.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oil.yvedp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://twp.zhongyouzk.top

TS:   /error/gim
来源：http://gly.nanxuanxn.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fyr.gogol.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gae.hywenlv.cn

Ruby: s.scan(/error/i)
来源：http://grt.jinqigfzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mxb.kuanghao11.cn

[I08] 贪婪与非贪婪匹配
来源：http://dok.wangshuangyany.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://otl.zhijiandao.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zms.cucudq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fui.chenlongwang.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aqm.ywan-chungtsiang.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://sgz.9152youxi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://abc.hysaishi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xbt.gogol.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qlz.ydzc1.top

================================================================================
来源：http://ugs.hammf.cn


<!-- 参考信息 -->