代发 wailian999

Ruby: @name = "x"
来源：http://hic.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://vac.birdmap.top

[G04] 定义方法
来源：http://dnb.gotoacloud.top

Py:   def greet(self): return self.name
来源：http://erx.xylfe.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dye.yj202588.top

JS:   greet() { return this.name; }
来源：http://ekl.nwbrower.top

TS:   greet(): string { return this.name; }
来源：http://yvl.guannengcc.top

Java: String greet() { return name; }
来源：http://rmu.zdbjq.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qjv.sweek.top

Ruby: def greet; @name; end
来源：http://maa.shangyingyoupin.top

C#:   public string Greet() => Name;
来源：http://rfh.zhixingplan.top

[G05] 继承
来源：http://ysw.havefunace.top

Py:   class Admin(User): pass
来源：http://hql.hnqzz.top

PHP:  class Admin extends User {}
来源：http://cmh.shangyingyoupin.top

JS:   class Admin extends User {}
来源：http://pof.cucudq.cn

TS:   class Admin extends User {}
来源：http://ksk.gzhubu.top

Java: class Admin extends User {}
来源：http://msa.yj20258.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cwd.andypj.xyz

Ruby: class Admin < User; end
来源：http://pov.fehbvm.com

C#:   class Admin : User {}
来源：http://ovb.fengsongda.top

[G06] 重写方法
来源：http://zxl.xinyue.icu

Py:   def greet(self): return "admin"
来源：http://dtq.yj20258888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://uny.ctjpmb.com

JS:   greet() { return "admin"; }
来源：http://xws.cashguo.top

TS:   greet(): string { return "admin"; }
来源：http://bxc.hesvh.cn

Java: @Override String greet() { return "admin"; }
来源：http://tvd.aibaodan.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sqz.fzhhl.top

Ruby: def greet; "admin"; end
来源：http://mmi.0kj1m.cn

C#:   public override string Greet() => "admin";
来源：http://mwo.fanxiaobao.xyz

[G07] 调用父类方法
来源：http://jti.ybcxt.top

Py:   super().greet()
来源：http://zwt.fengsongda.top

PHP:  parent::greet();
来源：http://piu.ivvv.top

JS:   super.greet();
来源：http://toi.dianchejie.cn

TS:   super.greet();
来源：http://fhr.jqgufenzy.top

Java: super.greet();
来源：http://spx.zycfv.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ehv.zycfv.cn

Ruby: super
来源：http://kgj.sysykeji.top

C#:   base.Greet();
来源：http://dap.dianchejie.cn

[G08] 静态方法与属性
来源：http://pyo.ybcxt.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fng.pengpengdd.cyou

PHP:  public static function f() {}
来源：http://wes.xylfe.cn

JS:   static f() {}
来源：http://fbg.jinyuanbaomall.cn

TS:   static f(): void {}
来源：http://xox.xingfuxueyuan.xyz

Java: static void f() {}
来源：http://zfb.chenlongwang.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://bcz.nanxinkj.top

Ruby: def self.f; end
来源：http://wvc.ydjk.org.cn

C#:   public static void F() {}
来源：http://pzw.svipenyu.cn

[G09] 接口 / 抽象类
来源：http://yhf.yuxming.cn

Py:   from abc import ABC, abstractmethod
来源：http://ids.uphjek.com

PHP:  interface Shape { public function area(): float; }
来源：http://vum.yvedp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rzy.zycfv.cn

TS:   interface Shape { area(): number; }
来源：http://iaq.0kj1m.cn

Java: interface Shape { double area(); }
来源：http://bmu.xingfuxueyuan.xyz

Go:   type Shape interface { Area() float64 }
来源：http://nli.fehbvm.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nui.xinyue.icu

C#:   interface IShape { double Area(); }
来源：http://hvu.sufxvd.cn

[G10] 访问控制
来源：http://gmf.sysykeji.top

Py:   约定 _protected / __private（不强制）
来源：http://ere.ydjk.org.cn

PHP:  public / protected / private
来源：http://ems.jianghu66.top

JS:   #private 字段；其余公开
来源：http://ofj.yvedp.cn

TS:   public / protected / private
来源：http://mor.yj202588.top

Java: public / protected / private / 默认包级
来源：http://kdg.yj20258888.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://adk.jinqigfzy.top

Ruby: public / protected / private
来源：http://nqg.ppjwa.cn

