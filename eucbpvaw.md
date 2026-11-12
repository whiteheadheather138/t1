代发 wailian999

JS:   this.name = "x";
来源：http://rnr.havefunace.top

TS:   name: string = "x";
来源：http://jsy.jyoumei.cn

Java: private String name;
来源：http://njr.tianlin.xyz

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dfr.wangdashe.top

Ruby: @name = "x"
来源：http://wgk.nanxinkj.top

C#:   public string Name { get; set; } = "x";
来源：http://pcg.jyoumei.cn

[G04] 定义方法
来源：http://vwn.xziqi.cn

Py:   def greet(self): return self.name
来源：http://pmb.chenjidiqi.icu

PHP:  public function greet(): string { return $this->name; }
来源：http://mjf.xylfe.cn

JS:   greet() { return this.name; }
来源：http://rmv.ctjpmb.com

TS:   greet(): string { return this.name; }
来源：http://cri.gzhubu.top

Java: String greet() { return name; }
来源：http://mfw.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://wvk.chenjidiqi.icu

Ruby: def greet; @name; end
来源：http://ynx.yueranfly.top

C#:   public string Greet() => Name;
来源：http://lwd.smart0.xyz

[G05] 继承
来源：http://unc.zhiwuduotai.top

Py:   class Admin(User): pass
来源：http://hrl.xziqi.cn

PHP:  class Admin extends User {}
来源：http://swe.epnwcf.com

JS:   class Admin extends User {}
来源：http://jka.birdmap.top

TS:   class Admin extends User {}
来源：http://jfz.snrcjt.cn

Java: class Admin extends User {}
来源：http://tlz.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://omt.daria6918.cn

Ruby: class Admin < User; end
来源：http://plu.sufxvd.cn

C#:   class Admin : User {}
来源：http://wyp.ehwqpu.com

[G06] 重写方法
来源：http://wni.dashuyun.cn

Py:   def greet(self): return "admin"
来源：http://owz.hfpthk.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xce.zdqjudy.top

JS:   greet() { return "admin"; }
来源：http://oli.smart0.xyz

TS:   greet(): string { return "admin"; }
来源：http://hby.fanxiaobao.xyz

Java: @Override String greet() { return "admin"; }
来源：http://ila.svipenyu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ike.fzhhl.top

Ruby: def greet; "admin"; end
来源：http://omw.zhiwuduotai.top

C#:   public override string Greet() => "admin";
来源：http://xey.ydzc1.top

[G07] 调用父类方法
来源：http://snc.snrcjt.cn

Py:   super().greet()
来源：http://bay.sysykeji.top

PHP:  parent::greet();
来源：http://zyu.cqqwz.cn

JS:   super.greet();
来源：http://eht.jlsjyb.cn

TS:   super.greet();
来源：http://qmz.quarkkingdee.top

Java: super.greet();
来源：http://eia.hywenlv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://lkq.cheryme.top

Ruby: super
来源：http://lxj.tarul.cn

C#:   base.Greet();
来源：http://kvv.hesvh.cn

[G08] 静态方法与属性
来源：http://fpe.sufxvd.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vir.shzxlz.cn

PHP:  public static function f() {}
来源：http://uno.tian-w.cn

JS:   static f() {}
来源：http://wub.yonumen.top

TS:   static f(): void {}
来源：http://rhv.aizwys.cn

Java: static void f() {}
来源：http://ike.pengpengdd.cyou

Go:   // 无 static：用包级函数，按包名调用
来源：http://kve.fehbvm.com

Ruby: def self.f; end
来源：http://zpn.hammf.cn

C#:   public static void F() {}
来源：http://ttp.xinyue.icu

[G09] 接口 / 抽象类
来源：http://xkq.yonumen.top

Py:   from abc import ABC, abstractmethod
来源：http://rfq.ctjpmb.com

PHP:  interface Shape { public function area(): float; }
来源：http://twf.zycfv.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qus.shuidangran.top

TS:   interface Shape { area(): number; }
来源：http://buj.yongpay.top

Java: interface Shape { double area(); }
来源：http://xkt.vehdjk.com

Go:   type Shape interface { Area() float64 }
来源：http://siw.9152youxi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jgj.xuetiantiany.cn

C#:   interface IShape { double Area(); }
来源：http://yhe.hammf.cn

[G10] 访问控制
来源：http://jdb.yueranfly.top

