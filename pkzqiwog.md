代发 wailian999

JS:   this.name = "x";
来源：http://sph.pengpengdd.cyou

TS:   name: string = "x";
来源：http://zfn.quarkkingdee.top

Java: private String name;
来源：http://iyn.xylfe.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://osl.hnqzz.top

Ruby: @name = "x"
来源：http://yrf.ydzc1.top

C#:   public string Name { get; set; } = "x";
来源：http://tmj.havefunace.top

[G04] 定义方法
来源：http://zap.andypj.xyz

Py:   def greet(self): return self.name
来源：http://ywx.yvedp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ewo.hammf.cn

JS:   greet() { return this.name; }
来源：http://ysf.jinghuilouyu.cn

TS:   greet(): string { return this.name; }
来源：http://zwp.meibo888.top

Java: String greet() { return name; }
来源：http://ulf.ydjk.org.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ypb.yj202588.top

Ruby: def greet; @name; end
来源：http://lqu.kuanghao11.cn

C#:   public string Greet() => Name;
来源：http://tbo.52xcode.cn

[G05] 继承
来源：http://vnq.zhengqikj.top

Py:   class Admin(User): pass
来源：http://vqt.sweek.top

PHP:  class Admin extends User {}
来源：http://nwj.zhaomingkeji.xyz

JS:   class Admin extends User {}
来源：http://vql.smart0.xyz

TS:   class Admin extends User {}
来源：http://tyt.tarul.cn

Java: class Admin extends User {}
来源：http://fgv.vqdsnc.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bgn.pengpengdd.cyou

Ruby: class Admin < User; end
来源：http://gip.zhoulong.xyz

C#:   class Admin : User {}
来源：http://ecq.zhiwuduotai.top

[G06] 重写方法
来源：http://kze.yangfankeji.com

Py:   def greet(self): return "admin"
来源：http://elm.guowangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://aky.jinyuanbaomall.cn

JS:   greet() { return "admin"; }
来源：http://xvc.yangfankeji.com

TS:   greet(): string { return "admin"; }
来源：http://lvi.tian-w.cn

Java: @Override String greet() { return "admin"; }
来源：http://bpt.chenlongwang.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kgo.nwbrower.top

Ruby: def greet; "admin"; end
来源：http://nqm.redwolf501.top

C#:   public override string Greet() => "admin";
来源：http://ihc.ybcxt.top

[G07] 调用父类方法
来源：http://fsz.jlsjyb.cn

Py:   super().greet()
来源：http://iho.zhixingplan.top

PHP:  parent::greet();
来源：http://rmp.andypj.xyz

JS:   super.greet();
来源：http://efd.yueranfly.top

TS:   super.greet();
来源：http://bbv.shanyushiyangkeji.top

Java: super.greet();
来源：http://vbs.yj20258888.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ena.ehwqpu.com

Ruby: super
来源：http://oan.chenzaomai.com

C#:   base.Greet();
来源：http://eqk.jlsjyb.cn

[G08] 静态方法与属性
来源：http://cop.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mjl.epnwcf.com

PHP:  public static function f() {}
来源：http://sfm.shanyushiyangkeji.top

JS:   static f() {}
来源：http://hxg.hnqzz.top

TS:   static f(): void {}
来源：http://iyr.iojbl.cn

Java: static void f() {}
来源：http://tod.cdnleiting.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://lsd.birdmap.top

Ruby: def self.f; end
来源：http://npp.ctjpmb.com

C#:   public static void F() {}
来源：http://jxz.shanyushiyangtech.top

[G09] 接口 / 抽象类
来源：http://ere.hysaishi.cn

Py:   from abc import ABC, abstractmethod
来源：http://fmb.feifeiyinyue.top

PHP:  interface Shape { public function area(): float; }
来源：http://ldg.yj202588.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://lkh.ehwqpu.com

TS:   interface Shape { area(): number; }
来源：http://aqs.xziqi.cn

Java: interface Shape { double area(); }
来源：http://urb.cheryme.top

Go:   type Shape interface { Area() float64 }
来源：http://cpp.chenlongwang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xcn.shanyushiyangkeji.top

C#:   interface IShape { double Area(); }
来源：http://hcu.pycfn.com

[G10] 访问控制
来源：http://xei.daxiang520.top

Py:   约定 _protected / __private（不强制）
来源：http://pdq.pycfn.com

PHP:  public / protected / private
来源：http://yxn.daxiang520.top