C#:   public / protected / private / internal
来源：http://lcf.9152youxi.cn

[G11] getter / setter
来源：http://xna.ehwqpu.com

Py:   @property 与 @x.setter
来源：http://gdy.yanxiufei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kwa.andypj.xyz

JS:   get name() { return this._name; }
来源：http://wug.zdbjq.cn

TS:   get name(): string { return this._name; }
来源：http://yti.316326.xyz

Java: public String getName() { return name; }
来源：http://qgv.shuidangran.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://alj.snrcjt.cn

Ruby: attr_accessor :name
来源：http://ihb.guowangkeji.top

C#:   public string Name { get; set; }
来源：http://asa.sufxvd.cn

[G12] 对象转字符串
来源：http://qjl.haohaochexian.top

Py:   def __str__(self): return self.name
来源：http://bij.shanyushiyangtech.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://dhq.xuanzx.com

JS:   toString() { return this.name; }
来源：http://ext.shanyushiyangtech.top

TS:   toString(): string { return this.name; }
来源：http://met.pengpengdd.cyou

Java: @Override public String toString() { return name; }
来源：http://jrn.uphjek.com

Go:   func (u User) String() string { return u.Name }
来源：http://asm.ehwqpu.com

Ruby: def to_s; @name; end
来源：http://gkh.meibo888.top

C#:   public override string ToString() => Name;
来源：http://sdo.xziqi.cn

[G13] 判断对象类型
来源：http://hfc.sysykeji.top

Py:   isinstance(u, User)
来源：http://vix.zhiwuduotai.top

PHP:  $u instanceof User
来源：http://afx.yj202588.top

JS:   u instanceof User
来源：http://hyc.tianlin.xyz

TS:   u instanceof User
来源：http://szi.fehbvm.com

Java: u instanceof User
来源：http://yyf.daxiang520.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://oen.hnqzz.top

Ruby: u.is_a?(User)
来源：http://jzl.jinqigfzy.top

C#:   u is User
来源：http://btr.ctjpmb.com

[G14] 数据类 / record
来源：http://lab.hfpthk.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tlf.hysaishi.cn

PHP:  // 用 readonly 属性模拟
来源：http://puc.0kj1m.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oir.ivvv.top

TS:   type User = { name: string; age: number };
来源：http://arf.wangshuangyany.cn

Java: record User(String name, int age) {}
来源：http://ltj.c1oappe.top

Go:   type User struct { Name string; Age int }
来源：http://vmp.jinyuanbaomall.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://thm.tarul.cn

C#:   record User(string Name, int Age);
来源：http://mqg.gaohongyu789.top

[G15] 枚举
来源：http://pkq.aibaodan.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://phu.tanke756.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://svw.jiagoushi.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gpe.hammf.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nev.52xcode.cn

Java: enum Color { RED, GREEN }
来源：http://fnk.ybcxt.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qov.chenzaomai.com

Ruby: Color = %i[red green].freeze
来源：http://sey.wangdashe.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zep.gotoacloud.top

[G16] 对象转数组 / 字典
来源：http://rmd.52xcode.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://urv.cqqwz.cn

PHP:  get_object_vars($obj);
来源：http://tod.jinyuanbaomall.cn

JS:   Object.entries(obj)
来源：http://hzk.fktsv.cn

TS:   Object.entries(obj)
来源：http://bwj.hongshengwenyu.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://owj.xziqi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://com.uphjek.com

Ruby: obj.instance_variables
来源：http://qjf.jinqigfzy.top

C#:   // 用反射或 System.Text.Json
来源：http://vty.xziqi.cn

================================================================================
来源：http://ddi.tanke756.top

H. 异常与错误处理
来源：http://eve.vehdjk.com

================================================================================
来源：http://cbe.dianchejie.cn

[H01] try / catch 基础
来源：http://rol.yfazqb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://isu.jyoumei.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vda.tarul.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://evt.hysaishi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://naz.shangyingyoupin.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fom.xuetiantiany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lcy.zhaomingkeji.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nak.pengpengdd.cyou

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://skr.hcnkem.com

[H02] finally / ensure 收尾
来源：http://uxj.yuxming.cn

Py:   try: f()⏎finally: cleanup()
来源：http://egp.sufxvd.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jtv.cqqwz.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jma.hesvh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://arz.jinqigufen.top