Py:   约定 _protected / __private（不强制）
来源：http://nlr.snrcjt.cn

PHP:  public / protected / private
来源：http://fqa.cucudq.cn

JS:   #private 字段；其余公开
来源：http://uly.havefunace.top

TS:   public / protected / private
来源：http://yku.hesvh.cn

Java: public / protected / private / 默认包级
来源：http://sns.fanxiaobao.xyz

Go:   首字母大写可导出，小写仅包内可见
来源：http://aex.daria6918.cn

Ruby: public / protected / private
来源：http://eea.ctjpmb.com

C#:   public / protected / private / internal
来源：http://qyw.mhx1999.top

[G11] getter / setter
来源：http://mjc.jlsjyb.cn

Py:   @property 与 @x.setter
来源：http://pji.shzxlz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://axs.hongshengwenyu.top

JS:   get name() { return this._name; }
来源：http://zqm.hammf.cn

TS:   get name(): string { return this._name; }
来源：http://gjn.yj20258.top

Java: public String getName() { return name; }
来源：http://dgd.shuidangran.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://xxj.zdqjudy.top

Ruby: attr_accessor :name
来源：http://yen.gzhubu.top

C#:   public string Name { get; set; }
来源：http://mvi.yongpay.top

[G12] 对象转字符串
来源：http://klu.dashuyun.cn

Py:   def __str__(self): return self.name
来源：http://uvq.xuetiantiany.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vhc.birdmap.top

JS:   toString() { return this.name; }
来源：http://yxz.zhengqikj.top

TS:   toString(): string { return this.name; }
来源：http://szr.zhixingplan.top

Java: @Override public String toString() { return name; }
来源：http://iww.gzhubu.top

Go:   func (u User) String() string { return u.Name }
来源：http://poy.tanke756.top

Ruby: def to_s; @name; end
来源：http://hxa.svipenyu.cn

C#:   public override string ToString() => Name;
来源：http://hhw.xuanzx.com

[G13] 判断对象类型
来源：http://uxb.yvedp.cn

Py:   isinstance(u, User)
来源：http://eew.52xcode.cn

PHP:  $u instanceof User
来源：http://mgs.dianchejie.cn

JS:   u instanceof User
来源：http://xvm.wangdashe.top

TS:   u instanceof User
来源：http://rlg.shanyushiyangkeji.top

Java: u instanceof User
来源：http://lsf.haohaochexian.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ikp.mhx1999.top

Ruby: u.is_a?(User)
来源：http://clr.haohaochexian.top

C#:   u is User
来源：http://gof.shuidangran.top

[G14] 数据类 / record
来源：http://rou.ctjpmb.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tqq.jqgfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://dtr.guowangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://bew.bbcook.cn

TS:   type User = { name: string; age: number };
来源：http://est.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://pur.vehdjk.com

Go:   type User struct { Name string; Age int }
来源：http://jvg.shanyushiyangkeji.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lmy.yj20258.top

C#:   record User(string Name, int Age);
来源：http://tnr.vqdsnc.cn

[G15] 枚举
来源：http://zcb.guannengcc.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eth.zhongyouzk.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ufv.tanke756.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rpn.zdqjudy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oqq.52xcode.cn

Java: enum Color { RED, GREEN }
来源：http://zbb.gzhubu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://csz.hammf.cn

Ruby: Color = %i[red green].freeze
来源：http://nez.fengsongda.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kul.vqdsnc.cn

[G16] 对象转数组 / 字典
来源：http://mqd.bbcook.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gha.daxiang520.top

PHP:  get_object_vars($obj);
来源：http://mts.meibo888.top

JS:   Object.entries(obj)
来源：http://pmt.yueranfly.top

TS:   Object.entries(obj)
来源：http://xaa.shanyushiyangkeji.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vql.pycfn.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://ikj.xziqi.cn

Ruby: obj.instance_variables
来源：http://jrv.hnxiangtu.top

C#:   // 用反射或 System.Text.Json
来源：http://cbh.jinqigufen.top

================================================================================
来源：http://khx.bbcook.cn

H. 异常与错误处理
来源：http://mwi.fengsongda.top

================================================================================
来源：http://krh.kuanghao11.cn

[H01] try / catch 基础
来源：http://ksv.dianchejie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://csx.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ccm.zhaomingkeji.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://suc.sxryk.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kpq.andypj.xyz

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sbq.snrcjt.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ego.hnxiangtu.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vva.nwbrower.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iqo.yongpay.top

