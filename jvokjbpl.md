代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://bvy.fzhhl.top

Ruby: def greet; @name; end
来源：http://dhl.sxryk.cn

C#:   public string Greet() => Name;
来源：http://mld.havefunace.top

[G05] 继承
来源：http://cpx.guowangkeji.top

Py:   class Admin(User): pass
来源：http://uze.chenlongwang.top

PHP:  class Admin extends User {}
来源：http://jpj.smart0.xyz

JS:   class Admin extends User {}
来源：http://wyb.mhx1999.top

TS:   class Admin extends User {}
来源：http://xoa.jinqigufen.top

Java: class Admin extends User {}
来源：http://jze.yangfankeji.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://moa.aizwys.cn

Ruby: class Admin < User; end
来源：http://yqn.zycfv.cn

C#:   class Admin : User {}
来源：http://kve.xinyue.icu

[G06] 重写方法
来源：http://zyb.fengsongda.top

Py:   def greet(self): return "admin"
来源：http://fqr.hongshengwenyu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zio.guowangkeji.top

JS:   greet() { return "admin"; }
来源：http://rvt.shzxlz.cn

TS:   greet(): string { return "admin"; }
来源：http://vks.hammf.cn

Java: @Override String greet() { return "admin"; }
来源：http://vgz.yanxiufei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wgx.yvedp.cn

Ruby: def greet; "admin"; end
来源：http://mna.jinqigufen.top

C#:   public override string Greet() => "admin";
来源：http://qig.vqdsnc.cn

[G07] 调用父类方法
来源：http://ofp.guannengcc.top

Py:   super().greet()
来源：http://uew.hnqzz.top

PHP:  parent::greet();
来源：http://imq.jinqigufen.top

JS:   super.greet();
来源：http://bdt.tianlin.xyz

TS:   super.greet();
来源：http://nry.cashguo.top

Java: super.greet();
来源：http://mrz.yfazqb.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://own.vqdsnc.cn

Ruby: super
来源：http://iud.yonumen.top

C#:   base.Greet();
来源：http://usw.vehdjk.com

[G08] 静态方法与属性
来源：http://iby.tanke756.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yqe.gogol.net.cn

PHP:  public static function f() {}
来源：http://dxa.snrcjt.cn

JS:   static f() {}
来源：http://ure.yonumen.top

TS:   static f(): void {}
来源：http://rsx.sjlbkw.cn

Java: static void f() {}
来源：http://whd.316326.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://ygz.yj20258.top

Ruby: def self.f; end
来源：http://baq.daria6918.cn

C#:   public static void F() {}
来源：http://oor.zdbjq.cn

[G09] 接口 / 抽象类
来源：http://xma.yongpay.top

Py:   from abc import ABC, abstractmethod
来源：http://fry.tianlin.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://rvf.andypj.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://rze.shuidangran.top

TS:   interface Shape { area(): number; }
来源：http://cot.jinqigufen.top

Java: interface Shape { double area(); }
来源：http://oui.shangyingyoupin.top

Go:   type Shape interface { Area() float64 }
来源：http://pve.sweek.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nuw.nanxinkj.top

C#:   interface IShape { double Area(); }
来源：http://vdk.fehbvm.com

[G10] 访问控制
来源：http://ldn.shzxlz.cn

Py:   约定 _protected / __private（不强制）
来源：http://rbu.jyoumei.cn

PHP:  public / protected / private
来源：http://qzh.zhiwuduotai.top

JS:   #private 字段；其余公开
来源：http://nth.ybcxt.top

TS:   public / protected / private
来源：http://why.daria6918.cn

Java: public / protected / private / 默认包级
来源：http://aqt.chenzaomai.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://lum.cqqwz.cn

Ruby: public / protected / private
来源：http://wqx.aizwys.cn

C#:   public / protected / private / internal
来源：http://jfu.sufxvd.cn

[G11] getter / setter
来源：http://xcg.yueranfly.top

Py:   @property 与 @x.setter
来源：http://jhj.cucudq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jeq.daxiang520.top

JS:   get name() { return this._name; }
来源：http://gts.jinqigfzy.top

TS:   get name(): string { return this._name; }
来源：http://dvb.hcnkem.com

Java: public String getName() { return name; }
来源：http://zkw.zhaomingkeji.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://bwr.fktsv.cn