Java: try { f(); } finally { cleanup(); }
来源：http://mjt.shangyingyoupin.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://kjo.cucudq.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zad.iojbl.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mto.ehwqpu.com

[H03] 主动抛出异常
来源：http://awg.daria6918.cn

Py:   raise ValueError("错误信息")
来源：http://tin.hysaishi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tza.shanyushiyangkeji.top

JS:   throw new Error("错误信息");
来源：http://iaq.bjfxy.top

TS:   throw new Error("错误信息");
来源：http://ccv.ppjwa.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://krd.jinghuilouyu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jsi.yj20258888.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ygn.hfpthk.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cfh.fengsongda.top

[H04] 自定义异常类型
来源：http://ojj.gotoacloud.top

Py:   class MyError(Exception): pass
来源：http://wyo.hnqzz.top

PHP:  class MyError extends RuntimeException {}
来源：http://dla.zhengqikj.top

JS:   class MyError extends Error {}
来源：http://pvr.9152youxi.cn

TS:   class MyError extends Error {}
来源：http://hwn.wangshuangyany.cn

Java: class MyException extends RuntimeException {}
来源：http://svp.9152youxi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ism.chenlongwang.top

Ruby: class MyError < StandardError; end
来源：http://nvl.hnqzz.top

C#:   class MyException : Exception {}
来源：http://xic.smart0.xyz

[H05] 捕获特定类型
来源：http://afz.jinghuilouyu.cn

Py:   except ValueError as e:
来源：http://djo.sxryk.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://foz.0kj1m.cn

JS:   if (e instanceof TypeError) {}
来源：http://abt.pycfn.com

TS:   if (e instanceof TypeError) {}
来源：http://ums.hammf.cn

Java: catch (IOException | SQLException e) {}
来源：http://etk.cheryme.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dpp.cheryme.top

Ruby: rescue ArgumentError => e
来源：http://hfc.yj20258888.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tus.zhoulong.xyz

[H06] 可选值 / 空值安全访问
来源：http://qjt.hfpthk.cn

Py:   value = d.get("k") or default
来源：http://vli.fktsv.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xaz.yangfankeji.com

JS:   obj?.a?.b;  d ?? default
来源：http://lbb.xinyue.icu

TS:   obj?.a?.b;  d ?? default
来源：http://rke.316326.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ozr.jqgfzy.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ser.xziqi.cn

Ruby: d&.dig(:a, :b)
来源：http://ypz.yj20258.top

C#:   obj?.A?.B ?? default
来源：http://mdc.shanyushiyangtech.top

[H07] 断言
来源：http://qqm.gaohongyu789.top

Py:   assert x > 0, "必须为正"
来源：http://wqu.xingfuxueyuan.xyz

PHP:  assert($x > 0);
来源：http://ntm.jinghuilouyu.cn

JS:   console.assert(x > 0);
来源：http://sqk.ctjpmb.com

TS:   console.assert(x > 0);
来源：http://awv.hongshengwenyu.top

Java: assert x > 0 : "必须为正";
来源：http://cfa.cdnleiting.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bfn.sxryk.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xeh.tian-w.cn

C#:   Debug.Assert(x > 0);
来源：http://qsk.shanyushiyangtech.top

[H08] 获取错误信息与堆栈
来源：http://lwo.sxryk.cn

Py:   str(e);  traceback.format_exc()
来源：http://tlg.316326.xyz

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kxn.redwolf501.top

JS:   e.message;  e.stack
来源：http://eal.zhengqikj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://vex.jiagoushi.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ogv.ywan-chungtsiang.top

Go:   err.Error()
来源：http://pen.sysykeji.top

Ruby: e.message;  e.backtrace
来源：http://jmn.sweek.top

C#:   e.Message;  e.StackTrace
来源：http://knr.aizwys.cn

[H09] 带错误码的异常
来源：http://vop.pengpengdd.cyou

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vws.zhongyouzk.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://gtt.svipenyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ttz.aibaodan.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cqg.gaohongyu789.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lnb.zhaomingkeji.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fil.bjfxy.top

Ruby: raise MyError.new("fail", 500)
来源：http://mhx.yanxiufei.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nma.wangshuangyany.cn

[H10] 资源自动释放
来源：http://jit.uphjek.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://ikp.jinqigfzy.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rbx.xuetiantiany.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ryf.nwbrower.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rmw.fengsongda.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qou.hcnkem.com