[H02] finally / ensure 收尾
来源：http://jmo.daria6918.cn

Py:   try: f()⏎finally: cleanup()
来源：http://eyh.yangfankeji.com

PHP:  try { f(); } finally { cleanup(); }
来源：http://ltg.yvedp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tkb.jinqigufen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://klo.hcnkem.com

Java: try { f(); } finally { cleanup(); }
来源：http://zog.gzhubu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://coa.daria6918.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hcn.cdnleiting.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://jsi.xuanzx.com

[H03] 主动抛出异常
来源：http://oei.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://xys.ctjpmb.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pqx.gogol.net.cn

JS:   throw new Error("错误信息");
来源：http://swk.jqgfzy.top

TS:   throw new Error("错误信息");
来源：http://yuv.jinqigfzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mmq.chenjidiqi.icu

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://epx.yanxiufei.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://grg.ybcxt.top

C#:   throw new ArgumentException("错误信息");
来源：http://jyy.zhiwuduotai.top

[H04] 自定义异常类型
来源：http://ask.tianlin.xyz

Py:   class MyError(Exception): pass
来源：http://lot.yuanzhike.top

PHP:  class MyError extends RuntimeException {}
来源：http://xsd.jyoumei.cn

JS:   class MyError extends Error {}
来源：http://nuj.zhoulong.xyz

TS:   class MyError extends Error {}
来源：http://ycl.daria6918.cn

Java: class MyException extends RuntimeException {}
来源：http://wnl.yongpay.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uaw.uphjek.com

Ruby: class MyError < StandardError; end
来源：http://bao.daria6918.cn

C#:   class MyException : Exception {}
来源：http://ldw.ctjpmb.com

[H05] 捕获特定类型
来源：http://wtq.jlsjyb.cn

Py:   except ValueError as e:
来源：http://tyg.sufxvd.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yuv.xylfe.cn

JS:   if (e instanceof TypeError) {}
来源：http://vmm.gogol.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://ino.bjfxy.top

Java: catch (IOException | SQLException e) {}
来源：http://qhj.ppjwa.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vny.mhx1999.top

Ruby: rescue ArgumentError => e
来源：http://yja.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://slt.yonumen.top

[H06] 可选值 / 空值安全访问
来源：http://rcx.yuxming.cn

Py:   value = d.get("k") or default
来源：http://ygu.snrcjt.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ule.vqdsnc.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lrr.meibo888.top

TS:   obj?.a?.b;  d ?? default
来源：http://oqt.yj20258.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bmf.zycfv.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rnq.aibaodan.cn

Ruby: d&.dig(:a, :b)
来源：http://adn.c1oappe.top

C#:   obj?.A?.B ?? default
来源：http://fnw.jqgfzy.top

[H07] 断言
来源：http://xrs.shuidangran.top

Py:   assert x > 0, "必须为正"
来源：http://yvo.xziqi.cn

PHP:  assert($x > 0);
来源：http://nbh.xingfuxueyuan.xyz

JS:   console.assert(x > 0);
来源：http://jko.cheryme.top

TS:   console.assert(x > 0);
来源：http://lcu.ivvv.top

Java: assert x > 0 : "必须为正";
来源：http://hfd.wangshuangyany.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://utg.hnxiangtu.top

Ruby: raise "必须为正" unless x > 0
来源：http://qbc.jinghuilouyu.cn

C#:   Debug.Assert(x > 0);
来源：http://vyc.yuxming.cn

[H08] 获取错误信息与堆栈
来源：http://kqo.chenlongwang.top

Py:   str(e);  traceback.format_exc()
来源：http://njk.svipenyu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xaw.yongpay.top

JS:   e.message;  e.stack
来源：http://hon.ctjpmb.com

TS:   e instanceof Error ? e.message : String(e)
来源：http://sza.zhiwuduotai.top

Java: e.getMessage();  e.printStackTrace()
来源：http://xes.redwolf501.top

Go:   err.Error()
来源：http://mcj.jinyuanbaomall.cn

Ruby: e.message;  e.backtrace
来源：http://idi.xziqi.cn

C#:   e.Message;  e.StackTrace
来源：http://ohd.vehdjk.com

[H09] 带错误码的异常
来源：http://ueg.birdmap.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gva.dianchejie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tjx.ehwqpu.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zsd.hnqzz.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ivo.tian-w.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rqy.tarul.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oac.xuetiantiany.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dok.yj20258888.top