JS:   #private 字段；其余公开
来源：http://wqf.pycfn.com

TS:   public / protected / private
来源：http://rmq.gaohongyu789.top

Java: public / protected / private / 默认包级
来源：http://vwb.xinyue.icu

Go:   首字母大写可导出，小写仅包内可见
来源：http://wnc.hcnkem.com

Ruby: public / protected / private
来源：http://gyb.fzhhl.top

C#:   public / protected / private / internal
来源：http://dvq.hesvh.cn

[G11] getter / setter
来源：http://uuu.birdmap.top

Py:   @property 与 @x.setter
来源：http://iqt.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rdg.zdqjudy.top

JS:   get name() { return this._name; }
来源：http://yit.vqdsnc.cn

TS:   get name(): string { return this._name; }
来源：http://huo.zhaomingkeji.xyz

Java: public String getName() { return name; }
来源：http://kgf.redwolf501.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://qqv.52xcode.cn

Ruby: attr_accessor :name
来源：http://oic.hnxiangtu.top

C#:   public string Name { get; set; }
来源：http://enh.quarkkingdee.top

[G12] 对象转字符串
来源：http://lbt.nanxuanxn.top

Py:   def __str__(self): return self.name
来源：http://sno.yangfankeji.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://lon.jqgufenzy.top

JS:   toString() { return this.name; }
来源：http://mkh.yuxming.cn

TS:   toString(): string { return this.name; }
来源：http://ujt.iojbl.cn

Java: @Override public String toString() { return name; }
来源：http://fgf.guannengcc.top

Go:   func (u User) String() string { return u.Name }
来源：http://xmo.cheryme.top

Ruby: def to_s; @name; end
来源：http://qrq.hammf.cn

C#:   public override string ToString() => Name;
来源：http://zaf.jqgufenzy.top

[G13] 判断对象类型
来源：http://wqm.zdbjq.cn

Py:   isinstance(u, User)
来源：http://dpp.ybcxt.top

PHP:  $u instanceof User
来源：http://mxg.chenjidiqi.icu

JS:   u instanceof User
来源：http://woj.kuanghao11.cn

TS:   u instanceof User
来源：http://pue.316326.xyz

Java: u instanceof User
来源：http://mcl.gaohongyu789.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lcy.jinghuilouyu.cn

Ruby: u.is_a?(User)
来源：http://sfj.wangshuangyany.cn

C#:   u is User
来源：http://tno.tian-w.cn

[G14] 数据类 / record
来源：http://fvc.feifeiyinyue.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ecu.feifeiyinyue.top

PHP:  // 用 readonly 属性模拟
来源：http://toj.ydjk.org.cn

JS:   // 无内置：普通类或对象字面量
来源：http://azo.yfazqb.com

TS:   type User = { name: string; age: number };
来源：http://npd.ybcxt.top

Java: record User(String name, int age) {}
来源：http://yjf.quarkkingdee.top

Go:   type User struct { Name string; Age int }
来源：http://qhk.guannengcc.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dsq.hcnkem.com

C#:   record User(string Name, int Age);
来源：http://bvc.yongpay.top

[G15] 枚举
来源：http://vxq.yj20258888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zue.hesvh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lwo.svipenyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://quf.yuanzhike.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://krg.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://tjz.hfpthk.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jcb.fehbvm.com

Ruby: Color = %i[red green].freeze
来源：http://asi.shanyushiyangkeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vnv.jinqigufen.top

[G16] 对象转数组 / 字典
来源：http://mxz.hysaishi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://brj.pengpengdd.cyou

PHP:  get_object_vars($obj);
来源：http://dze.nanxuanxn.top

JS:   Object.entries(obj)
来源：http://izf.tianlin.xyz

TS:   Object.entries(obj)
来源：http://rps.nanxuanxn.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://buf.sufxvd.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ebv.havefunace.top

Ruby: obj.instance_variables
来源：http://vwy.fehbvm.com

C#:   // 用反射或 System.Text.Json
来源：http://nrd.cdnleiting.top

================================================================================
来源：http://pkk.yonumen.top

H. 异常与错误处理
来源：http://zmr.tarul.cn

================================================================================
来源：http://qkt.ybcxt.top

[H01] try / catch 基础
来源：http://yli.yvedp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dbq.hnxiangtu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xrl.hnxiangtu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://irf.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ybx.0kj1m.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://omp.fktsv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qrb.ivvv.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wef.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mzb.fzhhl.top

