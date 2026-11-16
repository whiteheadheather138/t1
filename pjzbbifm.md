代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://yim.aibaodan.cn

[G03] 实例属性
来源：http://eva.xziqi.cn

Py:   self.name = "x"
来源：http://tku.zdbjq.cn

PHP:  public string $name = "x";
来源：http://ima.c1oappe.top

JS:   this.name = "x";
来源：http://soh.xuetiantiany.cn

TS:   name: string = "x";
来源：http://gos.sufxvd.cn

Java: private String name;
来源：http://ogd.quarkkingdee.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kyd.epnwcf.com

Ruby: @name = "x"
来源：http://bwh.sysykeji.top

C#:   public string Name { get; set; } = "x";
来源：http://bcu.vehdjk.com

[G04] 定义方法
来源：http://eah.nanxinkj.top

Py:   def greet(self): return self.name
来源：http://hrx.shanyushiyangtech.top

PHP:  public function greet(): string { return $this->name; }
来源：http://elq.fzhhl.top

JS:   greet() { return this.name; }
来源：http://elr.xziqi.cn

TS:   greet(): string { return this.name; }
来源：http://lfl.gogol.net.cn

Java: String greet() { return name; }
来源：http://rrd.zhongyouzk.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://prp.nwbrower.top

Ruby: def greet; @name; end
来源：http://frj.zhoulong.xyz

C#:   public string Greet() => Name;
来源：http://iri.xuetiantiany.cn

[G05] 继承
来源：http://fxv.tarul.cn

Py:   class Admin(User): pass
来源：http://scj.52xcode.cn

PHP:  class Admin extends User {}
来源：http://nvh.guannengcc.top

JS:   class Admin extends User {}
来源：http://vnf.iojbl.cn

TS:   class Admin extends User {}
来源：http://asm.jinghuilouyu.cn

Java: class Admin extends User {}
来源：http://buc.haohaochexian.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kjz.chenzaomai.com

Ruby: class Admin < User; end
来源：http://ccx.sjlbkw.cn

C#:   class Admin : User {}
来源：http://xvh.c1oappe.top

[G06] 重写方法
来源：http://eui.ybcxt.top

Py:   def greet(self): return "admin"
来源：http://sdg.nanxinkj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://eij.hywenlv.cn

JS:   greet() { return "admin"; }
来源：http://gjw.birdmap.top

TS:   greet(): string { return "admin"; }
来源：http://lqr.fktsv.cn

Java: @Override String greet() { return "admin"; }
来源：http://brh.ctjpmb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dzm.fanxiaobao.xyz

Ruby: def greet; "admin"; end
来源：http://cam.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://voj.hfpthk.cn

[G07] 调用父类方法
来源：http://ocg.hysaishi.cn

Py:   super().greet()
来源：http://joh.fzhhl.top

PHP:  parent::greet();
来源：http://vru.fanxiaobao.xyz

JS:   super.greet();
来源：http://hyj.nanxuanxn.top

TS:   super.greet();
来源：http://uzb.ydjk.org.cn

Java: super.greet();
来源：http://uvm.jinyuanbaomall.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cxx.epnwcf.com

Ruby: super
来源：http://bib.ppjwa.cn

C#:   base.Greet();
来源：http://sta.sxryk.cn

[G08] 静态方法与属性
来源：http://usv.jiagoushi.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://upl.feifeiyinyue.top

PHP:  public static function f() {}
来源：http://tyc.hammf.cn

JS:   static f() {}
来源：http://wfj.yueranfly.top

TS:   static f(): void {}
来源：http://aim.ctjpmb.com

Java: static void f() {}
来源：http://eym.xuetiantiany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uci.sufxvd.cn

Ruby: def self.f; end
来源：http://amz.jqgufenzy.top

C#:   public static void F() {}
来源：http://oyd.xuetiantiany.cn

[G09] 接口 / 抽象类
来源：http://mpg.fengsongda.top

Py:   from abc import ABC, abstractmethod
来源：http://vzi.yueranfly.top

PHP:  interface Shape { public function area(): float; }
来源：http://ecq.hcnkem.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://tko.52xcode.cn

TS:   interface Shape { area(): number; }
来源：http://sur.chenjidiqi.icu

Java: interface Shape { double area(); }
来源：http://oeu.zycfv.cn

Go:   type Shape interface { Area() float64 }
来源：http://uaj.hnqzz.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lpt.zhaomingkeji.xyz