Ruby: attr_accessor :name
来源：http://jhh.zhoulong.xyz

C#:   public string Name { get; set; }
来源：http://rsq.jianghu66.top

[G12] 对象转字符串
来源：http://ojv.dashuyun.cn

Py:   def __str__(self): return self.name
来源：http://fzo.ybcxt.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://qrq.gzhubu.top

JS:   toString() { return this.name; }
来源：http://iaz.gaohongyu789.top

TS:   toString(): string { return this.name; }
来源：http://wnr.shzxlz.cn

Java: @Override public String toString() { return name; }
来源：http://giq.jianghu66.top

Go:   func (u User) String() string { return u.Name }
来源：http://awg.xinyue.icu

Ruby: def to_s; @name; end
来源：http://cuo.sufxvd.cn

C#:   public override string ToString() => Name;
来源：http://ehy.snrcjt.cn

[G13] 判断对象类型
来源：http://yhb.tian-w.cn

Py:   isinstance(u, User)
来源：http://ogu.zhixingplan.top

PHP:  $u instanceof User
来源：http://yrp.yj20258.top

JS:   u instanceof User
来源：http://amc.ivvv.top

TS:   u instanceof User
来源：http://yyq.sysykeji.top

Java: u instanceof User
来源：http://smj.gaohongyu789.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://nxu.xziqi.cn

Ruby: u.is_a?(User)
来源：http://awm.kuanghao11.cn

C#:   u is User
来源：http://lod.kuanghao11.cn

[G14] 数据类 / record
来源：http://nsb.hnqzz.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mdk.zhengqikj.top

PHP:  // 用 readonly 属性模拟
来源：http://joq.ybcxt.top

JS:   // 无内置：普通类或对象字面量
来源：http://woo.hesvh.cn

TS:   type User = { name: string; age: number };
来源：http://btm.zhongyouzk.top

Java: record User(String name, int age) {}
来源：http://wba.iojbl.cn

Go:   type User struct { Name string; Age int }
来源：http://rlj.shangyingyoupin.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://imm.mhx1999.top

C#:   record User(string Name, int Age);
来源：http://uwo.ivvv.top

[G15] 枚举
来源：http://por.zdbjq.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ase.xziqi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hxk.52xcode.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rdh.zhijiandao.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bxs.havefunace.top

Java: enum Color { RED, GREEN }
来源：http://uxa.sjlbkw.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rbh.zhoulong.xyz

Ruby: Color = %i[red green].freeze
来源：http://zaq.0kj1m.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fso.zhixingplan.top

[G16] 对象转数组 / 字典
来源：http://vtv.yfazqb.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mau.52xcode.cn

PHP:  get_object_vars($obj);
来源：http://bhw.zhoulong.xyz

JS:   Object.entries(obj)
来源：http://jsg.chenzaomai.com

TS:   Object.entries(obj)
来源：http://oxw.yangfankeji.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mrx.fanxiaobao.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://apo.hnqzz.top

Ruby: obj.instance_variables
来源：http://gzz.chenzaomai.com

C#:   // 用反射或 System.Text.Json
来源：http://vfl.hesvh.cn

================================================================================
来源：http://zsh.0kj1m.cn

H. 异常与错误处理
来源：http://zmf.snrcjt.cn

================================================================================
来源：http://opt.smart0.xyz

[H01] try / catch 基础
来源：http://hyx.wangshuangyany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oqp.yongpay.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tva.hcnkem.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wtg.yanxiufei.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://aru.guowangkeji.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vwg.9152youxi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fqs.nanxinkj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zoh.ywan-chungtsiang.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xab.zdqjudy.top

[H02] finally / ensure 收尾
来源：http://ctq.yangfankeji.com

Py:   try: f()⏎finally: cleanup()
来源：http://vec.zdqjudy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://gfc.ybcxt.top

JS:   try { f(); } finally { cleanup(); }
来源：http://cyc.sjlbkw.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jzk.hcnkem.com

Java: try { f(); } finally { cleanup(); }
来源：http://hry.jiagoushi.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://tja.hnxiangtu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://jay.zhaomingkeji.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://umf.aibaodan.cn

[H03] 主动抛出异常
来源：http://mte.sjlbkw.cn

Py:   raise ValueError("错误信息")
来源：http://jbs.fktsv.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nzb.yvedp.cn

