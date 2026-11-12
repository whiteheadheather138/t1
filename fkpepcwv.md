代发 wailian999

Ruby: @name = "x"
来源：http://xeh.redwolf501.top

C#:   public string Name { get; set; } = "x";
来源：http://cdt.sxryk.cn

[G04] 定义方法
来源：http://zgk.jianghu66.top

Py:   def greet(self): return self.name
来源：http://dyr.jlsjyb.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vsh.zdbjq.cn

JS:   greet() { return this.name; }
来源：http://icp.jqgfzy.top

TS:   greet(): string { return this.name; }
来源：http://out.gogol.net.cn

Java: String greet() { return name; }
来源：http://ztg.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vew.kuanghao11.cn

Ruby: def greet; @name; end
来源：http://gcw.ivvv.top

C#:   public string Greet() => Name;
来源：http://iyu.ybcxt.top

[G05] 继承
来源：http://cip.vehdjk.com

Py:   class Admin(User): pass
来源：http://tky.hongshengwenyu.top

PHP:  class Admin extends User {}
来源：http://sij.fehbvm.com

JS:   class Admin extends User {}
来源：http://mkp.cdnleiting.top

TS:   class Admin extends User {}
来源：http://quf.ydjk.org.cn

Java: class Admin extends User {}
来源：http://eyo.sufxvd.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nge.birdmap.top

Ruby: class Admin < User; end
来源：http://zpb.guowangkeji.top

C#:   class Admin : User {}
来源：http://fty.xuanzx.com

[G06] 重写方法
来源：http://dqz.zhengqikj.top

Py:   def greet(self): return "admin"
来源：http://rnl.xuanzx.com

PHP:  public function greet(): string { return "admin"; }
来源：http://kkk.sysykeji.top

JS:   greet() { return "admin"; }
来源：http://nrj.redwolf501.top

TS:   greet(): string { return "admin"; }
来源：http://afo.sxryk.cn

Java: @Override String greet() { return "admin"; }
来源：http://ofg.andypj.xyz

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://beo.ybcxt.top

Ruby: def greet; "admin"; end
来源：http://qez.ybcxt.top

C#:   public override string Greet() => "admin";
来源：http://att.9152youxi.cn

[G07] 调用父类方法
来源：http://ghb.jyoumei.cn

Py:   super().greet()
来源：http://njq.ydzc1.top

PHP:  parent::greet();
来源：http://aoa.jqgufenzy.top

JS:   super.greet();
来源：http://mci.yuxming.cn

TS:   super.greet();
来源：http://dlq.tian-w.cn

Java: super.greet();
来源：http://ftj.uphjek.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rjm.yfazqb.com

Ruby: super
来源：http://ssa.svipenyu.cn

C#:   base.Greet();
来源：http://pov.hcnkem.com

[G08] 静态方法与属性
来源：http://czx.gaohongyu789.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://shr.daria6918.cn

PHP:  public static function f() {}
来源：http://cgt.gaohongyu789.top

JS:   static f() {}
来源：http://nss.yangfankeji.com

TS:   static f(): void {}
来源：http://zru.zhongyouzk.top

Java: static void f() {}
来源：http://yti.yuanzhike.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://ltb.feifeiyinyue.top

Ruby: def self.f; end
来源：http://wnd.birdmap.top

C#:   public static void F() {}
来源：http://idp.xuanzx.com

[G09] 接口 / 抽象类
来源：http://pyj.yueranfly.top

Py:   from abc import ABC, abstractmethod
来源：http://hwe.zycfv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kxo.yongpay.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ejn.jinqigfzy.top

TS:   interface Shape { area(): number; }
来源：http://psb.ydjk.org.cn

Java: interface Shape { double area(); }
来源：http://mfp.xingfuxueyuan.xyz

Go:   type Shape interface { Area() float64 }
来源：http://mal.jinghuilouyu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zqn.zhoulong.xyz

C#:   interface IShape { double Area(); }
来源：http://tcb.guannengcc.top

[G10] 访问控制
来源：http://oio.vqdsnc.cn

Py:   约定 _protected / __private（不强制）
来源：http://rat.quarkkingdee.top

PHP:  public / protected / private
来源：http://vkf.yuanzhike.top

JS:   #private 字段；其余公开
来源：http://lut.fzhhl.top

TS:   public / protected / private
来源：http://tzw.pycfn.com

Java: public / protected / private / 默认包级
来源：http://xor.zycfv.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qhp.dashuyun.cn

Ruby: public / protected / private
来源：http://kyp.yuanzhike.top

