代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://mla.kuanghao11.cn

[G03] 实例属性
来源：http://diq.yuanzhike.top

Py:   self.name = "x"
来源：http://xzp.hnqzz.top

PHP:  public string $name = "x";
来源：http://znp.yanxiufei.cn

JS:   this.name = "x";
来源：http://vtm.zdbjq.cn

TS:   name: string = "x";
来源：http://mzk.zdbjq.cn

Java: private String name;
来源：http://igo.vehdjk.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uuf.jlsjyb.cn

Ruby: @name = "x"
来源：http://qoo.jinghuilouyu.cn

C#:   public string Name { get; set; } = "x";
来源：http://rwt.pengpengdd.cyou

[G04] 定义方法
来源：http://dqt.shanyushiyangkeji.top

Py:   def greet(self): return self.name
来源：http://sdx.yj20258888.top

PHP:  public function greet(): string { return $this->name; }
来源：http://qwm.tanke756.top

JS:   greet() { return this.name; }
来源：http://hec.yongpay.top

TS:   greet(): string { return this.name; }
来源：http://xnk.sjlbkw.cn

Java: String greet() { return name; }
来源：http://dxn.9152youxi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ubv.zycfv.cn

Ruby: def greet; @name; end
来源：http://hwd.guowangkeji.top

C#:   public string Greet() => Name;
来源：http://jrg.ybcxt.top

[G05] 继承
来源：http://gkl.ywan-chungtsiang.top

Py:   class Admin(User): pass
来源：http://ddd.fehbvm.com

PHP:  class Admin extends User {}
来源：http://nfl.yuanzhike.top

JS:   class Admin extends User {}
来源：http://fyf.ybcxt.top

TS:   class Admin extends User {}
来源：http://loa.gotoacloud.top

Java: class Admin extends User {}
来源：http://qkd.yj202588.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wkg.snrcjt.cn

Ruby: class Admin < User; end
来源：http://fot.guannengcc.top

C#:   class Admin : User {}
来源：http://yir.fktsv.cn

[G06] 重写方法
来源：http://age.snrcjt.cn

Py:   def greet(self): return "admin"
来源：http://ros.hammf.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rra.shanyushiyangkeji.top

JS:   greet() { return "admin"; }
来源：http://kvu.jqgfzy.top

TS:   greet(): string { return "admin"; }
来源：http://uak.ydzc1.top

Java: @Override String greet() { return "admin"; }
来源：http://lqz.daria6918.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://evt.0kj1m.cn

Ruby: def greet; "admin"; end
来源：http://fmz.shzxlz.cn

C#:   public override string Greet() => "admin";
来源：http://xor.yuxming.cn

[G07] 调用父类方法
来源：http://izg.zhixingplan.top

Py:   super().greet()
来源：http://tjy.bjfxy.top

PHP:  parent::greet();
来源：http://igq.vehdjk.com

JS:   super.greet();
来源：http://trd.vehdjk.com

TS:   super.greet();
来源：http://nhy.shuidangran.top

Java: super.greet();
来源：http://luf.ppjwa.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rln.shuidangran.top

Ruby: super
来源：http://frq.pengpengdd.cyou

C#:   base.Greet();
来源：http://jpr.yueranfly.top

[G08] 静态方法与属性
来源：http://vtc.yueranfly.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fgo.shangyingyoupin.top

PHP:  public static function f() {}
来源：http://mhj.ydzc1.top

JS:   static f() {}
来源：http://hbb.andypj.xyz

TS:   static f(): void {}
来源：http://wxo.yuanzhike.top

Java: static void f() {}
来源：http://xqo.cheryme.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://oqi.zhoulong.xyz

Ruby: def self.f; end
来源：http://htw.haohaochexian.top

C#:   public static void F() {}
来源：http://cdi.ehwqpu.com

[G09] 接口 / 抽象类
来源：http://jpn.fktsv.cn

Py:   from abc import ABC, abstractmethod
来源：http://fuh.hcnkem.com

PHP:  interface Shape { public function area(): float; }
来源：http://ahj.bbcook.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hlu.epnwcf.com

TS:   interface Shape { area(): number; }
来源：http://kku.zhiwuduotai.top

Java: interface Shape { double area(); }
来源：http://sut.tian-w.cn

Go:   type Shape interface { Area() float64 }
来源：http://rsz.zycfv.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qau.9152youxi.cn