[H02] finally / ensure 收尾
来源：http://rug.andypj.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://ige.ivvv.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://enc.xinyue.icu

JS:   try { f(); } finally { cleanup(); }
来源：http://hmr.aibaodan.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://suc.epnwcf.com

Java: try { f(); } finally { cleanup(); }
来源：http://fsx.zhoulong.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://mom.cdnleiting.top

Ruby: begin; f; ensure; cleanup; end
来源：http://vma.52xcode.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fef.zhaomingkeji.xyz

[H03] 主动抛出异常
来源：http://rhz.xinyue.icu

Py:   raise ValueError("错误信息")
来源：http://rsr.0kj1m.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lmj.fktsv.cn

JS:   throw new Error("错误信息");
来源：http://sga.cucudq.cn

TS:   throw new Error("错误信息");
来源：http://lxz.yongpay.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://sff.tanke756.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gzr.ctjpmb.com

Ruby: raise ArgumentError, "错误信息"
来源：http://clt.svipenyu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hro.fanxiaobao.xyz

[H04] 自定义异常类型
来源：http://zzy.tarul.cn

Py:   class MyError(Exception): pass
来源：http://pmh.gaohongyu789.top

PHP:  class MyError extends RuntimeException {}
来源：http://yen.sufxvd.cn

JS:   class MyError extends Error {}
来源：http://bbz.quarkkingdee.top

TS:   class MyError extends Error {}
来源：http://cwq.guannengcc.top

Java: class MyException extends RuntimeException {}
来源：http://bsg.gogol.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://igr.jianghu66.top

Ruby: class MyError < StandardError; end
来源：http://chz.nwbrower.top

C#:   class MyException : Exception {}
来源：http://csw.gotoacloud.top

[H05] 捕获特定类型
来源：http://hzm.yuanzhike.top

Py:   except ValueError as e:
来源：http://vxm.yueranfly.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://joo.yangfankeji.com

JS:   if (e instanceof TypeError) {}
来源：http://xyc.shuidangran.top

TS:   if (e instanceof TypeError) {}
来源：http://czh.xuetiantiany.cn

Java: catch (IOException | SQLException e) {}
来源：http://ezn.ivvv.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vml.jinqigfzy.top

Ruby: rescue ArgumentError => e
来源：http://hba.snrcjt.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yvi.quarkkingdee.top

[H06] 可选值 / 空值安全访问
来源：http://tph.chenjidiqi.icu

Py:   value = d.get("k") or default
来源：http://wfq.ivvv.top

PHP:  $v = $d["k"] ?? null;
来源：http://bqu.wangshuangyany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://eas.chenlongwang.top

TS:   obj?.a?.b;  d ?? default
来源：http://kra.yangfankeji.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ywm.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://qhz.sysykeji.top

Ruby: d&.dig(:a, :b)
来源：http://sbg.shuidangran.top

C#:   obj?.A?.B ?? default
来源：http://uui.pengpengdd.cyou

[H07] 断言
来源：http://lbu.aibaodan.cn

Py:   assert x > 0, "必须为正"
来源：http://bac.sweek.top

PHP:  assert($x > 0);
来源：http://sgn.yfazqb.com

JS:   console.assert(x > 0);
来源：http://lvu.hongshengwenyu.top

TS:   console.assert(x > 0);
来源：http://peo.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://yjc.zhongyouzk.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xpt.guowangkeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://ywn.fzhhl.top

C#:   Debug.Assert(x > 0);
来源：http://hnu.ydjk.org.cn

[H08] 获取错误信息与堆栈
来源：http://eij.9152youxi.cn

Py:   str(e);  traceback.format_exc()
来源：http://jpw.chenjidiqi.icu

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uvt.redwolf501.top

JS:   e.message;  e.stack
来源：http://ioi.9152youxi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ggv.shuidangran.top

Java: e.getMessage();  e.printStackTrace()
来源：http://exi.gaohongyu789.top

Go:   err.Error()
来源：http://fld.cheryme.top

Ruby: e.message;  e.backtrace
来源：http://dsh.ydzc1.top

C#:   e.Message;  e.StackTrace
来源：http://hcu.jyoumei.cn

[H09] 带错误码的异常
来源：http://ddq.9152youxi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tjl.ywan-chungtsiang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://bwu.feifeiyinyue.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zxq.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fhw.jinghuilouyu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rqd.yongpay.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gdp.daxiang520.top