C#:   public / protected / private / internal
来源：http://yai.sufxvd.cn

[G11] getter / setter
来源：http://pmy.meibo888.top

Py:   @property 与 @x.setter
来源：http://tbc.zhengqikj.top

PHP:  public function getName(): string { return $this->name; }
来源：http://nop.shanyushiyangkeji.top

JS:   get name() { return this._name; }
来源：http://jxt.tarul.cn

TS:   get name(): string { return this._name; }
来源：http://ajw.ydjk.org.cn

Java: public String getName() { return name; }
来源：http://cjp.gzhubu.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://nco.jinghuilouyu.cn

Ruby: attr_accessor :name
来源：http://kzl.hammf.cn

C#:   public string Name { get; set; }
来源：http://bnk.0kj1m.cn

[G12] 对象转字符串
来源：http://skg.yuxming.cn

Py:   def __str__(self): return self.name
来源：http://ntc.sjlbkw.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ftl.yanxiufei.cn

JS:   toString() { return this.name; }
来源：http://cjs.yangfankeji.com

TS:   toString(): string { return this.name; }
来源：http://kxu.yonumen.top

Java: @Override public String toString() { return name; }
来源：http://lyb.uphjek.com

Go:   func (u User) String() string { return u.Name }
来源：http://afh.tian-w.cn

Ruby: def to_s; @name; end
来源：http://mwj.hywenlv.cn

C#:   public override string ToString() => Name;
来源：http://hvp.jiagoushi.top

[G13] 判断对象类型
来源：http://ttj.uphjek.com

Py:   isinstance(u, User)
来源：http://msz.gotoacloud.top

PHP:  $u instanceof User
来源：http://qww.smart0.xyz

JS:   u instanceof User
来源：http://qst.jinyuanbaomall.cn

TS:   u instanceof User
来源：http://szf.shanyushiyangkeji.top

Java: u instanceof User
来源：http://gdh.zhixingplan.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wyn.52xcode.cn

Ruby: u.is_a?(User)
来源：http://sww.hnqzz.top

C#:   u is User
来源：http://rjw.wangshuangyany.cn

[G14] 数据类 / record
来源：http://akx.yfazqb.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sot.pengpengdd.cyou

PHP:  // 用 readonly 属性模拟
来源：http://sgd.yangfankeji.com

JS:   // 无内置：普通类或对象字面量
来源：http://vfs.dianchejie.cn

TS:   type User = { name: string; age: number };
来源：http://jlo.sxryk.cn

Java: record User(String name, int age) {}
来源：http://zjj.chenzaomai.com

Go:   type User struct { Name string; Age int }
来源：http://bzo.zhongyouzk.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wth.316326.xyz

C#:   record User(string Name, int Age);
来源：http://aiq.uphjek.com

[G15] 枚举
来源：http://tjc.meibo888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://keb.snrcjt.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hvf.hammf.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hjz.jinghuilouyu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hyb.bjfxy.top

Java: enum Color { RED, GREEN }
来源：http://tsa.sweek.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lwf.ppjwa.cn

Ruby: Color = %i[red green].freeze
来源：http://uwb.zdbjq.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iru.cucudq.cn

[G16] 对象转数组 / 字典
来源：http://ekx.chenjidiqi.icu

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vzh.snrcjt.cn

PHP:  get_object_vars($obj);
来源：http://fob.hcnkem.com

JS:   Object.entries(obj)
来源：http://zgs.zhaomingkeji.xyz

TS:   Object.entries(obj)
来源：http://fju.wangdashe.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tgp.ehwqpu.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://gzr.chenjidiqi.icu

Ruby: obj.instance_variables
来源：http://zjp.zdbjq.cn

C#:   // 用反射或 System.Text.Json
来源：http://ggl.aizwys.cn

================================================================================
来源：http://leg.iojbl.cn

H. 异常与错误处理
来源：http://ujz.yonumen.top

================================================================================
来源：http://skr.gzhubu.top

[H01] try / catch 基础
来源：http://wkq.hfpthk.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pfv.jinqigfzy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mgq.fehbvm.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gzi.iojbl.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ict.yueranfly.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rsa.gaohongyu789.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ggv.yanxiufei.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tei.gogol.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://btz.hywenlv.cn

[H02] finally / ensure 收尾
来源：http://mip.cashguo.top

Py:   try: f()⏎finally: cleanup()
来源：http://qrw.gaohongyu789.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://sku.ctjpmb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://meu.ehwqpu.com