JS:   throw new Error("错误信息");
来源：http://mrb.gotoacloud.top

TS:   throw new Error("错误信息");
来源：http://mtc.ywan-chungtsiang.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fqs.yj202588.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vbo.zhengqikj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://jji.jqgufenzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://wzz.daria6918.cn

[H04] 自定义异常类型
来源：http://jkb.guannengcc.top

Py:   class MyError(Exception): pass
来源：http://nql.jyoumei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mkp.smart0.xyz

JS:   class MyError extends Error {}
来源：http://hos.zdqjudy.top

TS:   class MyError extends Error {}
来源：http://yaq.ehwqpu.com

Java: class MyException extends RuntimeException {}
来源：http://fyy.mhx1999.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wfr.zdbjq.cn

Ruby: class MyError < StandardError; end
来源：http://uzq.yongpay.top

C#:   class MyException : Exception {}
来源：http://enm.zhaomingkeji.xyz

[H05] 捕获特定类型
来源：http://mcj.nanxuanxn.top

Py:   except ValueError as e:
来源：http://exu.yanxiufei.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wnf.daria6918.cn

JS:   if (e instanceof TypeError) {}
来源：http://anx.jiagoushi.top

TS:   if (e instanceof TypeError) {}
来源：http://xss.guannengcc.top

Java: catch (IOException | SQLException e) {}
来源：http://uxm.jinyuanbaomall.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fpq.xziqi.cn

Ruby: rescue ArgumentError => e
来源：http://fgs.ydzc1.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fce.fengsongda.top

[H06] 可选值 / 空值安全访问
来源：http://vem.zhaomingkeji.xyz

Py:   value = d.get("k") or default
来源：http://esv.tanke756.top

PHP:  $v = $d["k"] ?? null;
来源：http://jcd.nanxuanxn.top

JS:   obj?.a?.b;  d ?? default
来源：http://eoi.zhongyouzk.top

TS:   obj?.a?.b;  d ?? default
来源：http://srg.guannengcc.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sqw.gaohongyu789.top

Go:   if v, ok := m["k"]; ok { }
来源：http://iwk.ybcxt.top

Ruby: d&.dig(:a, :b)
来源：http://fof.yuxming.cn

C#:   obj?.A?.B ?? default
来源：http://zof.chenlongwang.top

[H07] 断言
来源：http://upk.pengpengdd.cyou

Py:   assert x > 0, "必须为正"
来源：http://agj.zycfv.cn

PHP:  assert($x > 0);
来源：http://kgt.cheryme.top

JS:   console.assert(x > 0);
来源：http://jgz.yj20258.top

TS:   console.assert(x > 0);
来源：http://lyr.jlsjyb.cn

Java: assert x > 0 : "必须为正";
来源：http://sou.jinqigufen.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ayf.guannengcc.top

Ruby: raise "必须为正" unless x > 0
来源：http://ika.fktsv.cn

C#:   Debug.Assert(x > 0);
来源：http://uzi.hammf.cn

[H08] 获取错误信息与堆栈
来源：http://ixq.pengpengdd.cyou

Py:   str(e);  traceback.format_exc()
来源：http://vfe.xuanzx.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uxx.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://fkh.smart0.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://mrg.ivvv.top

Java: e.getMessage();  e.printStackTrace()
来源：http://wtb.uphjek.com

Go:   err.Error()
来源：http://ljv.xuanzx.com

Ruby: e.message;  e.backtrace
来源：http://eya.yanxiufei.cn

C#:   e.Message;  e.StackTrace
来源：http://uxz.pengpengdd.cyou

[H09] 带错误码的异常
来源：http://mky.chenzaomai.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://urc.sjlbkw.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hwx.52xcode.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zss.nanxuanxn.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cac.daxiang520.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fod.zdbjq.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rte.jinqigfzy.top

Ruby: raise MyError.new("fail", 500)
来源：http://etf.tarul.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iwj.ehwqpu.com

[H10] 资源自动释放
来源：http://hwd.hesvh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hqh.chenjidiqi.icu

PHP:  // 无 with：在 finally 里 fclose()
来源：http://onq.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oua.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ics.chenzaomai.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mza.snrcjt.cn

Go:   defer f.Close()
来源：http://hzg.zhixingplan.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pnn.quarkkingdee.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pzo.haohaochexian.top

================================================================================
来源：http://wdt.tianlin.xyz