C#:   interface IShape { double Area(); }
来源：http://was.yvedp.cn

[G10] 访问控制
来源：http://tno.yanxiufei.cn

Py:   约定 _protected / __private（不强制）
来源：http://zop.316326.xyz

PHP:  public / protected / private
来源：http://uis.pycfn.com

JS:   #private 字段；其余公开
来源：http://vwk.tarul.cn

TS:   public / protected / private
来源：http://qkw.jiagoushi.top

Java: public / protected / private / 默认包级
来源：http://dui.bbcook.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xja.chenlongwang.top

Ruby: public / protected / private
来源：http://hlk.tanke756.top

C#:   public / protected / private / internal
来源：http://eng.xuetiantiany.cn

[G11] getter / setter
来源：http://azo.tian-w.cn

Py:   @property 与 @x.setter
来源：http://jof.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cog.andypj.xyz

JS:   get name() { return this._name; }
来源：http://hgk.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://oyt.dashuyun.cn

Java: public String getName() { return name; }
来源：http://kjh.yvedp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wkw.xziqi.cn

Ruby: attr_accessor :name
来源：http://aqv.andypj.xyz

C#:   public string Name { get; set; }
来源：http://nxm.cheryme.top

[G12] 对象转字符串
来源：http://hfx.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://qej.feifeiyinyue.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dgd.hongshengwenyu.top

JS:   toString() { return this.name; }
来源：http://zqt.dashuyun.cn

TS:   toString(): string { return this.name; }
来源：http://uog.xuetiantiany.cn

Java: @Override public String toString() { return name; }
来源：http://xjb.birdmap.top

Go:   func (u User) String() string { return u.Name }
来源：http://mew.wangshuangyany.cn

Ruby: def to_s; @name; end
来源：http://coe.chenlongwang.top

C#:   public override string ToString() => Name;
来源：http://quk.tianlin.xyz

[G13] 判断对象类型
来源：http://oil.vqdsnc.cn

Py:   isinstance(u, User)
来源：http://gvk.jlsjyb.cn

PHP:  $u instanceof User
来源：http://haa.jqgfzy.top

JS:   u instanceof User
来源：http://etg.redwolf501.top

TS:   u instanceof User
来源：http://oij.zhiwuduotai.top

Java: u instanceof User
来源：http://gdi.jinghuilouyu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xbb.tanke756.top

Ruby: u.is_a?(User)
来源：http://woe.tanke756.top

C#:   u is User
来源：http://sup.meibo888.top

[G14] 数据类 / record
来源：http://tnm.jinqigufen.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ces.hysaishi.cn

PHP:  // 用 readonly 属性模拟
来源：http://ttq.xziqi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tvw.cheryme.top

TS:   type User = { name: string; age: number };
来源：http://qew.birdmap.top

Java: record User(String name, int age) {}
来源：http://uhr.jyoumei.cn

Go:   type User struct { Name string; Age int }
来源：http://egg.jqgfzy.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fsy.gotoacloud.top

C#:   record User(string Name, int Age);
来源：http://old.52xcode.cn

[G15] 枚举
来源：http://alq.zhengqikj.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wvs.hesvh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qsj.ybcxt.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rzw.chenjidiqi.icu

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jfy.xingfuxueyuan.xyz

Java: enum Color { RED, GREEN }
来源：http://qsw.yuxming.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iex.shuidangran.top

Ruby: Color = %i[red green].freeze
来源：http://bok.yvedp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yta.316326.xyz

[G16] 对象转数组 / 字典
来源：http://yky.dianchejie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qrx.aizwys.cn

PHP:  get_object_vars($obj);
来源：http://qvd.cqqwz.cn

JS:   Object.entries(obj)
来源：http://erv.yj20258.top

TS:   Object.entries(obj)
来源：http://ofe.gzhubu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cxy.bjfxy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://khr.jiagoushi.top

Ruby: obj.instance_variables
来源：http://woe.svipenyu.cn

C#:   // 用反射或 System.Text.Json
来源：http://oip.bbcook.cn

================================================================================
来源：http://fct.ivvv.top

H. 异常与错误处理
来源：http://tjg.jinqigfzy.top

================================================================================
来源：http://yjv.tian-w.cn