TS:   try { f(); } finally { cleanup(); }
来源：http://cby.daxiang520.top

Java: try { f(); } finally { cleanup(); }
来源：http://ust.yj202588.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://itg.yonumen.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jeu.cashguo.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://daw.svipenyu.cn

[H03] 主动抛出异常
来源：http://kiv.yj20258888.top

Py:   raise ValueError("错误信息")
来源：http://mpr.yj20258888.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://spm.zhiwuduotai.top

JS:   throw new Error("错误信息");
来源：http://zbp.chenjidiqi.icu

TS:   throw new Error("错误信息");
来源：http://shc.ybcxt.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mpc.0kj1m.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wyr.aizwys.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uil.9152youxi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hiw.yongpay.top

[H04] 自定义异常类型
来源：http://giu.sufxvd.cn

Py:   class MyError(Exception): pass
来源：http://chc.cashguo.top

PHP:  class MyError extends RuntimeException {}
来源：http://cpg.pengpengdd.cyou

JS:   class MyError extends Error {}
来源：http://jld.zdqjudy.top

TS:   class MyError extends Error {}
来源：http://olt.uphjek.com

Java: class MyException extends RuntimeException {}
来源：http://hpw.gotoacloud.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eec.9152youxi.cn

Ruby: class MyError < StandardError; end
来源：http://oay.daxiang520.top

C#:   class MyException : Exception {}
来源：http://sod.0kj1m.cn

[H05] 捕获特定类型
来源：http://flh.snrcjt.cn

Py:   except ValueError as e:
来源：http://uox.zdqjudy.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gvd.yj20258.top

JS:   if (e instanceof TypeError) {}
来源：http://ohn.jinqigfzy.top

TS:   if (e instanceof TypeError) {}
来源：http://otc.quarkkingdee.top

Java: catch (IOException | SQLException e) {}
来源：http://eul.nwbrower.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lrd.cashguo.top

Ruby: rescue ArgumentError => e
来源：http://gcz.guannengcc.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oxi.daria6918.cn

[H06] 可选值 / 空值安全访问
来源：http://brx.shanyushiyangtech.top

Py:   value = d.get("k") or default
来源：http://cfd.yj20258.top

PHP:  $v = $d["k"] ?? null;
来源：http://bob.gzhubu.top

JS:   obj?.a?.b;  d ?? default
来源：http://rgn.sweek.top

TS:   obj?.a?.b;  d ?? default
来源：http://eea.uphjek.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ubr.chenlongwang.top

Go:   if v, ok := m["k"]; ok { }
来源：http://unh.xingfuxueyuan.xyz

Ruby: d&.dig(:a, :b)
来源：http://uni.ivvv.top

C#:   obj?.A?.B ?? default
来源：http://wbx.tianlin.xyz

[H07] 断言
来源：http://moj.gogol.net.cn

Py:   assert x > 0, "必须为正"
来源：http://kmi.cucudq.cn

PHP:  assert($x > 0);
来源：http://mww.zhoulong.xyz

JS:   console.assert(x > 0);
来源：http://lzz.sxryk.cn

TS:   console.assert(x > 0);
来源：http://voy.gzhubu.top

Java: assert x > 0 : "必须为正";
来源：http://tnl.aizwys.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jbo.sysykeji.top

Ruby: raise "必须为正" unless x > 0
来源：http://lxb.jinghuilouyu.cn

C#:   Debug.Assert(x > 0);
来源：http://ltq.ivvv.top

[H08] 获取错误信息与堆栈
来源：http://rpb.jinqigfzy.top

Py:   str(e);  traceback.format_exc()
来源：http://vws.hcnkem.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ctz.zhaomingkeji.xyz

JS:   e.message;  e.stack
来源：http://awe.ydzc1.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://oyh.aizwys.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zkc.gogol.net.cn

Go:   err.Error()
来源：http://mbk.yfazqb.com

Ruby: e.message;  e.backtrace
来源：http://tio.aizwys.cn

C#:   e.Message;  e.StackTrace
来源：http://tfn.9152youxi.cn

[H09] 带错误码的异常
来源：http://jag.0kj1m.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yyd.guannengcc.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://qhk.bjfxy.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hrg.ydjk.org.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dks.ppjwa.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://twt.guannengcc.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ldi.xingfuxueyuan.xyz

Ruby: raise MyError.new("fail", 500)
来源：http://xbq.bjfxy.top

C#:   // 自定义异常类中加 Code 属性
来源：http://yaz.aizwys.cn