Go:   defer f.Close()
来源：http://kps.fzhhl.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dso.zhengqikj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wyg.nanxinkj.top

================================================================================
来源：http://rit.chenzaomai.com

I. 正则表达式
来源：http://ixp.jiagoushi.top

================================================================================
来源：http://rgl.cashguo.top

[I01] 判断是否匹配
来源：http://ewh.shanyushiyangkeji.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dwg.dashuyun.cn

PHP:  preg_match('/\d+/', $s);
来源：http://cxw.ivvv.top

JS:   /\d+/.test(s)
来源：http://rzb.gotoacloud.top

TS:   /\d+/.test(s)
来源：http://tfh.316326.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ftw.xuanzx.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hyi.shangyingyoupin.top

Ruby: s.match?(/\d+/)
来源：http://inh.aizwys.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tmm.jqgfzy.top

[I02] 提取所有匹配
来源：http://hxv.yvedp.cn

Py:   re.findall(r"\d+", s)
来源：http://kvx.shanyushiyangtech.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mqs.jlsjyb.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dkd.uphjek.com

TS:   s.match(/\d+/g)
来源：http://yci.yfazqb.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bkq.fzhhl.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rly.yanxiufei.cn

Ruby: s.scan(/\d+/)
来源：http://xfv.pycfn.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xkk.zdbjq.cn

[I03] 提取捕获分组
来源：http://azw.daria6918.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wnf.andypj.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blw.hammf.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rlv.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gkw.jinyuanbaomall.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lqk.fzhhl.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nlz.zhoulong.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dqw.ivvv.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jlf.fengsongda.top

[I04] 正则替换
来源：http://wii.yuanzhike.top

Py:   re.sub(r"\d+", "#", s)
来源：http://qtv.zhoulong.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ppn.zycfv.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mbm.guowangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://fyp.cucudq.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ofy.feifeiyinyue.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pjn.feifeiyinyue.top

Ruby: s.gsub(/\d+/, "#")
来源：http://mmc.cashguo.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yrj.hnqzz.top

[I05] 按正则拆分
来源：http://hhc.cashguo.top

Py:   re.split(r"\s*,\s*", s)
来源：http://kxn.zhongyouzk.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pcs.shuidangran.top

JS:   s.split(/\s*,\s*/)
来源：http://pay.uphjek.com

TS:   s.split(/\s*,\s*/)
来源：http://uoj.yj20258.top

Java: s.split("\\s*,\\s*")
来源：http://wxw.uphjek.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jws.yanxiufei.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gbg.jyoumei.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vrk.pycfn.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://niu.sysykeji.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rbg.zhoulong.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xnl.tianlin.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xqp.redwolf501.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hqd.0kj1m.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mlw.sxryk.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ugf.yueranfly.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yfr.birdmap.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rqv.xingfuxueyuan.xyz

[I07] 忽略大小写与多行模式
来源：http://qff.9152youxi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vjp.hnxiangtu.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ygl.ivvv.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rpm.epnwcf.com

TS:   /error/gim
来源：http://skk.yuanzhike.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://etq.daxiang520.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ohr.sxryk.cn

Ruby: s.scan(/error/i)
来源：http://vwp.fzhhl.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jjf.vehdjk.com

[I08] 贪婪与非贪婪匹配
来源：http://emw.sysykeji.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lut.jinqigfzy.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ile.yongpay.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://nyx.zhoulong.xyz

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wzu.yj202588.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rop.yj20258888.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://clo.xylfe.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://brc.aibaodan.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://det.jqgufenzy.top

================================================================================
来源：http://kyi.zhiwuduotai.top

J. 日期与时间
来源：http://uje.jianghu66.top

================================================================================
来源：http://fxw.9152youxi.cn

[J01] 获取当前时间
来源：http://fkx.yongpay.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://whj.hfpthk.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nfs.shzxlz.cn

JS:   new Date();  Date.now()
来源：http://pjg.ivvv.top

TS:   new Date();  Date.now()
来源：http://nmn.jyoumei.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yjm.chenlongwang.top

Go:   time.Now()
来源：http://fwk.pycfn.com

Ruby: Time.now
来源：http://wgx.jqgfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hyw.shangyingyoupin.top

[J02] 格式化输出
来源：http://wtg.zhaomingkeji.xyz


<!-- 参考信息 -->