C#:   interface IShape { double Area(); }
来源：http://ngi.hywenlv.cn

[G10] 访问控制
来源：http://kpz.zhongyouzk.top

Py:   约定 _protected / __private（不强制）
来源：http://ful.cheryme.top

PHP:  public / protected / private
来源：http://yhf.ydzc1.top

JS:   #private 字段；其余公开
来源：http://xxd.chenlongwang.top

TS:   public / protected / private
来源：http://mux.cqqwz.cn

Java: public / protected / private / 默认包级
来源：http://zme.cheryme.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://aju.xylfe.cn

Ruby: public / protected / private
来源：http://tlo.sjlbkw.cn

C#:   public / protected / private / internal
来源：http://idl.c1oappe.top

[G11] getter / setter
来源：http://pkr.havefunace.top

Py:   @property 与 @x.setter
来源：http://zcv.sjlbkw.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vwj.hesvh.cn

JS:   get name() { return this._name; }
来源：http://uwx.yvedp.cn

TS:   get name(): string { return this._name; }
来源：http://ngw.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://qgw.bbcook.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yva.chenzaomai.com

Ruby: attr_accessor :name
来源：http://grj.gaohongyu789.top

C#:   public string Name { get; set; }
来源：http://imu.yanxiufei.cn

[G12] 对象转字符串
来源：http://hnv.ctjpmb.com

Py:   def __str__(self): return self.name
来源：http://fnh.zhoulong.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://ffb.ivvv.top

JS:   toString() { return this.name; }
来源：http://fmz.ivvv.top

TS:   toString(): string { return this.name; }
来源：http://vgr.52xcode.cn

Java: @Override public String toString() { return name; }
来源：http://xlw.meibo888.top

Go:   func (u User) String() string { return u.Name }
来源：http://zvo.fehbvm.com

Ruby: def to_s; @name; end
来源：http://wdp.aibaodan.cn

C#:   public override string ToString() => Name;
来源：http://uia.chenlongwang.top

[G13] 判断对象类型
来源：http://cgm.jqgufenzy.top

Py:   isinstance(u, User)
来源：http://ozs.xylfe.cn

PHP:  $u instanceof User
来源：http://sxh.c1oappe.top

JS:   u instanceof User
来源：http://wyp.zdbjq.cn

TS:   u instanceof User
来源：http://isu.nwbrower.top

Java: u instanceof User
来源：http://dat.birdmap.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ttc.jinyuanbaomall.cn

Ruby: u.is_a?(User)
来源：http://cvc.shuidangran.top

C#:   u is User
来源：http://wxy.zhiwuduotai.top

[G14] 数据类 / record
来源：http://bpt.yueranfly.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zfm.vehdjk.com

PHP:  // 用 readonly 属性模拟
来源：http://ezz.gotoacloud.top

JS:   // 无内置：普通类或对象字面量
来源：http://fil.jianghu66.top

TS:   type User = { name: string; age: number };
来源：http://moo.sysykeji.top

Java: record User(String name, int age) {}
来源：http://wbn.ehwqpu.com

Go:   type User struct { Name string; Age int }
来源：http://qnl.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oay.gaohongyu789.top

C#:   record User(string Name, int Age);
来源：http://shc.zdbjq.cn

[G15] 枚举
来源：http://dhk.xuetiantiany.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jiz.ctjpmb.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://lkk.hysaishi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kvo.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lxp.xinyue.icu

Java: enum Color { RED, GREEN }
来源：http://tzn.yuanzhike.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dmv.redwolf501.top

Ruby: Color = %i[red green].freeze
来源：http://hlw.feifeiyinyue.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uvw.yvedp.cn

[G16] 对象转数组 / 字典
来源：http://trh.vehdjk.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bkr.ybcxt.top

PHP:  get_object_vars($obj);
来源：http://svz.xinyue.icu

JS:   Object.entries(obj)
来源：http://kan.daxiang520.top

TS:   Object.entries(obj)
来源：http://vkc.shangyingyoupin.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ysk.shzxlz.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tbc.cqqwz.cn

Ruby: obj.instance_variables
来源：http://sec.xingfuxueyuan.xyz

C#:   // 用反射或 System.Text.Json
来源：http://wdc.ehwqpu.com

================================================================================
来源：http://inh.gogol.net.cn

H. 异常与错误处理
来源：http://onk.bjfxy.top

================================================================================
来源：http://yzg.aizwys.cn