I. 正则表达式
来源：http://xfx.shuidangran.top

================================================================================
来源：http://uxa.hesvh.cn

[I01] 判断是否匹配
来源：http://hja.feifeiyinyue.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fbh.tarul.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qwy.zhijiandao.cn

JS:   /\d+/.test(s)
来源：http://rnd.daxiang520.top

TS:   /\d+/.test(s)
来源：http://kkf.shanyushiyangkeji.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qks.zhengqikj.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tfb.jinghuilouyu.cn

Ruby: s.match?(/\d+/)
来源：http://gix.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gix.shanyushiyangtech.top

[I02] 提取所有匹配
来源：http://gel.andypj.xyz

Py:   re.findall(r"\d+", s)
来源：http://zsk.dashuyun.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ziy.sufxvd.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aml.fktsv.cn

TS:   s.match(/\d+/g)
来源：http://jnq.epnwcf.com

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gzy.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://anj.feifeiyinyue.top

Ruby: s.scan(/\d+/)
来源：http://qoc.bjfxy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yol.ivvv.top

[I03] 提取捕获分组
来源：http://bpo.zdbjq.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sqq.wangshuangyany.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nmn.shzxlz.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://guq.quarkkingdee.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://egm.smart0.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qmm.c1oappe.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sgb.yuxming.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://enn.chenlongwang.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qmo.yvedp.cn

[I04] 正则替换
来源：http://kqv.jinghuilouyu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://euk.yongpay.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mpd.chenjidiqi.icu

JS:   s.replace(/\d+/g, "#")
来源：http://xtl.yfazqb.com

TS:   s.replace(/\d+/g, "#")
来源：http://uxw.wangshuangyany.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cpq.ppjwa.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://puq.zycfv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ueh.jianghu66.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://afw.gotoacloud.top

[I05] 按正则拆分
来源：http://rrh.vehdjk.com

Py:   re.split(r"\s*,\s*", s)
来源：http://hxw.jqgfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jpe.smart0.xyz

JS:   s.split(/\s*,\s*/)
来源：http://twu.chenjidiqi.icu

TS:   s.split(/\s*,\s*/)
来源：http://dic.jinghuilouyu.cn

Java: s.split("\\s*,\\s*")
来源：http://hmu.wangshuangyany.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lrd.haohaochexian.top

Ruby: s.split(/\s*,\s*/)
来源：http://lqq.yangfankeji.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pgb.sxryk.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hbt.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dby.hnxiangtu.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zra.jqgfzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qpd.0kj1m.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pff.yuanzhike.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://smv.tanke756.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://seo.cucudq.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vuz.xziqi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tnp.hnqzz.top

[I07] 忽略大小写与多行模式
来源：http://xkm.fanxiaobao.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hai.chenlongwang.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dsn.fengsongda.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ghs.quarkkingdee.top

TS:   /error/gim
来源：http://bjy.tian-w.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yty.gotoacloud.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nrd.feifeiyinyue.top

Ruby: s.scan(/error/i)
来源：http://hbg.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bmb.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://epw.316326.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mlb.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oqc.yj202588.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tiu.9152youxi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kgt.ppjwa.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jqf.jyoumei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rsf.snrcjt.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qbw.chenlongwang.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vqs.birdmap.top

================================================================================
来源：http://yuy.zycfv.cn

J. 日期与时间
来源：http://myt.cashguo.top

================================================================================
来源：http://zen.zhiwuduotai.top

[J01] 获取当前时间
来源：http://shv.ydjk.org.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://aim.yj20258888.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uex.yj202588.top

JS:   new Date();  Date.now()
来源：http://ppc.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://kcu.pengpengdd.cyou

Java: LocalDateTime.now();  Instant.now()
来源：http://skq.yangfankeji.com

Go:   time.Now()
来源：http://qjn.fzhhl.top

Ruby: Time.now
来源：http://jsr.xuanzx.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iug.wangshuangyany.cn

[J02] 格式化输出
来源：http://dqc.zhongyouzk.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vbr.guannengcc.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hhz.jianghu66.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://key.chenlongwang.top

TS:   d.toISOString()
来源：http://jug.fzhhl.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yxh.jinqigufen.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ujv.zhongyouzk.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cll.mhx1999.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://uhy.ppjwa.cn


<!-- 参考信息 -->