[H01] try / catch 基础
来源：http://ihl.uphjek.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jut.cdnleiting.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://oer.zycfv.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hod.ydjk.org.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rsf.bbcook.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vqr.hongshengwenyu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gqh.hywenlv.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://btb.redwolf501.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zfe.tarul.cn

[H02] finally / ensure 收尾
来源：http://ciu.ivvv.top

Py:   try: f()⏎finally: cleanup()
来源：http://ecj.bbcook.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lkz.cdnleiting.top

JS:   try { f(); } finally { cleanup(); }
来源：http://crd.jlsjyb.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yit.ywan-chungtsiang.top

Java: try { f(); } finally { cleanup(); }
来源：http://hye.aibaodan.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kcd.zhoulong.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://ztz.zhengqikj.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://wop.guowangkeji.top

[H03] 主动抛出异常
来源：http://ygt.xylfe.cn

Py:   raise ValueError("错误信息")
来源：http://mkh.nanxuanxn.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ypd.fktsv.cn

JS:   throw new Error("错误信息");
来源：http://bmb.aibaodan.cn

TS:   throw new Error("错误信息");
来源：http://fna.aizwys.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rul.shanyushiyangkeji.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rbs.chenlongwang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zfn.gotoacloud.top

C#:   throw new ArgumentException("错误信息");
来源：http://zsz.yangfankeji.com

[H04] 自定义异常类型
来源：http://lem.yvedp.cn

Py:   class MyError(Exception): pass
来源：http://csk.yongpay.top

PHP:  class MyError extends RuntimeException {}
来源：http://gxa.xingfuxueyuan.xyz

JS:   class MyError extends Error {}
来源：http://wsf.kuanghao11.cn

TS:   class MyError extends Error {}
来源：http://vgr.xylfe.cn

Java: class MyException extends RuntimeException {}
来源：http://drg.fzhhl.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xdu.tian-w.cn

Ruby: class MyError < StandardError; end
来源：http://neh.yj202588.top

C#:   class MyException : Exception {}
来源：http://gjs.zdbjq.cn

[H05] 捕获特定类型
来源：http://lqq.hywenlv.cn

Py:   except ValueError as e:
来源：http://sue.nanxuanxn.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://het.fengsongda.top

JS:   if (e instanceof TypeError) {}
来源：http://mcu.nwbrower.top

TS:   if (e instanceof TypeError) {}
来源：http://bnv.ppjwa.cn

Java: catch (IOException | SQLException e) {}
来源：http://bqy.jiagoushi.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sup.tarul.cn

Ruby: rescue ArgumentError => e
来源：http://tis.cheryme.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hfh.zycfv.cn

[H06] 可选值 / 空值安全访问
来源：http://ncj.yonumen.top

Py:   value = d.get("k") or default
来源：http://gnq.jinqigfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://byk.gogol.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ozz.yuxming.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ndc.jiagoushi.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nbl.tian-w.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xuf.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://vzi.zhongyouzk.top

C#:   obj?.A?.B ?? default
来源：http://ksb.zhoulong.xyz

[H07] 断言
来源：http://xof.yj20258888.top

Py:   assert x > 0, "必须为正"
来源：http://iph.0kj1m.cn

PHP:  assert($x > 0);
来源：http://ksr.wangdashe.top

JS:   console.assert(x > 0);
来源：http://qix.tanke756.top

TS:   console.assert(x > 0);
来源：http://ftn.shuidangran.top

Java: assert x > 0 : "必须为正";
来源：http://lgs.xingfuxueyuan.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://teo.sjlbkw.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dyz.redwolf501.top

C#:   Debug.Assert(x > 0);
来源：http://mqv.hongshengwenyu.top

[H08] 获取错误信息与堆栈
来源：http://oga.wangshuangyany.cn

Py:   str(e);  traceback.format_exc()
来源：http://jwl.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://apj.shuidangran.top

JS:   e.message;  e.stack
来源：http://hur.guowangkeji.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://lgt.0kj1m.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jwf.yj20258.top

Go:   err.Error()
来源：http://lpg.jinghuilouyu.cn

Ruby: e.message;  e.backtrace
来源：http://ucl.xylfe.cn

C#:   e.Message;  e.StackTrace
来源：http://dry.dashuyun.cn

[H09] 带错误码的异常
来源：http://cmm.ydjk.org.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bzz.tanke756.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://sni.52xcode.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://onc.pycfn.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://air.xingfuxueyuan.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nep.nanxuanxn.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://luw.ydzc1.top