[H01] try / catch 基础
来源：http://kjy.9152youxi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eng.nanxuanxn.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ckt.xuetiantiany.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gqh.zhiwuduotai.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wxg.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gua.tarul.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rpg.vqdsnc.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mla.yuanzhike.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rvi.shuidangran.top

[H02] finally / ensure 收尾
来源：http://qns.ctjpmb.com

Py:   try: f()⏎finally: cleanup()
来源：http://yac.zdqjudy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://pzw.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://fsz.yonumen.top

TS:   try { f(); } finally { cleanup(); }
来源：http://okk.zdqjudy.top

Java: try { f(); } finally { cleanup(); }
来源：http://ahd.sweek.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://sgw.guannengcc.top

Ruby: begin; f; ensure; cleanup; end
来源：http://waw.fktsv.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qhn.jinqigfzy.top

[H03] 主动抛出异常
来源：http://pfl.andypj.xyz

Py:   raise ValueError("错误信息")
来源：http://ogs.daria6918.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pmd.chenlongwang.top

JS:   throw new Error("错误信息");
来源：http://pan.shanyushiyangtech.top

TS:   throw new Error("错误信息");
来源：http://wrx.xingfuxueyuan.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://quu.jyoumei.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oah.meibo888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pof.sweek.top

C#:   throw new ArgumentException("错误信息");
来源：http://fjg.tarul.cn

[H04] 自定义异常类型
来源：http://pwk.chenzaomai.com

Py:   class MyError(Exception): pass
来源：http://ubi.yongpay.top

PHP:  class MyError extends RuntimeException {}
来源：http://die.yuxming.cn

JS:   class MyError extends Error {}
来源：http://vfl.dashuyun.cn

TS:   class MyError extends Error {}
来源：http://esy.shangyingyoupin.top

Java: class MyException extends RuntimeException {}
来源：http://tch.nwbrower.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://obd.andypj.xyz

Ruby: class MyError < StandardError; end
来源：http://kax.gaohongyu789.top

C#:   class MyException : Exception {}
来源：http://xno.birdmap.top

[H05] 捕获特定类型
来源：http://sho.yanxiufei.cn

Py:   except ValueError as e:
来源：http://nyx.snrcjt.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://izh.xuetiantiany.cn

JS:   if (e instanceof TypeError) {}
来源：http://lab.ybcxt.top

TS:   if (e instanceof TypeError) {}
来源：http://bdu.gaohongyu789.top

Java: catch (IOException | SQLException e) {}
来源：http://abu.jiagoushi.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jgx.cdnleiting.top

Ruby: rescue ArgumentError => e
来源：http://qif.jinqigufen.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zad.ydjk.org.cn

[H06] 可选值 / 空值安全访问
来源：http://tza.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://pct.mhx1999.top

PHP:  $v = $d["k"] ?? null;
来源：http://vfn.wangshuangyany.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pti.haohaochexian.top

TS:   obj?.a?.b;  d ?? default
来源：http://xon.jinqigfzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://oex.aizwys.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jhy.zhixingplan.top

Ruby: d&.dig(:a, :b)
来源：http://ljx.bbcook.cn

C#:   obj?.A?.B ?? default
来源：http://iqk.wangdashe.top

[H07] 断言
来源：http://nrx.redwolf501.top

Py:   assert x > 0, "必须为正"
来源：http://edl.hnqzz.top

PHP:  assert($x > 0);
来源：http://uwq.epnwcf.com

JS:   console.assert(x > 0);
来源：http://nvp.jinyuanbaomall.cn

TS:   console.assert(x > 0);
来源：http://rwu.jinqigufen.top

Java: assert x > 0 : "必须为正";
来源：http://rux.zdqjudy.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sjx.snrcjt.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ukv.zdqjudy.top

C#:   Debug.Assert(x > 0);
来源：http://wue.gaohongyu789.top

[H08] 获取错误信息与堆栈
来源：http://iwq.shanyushiyangkeji.top

Py:   str(e);  traceback.format_exc()
来源：http://gkd.zhoulong.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tpf.yuanzhike.top

JS:   e.message;  e.stack
来源：http://rzz.jianghu66.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tmv.andypj.xyz

Java: e.getMessage();  e.printStackTrace()
来源：http://ova.jiagoushi.top

Go:   err.Error()
来源：http://asm.ybcxt.top

Ruby: e.message;  e.backtrace
来源：http://vfv.52xcode.cn

C#:   e.Message;  e.StackTrace
来源：http://ywd.jqgfzy.top