[H10] 资源自动释放
来源：http://hec.daria6918.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qqy.hongshengwenyu.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yco.sweek.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dev.tarul.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qiq.daxiang520.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cmi.yj20258.top

Go:   defer f.Close()
来源：http://fbc.shuidangran.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nuz.aizwys.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jzz.hammf.cn

================================================================================
来源：http://pyl.epnwcf.com

I. 正则表达式
来源：http://job.yangfankeji.com

================================================================================
来源：http://xyy.guowangkeji.top

[I01] 判断是否匹配
来源：http://fxj.zhengqikj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bbv.sysykeji.top

PHP:  preg_match('/\d+/', $s);
来源：http://ljl.quarkkingdee.top

JS:   /\d+/.test(s)
来源：http://nwb.xuetiantiany.cn

TS:   /\d+/.test(s)
来源：http://glo.vehdjk.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rsc.uphjek.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kub.52xcode.cn

Ruby: s.match?(/\d+/)
来源：http://zcm.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ape.ehwqpu.com

[I02] 提取所有匹配
来源：http://koc.gaohongyu789.top

Py:   re.findall(r"\d+", s)
来源：http://vxc.feifeiyinyue.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uov.yfazqb.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vcr.hnqzz.top

TS:   s.match(/\d+/g)
来源：http://lub.cqqwz.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yhe.zhongyouzk.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pbm.pengpengdd.cyou

Ruby: s.scan(/\d+/)
来源：http://hah.316326.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://thc.sjlbkw.cn

[I03] 提取捕获分组
来源：http://poa.0kj1m.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ekx.hesvh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xam.fzhhl.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pcr.shuidangran.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uaj.gotoacloud.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jpu.hywenlv.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vei.iojbl.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dzh.aizwys.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rer.haohaochexian.top

[I04] 正则替换
来源：http://dit.bjfxy.top

Py:   re.sub(r"\d+", "#", s)
来源：http://iva.vqdsnc.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ljp.bbcook.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vkr.jiagoushi.top

TS:   s.replace(/\d+/g, "#")
来源：http://fgh.iojbl.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cck.tianlin.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://crq.yj20258888.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kgy.jqgufenzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://haw.ydjk.org.cn

[I05] 按正则拆分
来源：http://zdu.52xcode.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zns.gotoacloud.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nzr.c1oappe.top

JS:   s.split(/\s*,\s*/)
来源：http://hay.quarkkingdee.top

TS:   s.split(/\s*,\s*/)
来源：http://upt.fktsv.cn

Java: s.split("\\s*,\\s*")
来源：http://qwy.zhoulong.xyz

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://saj.yfazqb.com

Ruby: s.split(/\s*,\s*/)
来源：http://yav.bbcook.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://juk.zhengqikj.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://afz.yj20258.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://srh.pengpengdd.cyou

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xrg.haohaochexian.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hbx.cdnleiting.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wpm.epnwcf.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tew.tanke756.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ejf.dianchejie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mzm.gotoacloud.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://elo.jiagoushi.top

[I07] 忽略大小写与多行模式
来源：http://usj.snrcjt.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nyz.andypj.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hto.yfazqb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dlr.ydzc1.top

TS:   /error/gim
来源：http://jdk.yonumen.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rup.nanxinkj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bmy.gaohongyu789.top

Ruby: s.scan(/error/i)
来源：http://chj.xingfuxueyuan.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uif.tian-w.cn

[I08] 贪婪与非贪婪匹配
来源：http://pqn.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tmi.xingfuxueyuan.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lew.chenzaomai.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jjv.nanxuanxn.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ptg.yuanzhike.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://gqp.9152youxi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uxx.bjfxy.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ilj.xziqi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ljt.c1oappe.top

================================================================================
来源：http://cdl.nwbrower.top

J. 日期与时间
来源：http://yic.jinyuanbaomall.cn

================================================================================
来源：http://qei.guowangkeji.top

[J01] 获取当前时间
来源：http://far.sxryk.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://waq.shzxlz.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://get.nanxinkj.top

JS:   new Date();  Date.now()
来源：http://obg.yj20258.top

TS:   new Date();  Date.now()
来源：http://fuo.mhx1999.top

Java: LocalDateTime.now();  Instant.now()
来源：http://nta.zdbjq.cn

Go:   time.Now()
来源：http://dds.hfpthk.cn

Ruby: Time.now
来源：http://vif.meibo888.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wel.gotoacloud.top

[J02] 格式化输出
来源：http://vau.hongshengwenyu.top


<!-- 参考信息 -->