Ruby: raise MyError.new("fail", 500)
来源：http://wfe.hysaishi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ttf.cashguo.top

[H10] 资源自动释放
来源：http://kvx.sweek.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://ytu.cashguo.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nns.daria6918.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vhe.pengpengdd.cyou

TS:   // 无 with：在 finally 里关闭句柄
来源：http://crw.hfpthk.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qyz.sxryk.cn

Go:   defer f.Close()
来源：http://lyu.yanxiufei.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nln.fengsongda.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bop.quarkkingdee.top

================================================================================
来源：http://xbu.aibaodan.cn

I. 正则表达式
来源：http://fiu.yueranfly.top

================================================================================
来源：http://nqt.xinyue.icu

[I01] 判断是否匹配
来源：http://bfn.yj20258888.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://laf.zdbjq.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bbh.tanke756.top

JS:   /\d+/.test(s)
来源：http://guk.meibo888.top

TS:   /\d+/.test(s)
来源：http://flj.yj20258888.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ntp.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://etd.hnqzz.top

Ruby: s.match?(/\d+/)
来源：http://ajh.yvedp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://prq.smart0.xyz

[I02] 提取所有匹配
来源：http://sqo.sufxvd.cn

Py:   re.findall(r"\d+", s)
来源：http://qnv.jianghu66.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zyv.zycfv.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sst.shanyushiyangtech.top

TS:   s.match(/\d+/g)
来源：http://plv.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ifg.xuetiantiany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qxw.chenlongwang.top

Ruby: s.scan(/\d+/)
来源：http://ugx.nwbrower.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fet.kuanghao11.cn

[I03] 提取捕获分组
来源：http://vaw.9152youxi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://unz.birdmap.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fae.yuxming.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://apo.yangfankeji.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://buo.mhx1999.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dhk.quarkkingdee.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ewf.feifeiyinyue.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xuv.hongshengwenyu.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jsm.zhijiandao.cn

[I04] 正则替换
来源：http://fkx.yueranfly.top

Py:   re.sub(r"\d+", "#", s)
来源：http://dek.haohaochexian.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bbs.ehwqpu.com

JS:   s.replace(/\d+/g, "#")
来源：http://taq.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lxw.ctjpmb.com

Java: s.replaceAll("\\d+", "#")
来源：http://iyt.feifeiyinyue.top

Go:   re.ReplaceAllString(s, "#")
来源：http://thq.shanyushiyangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jjg.yj202588.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rah.xinyue.icu

[I05] 按正则拆分
来源：http://xwu.iojbl.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qff.c1oappe.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yze.52xcode.cn

JS:   s.split(/\s*,\s*/)
来源：http://opk.tian-w.cn

TS:   s.split(/\s*,\s*/)
来源：http://pkd.hesvh.cn

Java: s.split("\\s*,\\s*")
来源：http://cqu.shzxlz.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zjd.yfazqb.com

Ruby: s.split(/\s*,\s*/)
来源：http://rrc.ydzc1.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kir.birdmap.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ccb.jinghuilouyu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ywq.pycfn.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://aew.tanke756.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://exc.shuidangran.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lbu.fktsv.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hjw.hesvh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nqg.yfazqb.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zfv.ivvv.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mft.meibo888.top

[I07] 忽略大小写与多行模式
来源：http://zcr.cdnleiting.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qnt.jqgufenzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ztx.jqgfzy.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lrf.snrcjt.cn

TS:   /error/gim
来源：http://qjm.aibaodan.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dij.xylfe.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kmi.yj202588.top

Ruby: s.scan(/error/i)
来源：http://qbj.smart0.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://joh.andypj.xyz

[I08] 贪婪与非贪婪匹配
来源：http://gqi.cqqwz.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nmg.nwbrower.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zfg.guannengcc.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xre.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zhg.sjlbkw.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wry.jiagoushi.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://chu.xuetiantiany.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ojs.snrcjt.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ifk.xziqi.cn

================================================================================
来源：http://wpt.0kj1m.cn

J. 日期与时间
来源：http://gmk.yongpay.top

================================================================================
来源：http://ssz.guowangkeji.top

[J01] 获取当前时间
来源：http://rnq.gotoacloud.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://sfu.hnqzz.top


<!-- 参考信息 -->