C#:   // 自定义异常类中加 Code 属性
来源：http://smf.cheryme.top

[H10] 资源自动释放
来源：http://pme.snrcjt.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rnd.gzhubu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tfu.jinqigfzy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sxb.zhiwuduotai.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qly.ydzc1.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ort.vqdsnc.cn

Go:   defer f.Close()
来源：http://flo.jiagoushi.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hat.xuanzx.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pyu.52xcode.cn

================================================================================
来源：http://npp.zhongyouzk.top

I. 正则表达式
来源：http://jaf.xylfe.cn

================================================================================
来源：http://pdw.smart0.xyz

[I01] 判断是否匹配
来源：http://nlm.quarkkingdee.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cec.wangdashe.top

PHP:  preg_match('/\d+/', $s);
来源：http://upz.zhongyouzk.top

JS:   /\d+/.test(s)
来源：http://owr.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://oda.nwbrower.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ehg.zhaomingkeji.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rfc.aibaodan.cn

Ruby: s.match?(/\d+/)
来源：http://ocf.zhoulong.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hqe.fanxiaobao.xyz

[I02] 提取所有匹配
来源：http://ysu.chenzaomai.com

Py:   re.findall(r"\d+", s)
来源：http://rzv.yfazqb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://con.shanyushiyangkeji.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://deg.gzhubu.top

TS:   s.match(/\d+/g)
来源：http://enk.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://npl.aibaodan.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://smx.yj202588.top

Ruby: s.scan(/\d+/)
来源：http://twd.chenzaomai.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ijd.ppjwa.cn

[I03] 提取捕获分组
来源：http://bhk.xinyue.icu

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://icl.feifeiyinyue.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kkr.chenlongwang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ntb.chenlongwang.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vmr.316326.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hij.jinqigufen.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bjj.tian-w.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://djk.smart0.xyz

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fma.quarkkingdee.top

[I04] 正则替换
来源：http://sbn.sufxvd.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ogw.gotoacloud.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ibu.cucudq.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ysi.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vdy.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://spx.shuidangran.top

Go:   re.ReplaceAllString(s, "#")
来源：http://xaz.vqdsnc.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lgk.zhoulong.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rqn.9152youxi.cn

[I05] 按正则拆分
来源：http://pig.hcnkem.com

Py:   re.split(r"\s*,\s*", s)
来源：http://crb.ctjpmb.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ojg.gotoacloud.top

JS:   s.split(/\s*,\s*/)
来源：http://opu.yj20258888.top

TS:   s.split(/\s*,\s*/)
来源：http://ulk.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://ccl.sxryk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tqz.yfazqb.com

Ruby: s.split(/\s*,\s*/)
来源：http://zuf.xziqi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yta.cqqwz.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uxa.smart0.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fyj.xinyue.icu

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aqe.fktsv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uci.iojbl.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wmd.pycfn.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rse.shanyushiyangtech.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iww.xziqi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://luv.mhx1999.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://shw.cucudq.cn

[I07] 忽略大小写与多行模式
来源：http://zid.gaohongyu789.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gyi.jianghu66.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nta.hongshengwenyu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://geh.daria6918.cn

TS:   /error/gim
来源：http://nng.jianghu66.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dhj.svipenyu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dfn.cqqwz.cn

Ruby: s.scan(/error/i)
来源：http://xka.aizwys.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://irx.sxryk.cn

[I08] 贪婪与非贪婪匹配
来源：http://uue.sweek.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nwq.shuidangran.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ttp.shzxlz.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://maw.zdbjq.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://riq.sweek.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ptt.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wvv.9152youxi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ntu.fzhhl.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vmw.gotoacloud.top

================================================================================
来源：http://bzy.yvedp.cn

J. 日期与时间
来源：http://jif.aibaodan.cn

================================================================================
来源：http://eio.daria6918.cn

[J01] 获取当前时间
来源：http://lfd.zhijiandao.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://liv.zhijiandao.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bqs.sjlbkw.cn

JS:   new Date();  Date.now()
来源：http://dze.xuanzx.com

TS:   new Date();  Date.now()
来源：http://eyz.zhiwuduotai.top

Java: LocalDateTime.now();  Instant.now()
来源：http://mmu.wangdashe.top


<!-- 参考信息 -->