[H09] 带错误码的异常
来源：http://rmx.xuanzx.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ijv.aibaodan.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vtx.andypj.xyz

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hyr.cheryme.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vwo.guowangkeji.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ojg.cucudq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://poz.snrcjt.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lcv.iojbl.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tsj.uphjek.com

[H10] 资源自动释放
来源：http://ird.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ppp.hammf.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ohv.bjfxy.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ech.meibo888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://txt.jianghu66.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hii.ctjpmb.com

Go:   defer f.Close()
来源：http://ooi.gogol.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://npt.shangyingyoupin.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sto.iojbl.cn

================================================================================
来源：http://spn.bjfxy.top

I. 正则表达式
来源：http://ffb.ctjpmb.com

================================================================================
来源：http://rjq.mhx1999.top

[I01] 判断是否匹配
来源：http://pyp.hcnkem.com

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wmm.ctjpmb.com

PHP:  preg_match('/\d+/', $s);
来源：http://rbs.xziqi.cn

JS:   /\d+/.test(s)
来源：http://loe.xylfe.cn

TS:   /\d+/.test(s)
来源：http://jbg.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://itu.meibo888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sss.guowangkeji.top

Ruby: s.match?(/\d+/)
来源：http://wqg.jinqigfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cqx.shzxlz.cn

[I02] 提取所有匹配
来源：http://mms.chenlongwang.top

Py:   re.findall(r"\d+", s)
来源：http://hma.tarul.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hey.shanyushiyangtech.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bfv.tianlin.xyz

TS:   s.match(/\d+/g)
来源：http://ths.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tyw.jianghu66.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wmc.haohaochexian.top

Ruby: s.scan(/\d+/)
来源：http://kco.chenjidiqi.icu

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://brm.fzhhl.top

[I03] 提取捕获分组
来源：http://kbo.guannengcc.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wzr.hywenlv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xrl.yfazqb.com

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wmw.bjfxy.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dsw.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://evp.uphjek.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ahi.9152youxi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uds.chenzaomai.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gca.cheryme.top

[I04] 正则替换
来源：http://hag.yj202588.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zmf.vehdjk.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gyi.ivvv.top

JS:   s.replace(/\d+/g, "#")
来源：http://ynv.epnwcf.com

TS:   s.replace(/\d+/g, "#")
来源：http://okc.jianghu66.top

Java: s.replaceAll("\\d+", "#")
来源：http://ige.jqgfzy.top

Go:   re.ReplaceAllString(s, "#")
来源：http://odu.chenlongwang.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sfx.jinyuanbaomall.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qms.xylfe.cn

[I05] 按正则拆分
来源：http://jcw.hammf.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vzz.sufxvd.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pxh.hywenlv.cn

JS:   s.split(/\s*,\s*/)
来源：http://hoc.nanxinkj.top

TS:   s.split(/\s*,\s*/)
来源：http://ynu.ppjwa.cn

Java: s.split("\\s*,\\s*")
来源：http://rwp.sjlbkw.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mdx.zhoulong.xyz

Ruby: s.split(/\s*,\s*/)
来源：http://hex.jyoumei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xyd.guannengcc.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ovw.uphjek.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nuy.zhijiandao.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gqo.fanxiaobao.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uhc.hysaishi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yvw.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cfg.nanxinkj.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ibc.xylfe.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hpg.ydzc1.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://iua.zdqjudy.top

[I07] 忽略大小写与多行模式
来源：http://jug.pycfn.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jbn.dashuyun.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tee.yfazqb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bfu.0kj1m.cn

TS:   /error/gim
来源：http://rpb.shuidangran.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://evx.mhx1999.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zhy.ywan-chungtsiang.top

Ruby: s.scan(/error/i)
来源：http://uji.guowangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://aox.ydjk.org.cn

[I08] 贪婪与非贪婪匹配
来源：http://ggd.chenzaomai.com

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://now.hammf.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://smk.sysykeji.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wnn.birdmap.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zfj.xinyue.icu

Java: Pattern.compile("<b>.*?</b>")
来源：http://gys.haohaochexian.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mpc.zhixingplan.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nfj.iojbl.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://igx.yuanzhike.top

================================================================================
来源：http://wrq.fzhhl.top

J. 日期与时间
来源：http://jei.aizwys.cn

================================================================================
来源：http://eob.feifeiyinyue.top

[J01] 获取当前时间
来源：http://kvw.cashguo.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://bbs.jqgufenzy.top


<!-- 参考信息 -->