Ruby: raise MyError.new("fail", 500)
来源：http://ddz.shzxlz.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lkf.bjfxy.top

[H10] 资源自动释放
来源：http://onf.iojbl.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sgk.dianchejie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fba.zhongyouzk.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qfh.ywan-chungtsiang.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hda.ivvv.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uec.hnqzz.top

Go:   defer f.Close()
来源：http://bfe.nanxinkj.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://efl.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nad.hcnkem.com

================================================================================
来源：http://pnt.yuxming.cn

I. 正则表达式
来源：http://aoh.tianlin.xyz

================================================================================
来源：http://dzt.zhijiandao.cn

[I01] 判断是否匹配
来源：http://goj.jqgufenzy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://upw.hesvh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oxb.hongshengwenyu.top

JS:   /\d+/.test(s)
来源：http://oaj.daria6918.cn

TS:   /\d+/.test(s)
来源：http://czi.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://drw.gogol.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lmm.bjfxy.top

Ruby: s.match?(/\d+/)
来源：http://luk.kuanghao11.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dga.jiagoushi.top

[I02] 提取所有匹配
来源：http://zgd.sjlbkw.cn

Py:   re.findall(r"\d+", s)
来源：http://hzg.vqdsnc.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vfs.ybcxt.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://upx.yuanzhike.top

TS:   s.match(/\d+/g)
来源：http://rma.bjfxy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jof.chenlongwang.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zlb.yj20258.top

Ruby: s.scan(/\d+/)
来源：http://kzc.cucudq.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uod.snrcjt.cn

[I03] 提取捕获分组
来源：http://eko.zhijiandao.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ufz.nanxuanxn.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://shl.wangdashe.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wbd.cucudq.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zfx.redwolf501.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dna.xuanzx.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ugl.uphjek.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://goy.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wqp.nanxuanxn.top

[I04] 正则替换
来源：http://wiy.zhijiandao.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fjl.vehdjk.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ute.hnxiangtu.top

JS:   s.replace(/\d+/g, "#")
来源：http://cns.cdnleiting.top

TS:   s.replace(/\d+/g, "#")
来源：http://yjx.ppjwa.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tbh.zhoulong.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://psq.yueranfly.top

Ruby: s.gsub(/\d+/, "#")
来源：http://ase.havefunace.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://nug.zhongyouzk.top

[I05] 按正则拆分
来源：http://gdp.zdbjq.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jsy.gaohongyu789.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://sip.316326.xyz

JS:   s.split(/\s*,\s*/)
来源：http://rma.daria6918.cn

TS:   s.split(/\s*,\s*/)
来源：http://qpa.cdnleiting.top

Java: s.split("\\s*,\\s*")
来源：http://tdh.0kj1m.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ifl.shzxlz.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xwa.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ovu.aibaodan.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dnu.shanyushiyangtech.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kwa.feifeiyinyue.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://agx.xuanzx.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iyx.yangfankeji.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fxd.zhoulong.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lre.fktsv.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rrd.ctjpmb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vca.gogol.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bix.tian-w.cn

[I07] 忽略大小写与多行模式
来源：http://bby.shzxlz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ddj.ywan-chungtsiang.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ydi.ctjpmb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zxv.havefunace.top

TS:   /error/gim
来源：http://tzm.zdqjudy.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qrm.yongpay.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fib.sxryk.cn

Ruby: s.scan(/error/i)
来源：http://abz.cashguo.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ueo.hongshengwenyu.top

[I08] 贪婪与非贪婪匹配
来源：http://qks.gotoacloud.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jwo.yj20258.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://edp.cdnleiting.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://svn.shangyingyoupin.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bjz.shzxlz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sxj.wangshuangyany.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rpp.jinghuilouyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zjd.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ttz.aibaodan.cn

================================================================================
来源：http://vrz.daxiang520.top

J. 日期与时间
来源：http://kcm.jinyuanbaomall.cn

================================================================================
来源：http://bzi.c1oappe.top

[J01] 获取当前时间
来源：http://kzx.yvedp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cgn.nanxinkj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vnn.snrcjt.cn

JS:   new Date();  Date.now()
来源：http://uso.epnwcf.com

TS:   new Date();  Date.now()
来源：http://acp.meibo888.top

Java: LocalDateTime.now();  Instant.now()
来源：http://ybh.yanxiufei.cn


<!-- 参考信息 -->