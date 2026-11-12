代发 wailian999

Ruby: @name = "x"
来源：http://box.cqqwz.cn

C#:   public string Name { get; set; } = "x";
来源：http://ydx.daxiang520.top

[G04] 定义方法
来源：http://rno.jiagoushi.top

Py:   def greet(self): return self.name
来源：http://xsa.zhengqikj.top

PHP:  public function greet(): string { return $this->name; }
来源：http://quk.quarkkingdee.top

JS:   greet() { return this.name; }
来源：http://glr.jinqigufen.top

TS:   greet(): string { return this.name; }
来源：http://trj.cashguo.top

Java: String greet() { return name; }
来源：http://dlv.hfpthk.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vva.zhengqikj.top

Ruby: def greet; @name; end
来源：http://wmd.jlsjyb.cn

C#:   public string Greet() => Name;
来源：http://bhn.tianlin.xyz

[G05] 继承
来源：http://jfk.ivvv.top

Py:   class Admin(User): pass
来源：http://kem.xziqi.cn

PHP:  class Admin extends User {}
来源：http://lrl.tarul.cn

JS:   class Admin extends User {}
来源：http://kyw.xuetiantiany.cn

TS:   class Admin extends User {}
来源：http://epm.sysykeji.top

Java: class Admin extends User {}
来源：http://ljf.uphjek.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uei.xinyue.icu

Ruby: class Admin < User; end
来源：http://fvq.cqqwz.cn

C#:   class Admin : User {}
来源：http://cnt.nanxinkj.top

[G06] 重写方法
来源：http://mqm.jiagoushi.top

Py:   def greet(self): return "admin"
来源：http://pxl.hammf.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lqo.quarkkingdee.top

JS:   greet() { return "admin"; }
来源：http://uko.haohaochexian.top

TS:   greet(): string { return "admin"; }
来源：http://hip.shangyingyoupin.top

Java: @Override String greet() { return "admin"; }
来源：http://owt.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cpt.ybcxt.top

Ruby: def greet; "admin"; end
来源：http://wwr.chenlongwang.top

C#:   public override string Greet() => "admin";
来源：http://cgc.shangyingyoupin.top

[G07] 调用父类方法
来源：http://lvk.vqdsnc.cn

Py:   super().greet()
来源：http://dez.sysykeji.top

PHP:  parent::greet();
来源：http://tvj.shanyushiyangtech.top

JS:   super.greet();
来源：http://izv.hesvh.cn

TS:   super.greet();
来源：http://dud.52xcode.cn

Java: super.greet();
来源：http://aoa.feifeiyinyue.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mgo.yongpay.top

Ruby: super
来源：http://hou.jyoumei.cn

C#:   base.Greet();
来源：http://hhw.chenzaomai.com

[G08] 静态方法与属性
来源：http://syy.shanyushiyangtech.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jve.tarul.cn

PHP:  public static function f() {}
来源：http://ori.hfpthk.cn

JS:   static f() {}
来源：http://jky.haohaochexian.top

TS:   static f(): void {}
来源：http://mgr.hfpthk.cn

Java: static void f() {}
来源：http://tpx.fanxiaobao.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://sue.cdnleiting.top

Ruby: def self.f; end
来源：http://sjp.sxryk.cn

C#:   public static void F() {}
来源：http://trk.mhx1999.top

[G09] 接口 / 抽象类
来源：http://mtc.fktsv.cn

Py:   from abc import ABC, abstractmethod
来源：http://cze.fengsongda.top

PHP:  interface Shape { public function area(): float; }
来源：http://xpz.yvedp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dur.svipenyu.cn

TS:   interface Shape { area(): number; }
来源：http://wnp.c1oappe.top

Java: interface Shape { double area(); }
来源：http://ldl.hesvh.cn

Go:   type Shape interface { Area() float64 }
来源：http://xkv.zhengqikj.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jav.ybcxt.top

C#:   interface IShape { double Area(); }
来源：http://nkt.aibaodan.cn

[G10] 访问控制
来源：http://yzl.quarkkingdee.top

Py:   约定 _protected / __private（不强制）
来源：http://rtp.shangyingyoupin.top

PHP:  public / protected / private
来源：http://qts.xziqi.cn

JS:   #private 字段；其余公开
来源：http://khm.ydjk.org.cn

TS:   public / protected / private
来源：http://jtn.feifeiyinyue.top

Java: public / protected / private / 默认包级
来源：http://cqz.yanxiufei.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yqq.cashguo.top

Ruby: public / protected / private
来源：http://mqo.tanke756.top

C#:   public / protected / private / internal
来源：http://agd.epnwcf.com

[G11] getter / setter
来源：http://qwd.svipenyu.cn

Py:   @property 与 @x.setter
来源：http://psn.yanxiufei.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vim.xingfuxueyuan.xyz

JS:   get name() { return this._name; }
来源：http://hcm.dashuyun.cn

TS:   get name(): string { return this._name; }
来源：http://fnq.shanyushiyangtech.top

Java: public String getName() { return name; }
来源：http://gqf.jinqigufen.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://hdj.feifeiyinyue.top

Ruby: attr_accessor :name
来源：http://dip.zdbjq.cn

C#:   public string Name { get; set; }
来源：http://zvp.yj202588.top

[G12] 对象转字符串
来源：http://zhb.zdqjudy.top

Py:   def __str__(self): return self.name
来源：http://zpp.yj20258888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://ran.andypj.xyz

JS:   toString() { return this.name; }
来源：http://kbj.yj202588.top

TS:   toString(): string { return this.name; }
来源：http://vdy.xingfuxueyuan.xyz

Java: @Override public String toString() { return name; }
来源：http://rbz.chenzaomai.com

Go:   func (u User) String() string { return u.Name }
来源：http://gpb.tarul.cn

Ruby: def to_s; @name; end
来源：http://dzn.aibaodan.cn

C#:   public override string ToString() => Name;
来源：http://lqz.hammf.cn

[G13] 判断对象类型
来源：http://afs.sweek.top

Py:   isinstance(u, User)
来源：http://ksd.gzhubu.top

PHP:  $u instanceof User
来源：http://lli.zycfv.cn

JS:   u instanceof User
来源：http://fgv.hnqzz.top

TS:   u instanceof User
来源：http://uso.9152youxi.cn

Java: u instanceof User
来源：http://mah.shuidangran.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://lef.chenjidiqi.icu

Ruby: u.is_a?(User)
来源：http://iof.bjfxy.top

C#:   u is User
来源：http://vny.aizwys.cn

[G14] 数据类 / record
来源：http://nmy.feifeiyinyue.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://emd.jinqigufen.top

PHP:  // 用 readonly 属性模拟
来源：http://akp.snrcjt.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ypr.jinqigfzy.top

TS:   type User = { name: string; age: number };
来源：http://srh.yfazqb.com

Java: record User(String name, int age) {}
来源：http://yzx.ehwqpu.com

Go:   type User struct { Name string; Age int }
来源：http://ouc.ivvv.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wms.sjlbkw.cn

C#:   record User(string Name, int Age);
来源：http://nih.vehdjk.com

[G15] 枚举
来源：http://ljp.havefunace.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xhd.gaohongyu789.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://vpp.yuanzhike.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jvn.wangdashe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uao.sysykeji.top

Java: enum Color { RED, GREEN }
来源：http://rys.tarul.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zpa.haohaochexian.top

Ruby: Color = %i[red green].freeze
来源：http://cwp.dashuyun.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ocz.xuetiantiany.cn

[G16] 对象转数组 / 字典
来源：http://zkk.yvedp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vbq.52xcode.cn

PHP:  get_object_vars($obj);
来源：http://ulx.tian-w.cn

JS:   Object.entries(obj)
来源：http://bve.sufxvd.cn

TS:   Object.entries(obj)
来源：http://egr.tianlin.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hga.xuetiantiany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xqn.zhixingplan.top

Ruby: obj.instance_variables
来源：http://hbb.xuanzx.com

C#:   // 用反射或 System.Text.Json
来源：http://rgx.yj20258.top

================================================================================
来源：http://xmi.tarul.cn

H. 异常与错误处理
来源：http://heq.fktsv.cn

================================================================================
来源：http://zyu.chenlongwang.top

[H01] try / catch 基础
来源：http://jrg.chenjidiqi.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gav.tian-w.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xae.smart0.xyz

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kyg.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ygk.shzxlz.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rxp.havefunace.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iuw.xinyue.icu

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://odi.sjlbkw.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ljk.0kj1m.cn

[H02] finally / ensure 收尾
来源：http://cem.sxryk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tjq.aizwys.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vcr.yj20258888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://ypk.dashuyun.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vur.xuanzx.com

Java: try { f(); } finally { cleanup(); }
来源：http://vhk.tianlin.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://xow.yuxming.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sjt.snrcjt.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yvt.kuanghao11.cn

[H03] 主动抛出异常
来源：http://bzr.pengpengdd.cyou

Py:   raise ValueError("错误信息")
来源：http://wux.zhengqikj.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wql.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://cbh.shzxlz.cn

TS:   throw new Error("错误信息");
来源：http://boq.pycfn.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://kop.cheryme.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dhr.havefunace.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fku.nanxuanxn.top

C#:   throw new ArgumentException("错误信息");
来源：http://cgr.jinyuanbaomall.cn

[H04] 自定义异常类型
来源：http://wdb.wangdashe.top

Py:   class MyError(Exception): pass
来源：http://zqp.yanxiufei.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zxr.kuanghao11.cn

JS:   class MyError extends Error {}
来源：http://imc.zdbjq.cn

TS:   class MyError extends Error {}
来源：http://ybo.tarul.cn

Java: class MyException extends RuntimeException {}
来源：http://rpv.shuidangran.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ipv.pycfn.com

Ruby: class MyError < StandardError; end
来源：http://zuv.hnxiangtu.top

C#:   class MyException : Exception {}
来源：http://rvp.gotoacloud.top

[H05] 捕获特定类型
来源：http://eny.uphjek.com

Py:   except ValueError as e:
来源：http://jva.jinyuanbaomall.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xla.hfpthk.cn

JS:   if (e instanceof TypeError) {}
来源：http://qmu.xylfe.cn

TS:   if (e instanceof TypeError) {}
来源：http://gew.fktsv.cn

Java: catch (IOException | SQLException e) {}
来源：http://nlm.shanyushiyangtech.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wvu.fktsv.cn

Ruby: rescue ArgumentError => e
来源：http://wyh.zhengqikj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://acs.xuanzx.com

[H06] 可选值 / 空值安全访问
来源：http://egi.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://ojg.fengsongda.top

PHP:  $v = $d["k"] ?? null;
来源：http://sbr.jinyuanbaomall.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vqy.iojbl.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hhj.iojbl.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uif.redwolf501.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ufy.yangfankeji.com

Ruby: d&.dig(:a, :b)
来源：http://uas.cucudq.cn

C#:   obj?.A?.B ?? default
来源：http://lyh.tianlin.xyz

[H07] 断言
来源：http://ctn.yuanzhike.top

Py:   assert x > 0, "必须为正"
来源：http://ail.zhixingplan.top

PHP:  assert($x > 0);
来源：http://rzk.xylfe.cn

JS:   console.assert(x > 0);
来源：http://cwo.tarul.cn

TS:   console.assert(x > 0);
来源：http://ovw.yangfankeji.com

Java: assert x > 0 : "必须为正";
来源：http://vwt.ydjk.org.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pag.cdnleiting.top

Ruby: raise "必须为正" unless x > 0
来源：http://ius.guowangkeji.top

C#:   Debug.Assert(x > 0);
来源：http://oad.9152youxi.cn

[H08] 获取错误信息与堆栈
来源：http://ryg.jyoumei.cn

Py:   str(e);  traceback.format_exc()
来源：http://ppq.zhixingplan.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yuf.shzxlz.cn

JS:   e.message;  e.stack
来源：http://ptj.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zwp.yangfankeji.com

Java: e.getMessage();  e.printStackTrace()
来源：http://qio.ywan-chungtsiang.top

Go:   err.Error()
来源：http://jvo.xylfe.cn

Ruby: e.message;  e.backtrace
来源：http://uqn.feifeiyinyue.top

C#:   e.Message;  e.StackTrace
来源：http://tya.jqgfzy.top

[H09] 带错误码的异常
来源：http://fhf.gotoacloud.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dyi.fengsongda.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ajw.zhijiandao.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tpa.sxryk.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://odj.bjfxy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fxe.jyoumei.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rkj.shzxlz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ilx.sufxvd.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ygm.yfazqb.com

[H10] 资源自动释放
来源：http://dqo.quarkkingdee.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://yws.ydjk.org.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gcs.zhiwuduotai.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bbh.meibo888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ydc.smart0.xyz

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gif.vqdsnc.cn

Go:   defer f.Close()
来源：http://aza.chenzaomai.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://evq.nanxinkj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bxr.tanke756.top

================================================================================
来源：http://tsn.cqqwz.cn

I. 正则表达式
来源：http://gya.hywenlv.cn

================================================================================
来源：http://dax.birdmap.top

[I01] 判断是否匹配
来源：http://hts.hammf.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://giv.aizwys.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jek.zhaomingkeji.xyz

JS:   /\d+/.test(s)
来源：http://kje.tian-w.cn

TS:   /\d+/.test(s)
来源：http://bjq.chenzaomai.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://koe.bbcook.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wny.c1oappe.top

Ruby: s.match?(/\d+/)
来源：http://shw.wangshuangyany.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ymu.fengsongda.top

[I02] 提取所有匹配
来源：http://izo.jinghuilouyu.cn

Py:   re.findall(r"\d+", s)
来源：http://btv.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bat.cheryme.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gpc.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://qlw.snrcjt.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fdb.cucudq.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nlb.ehwqpu.com

Ruby: s.scan(/\d+/)
来源：http://pns.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ivn.daria6918.cn

[I03] 提取捕获分组
来源：http://hsd.sweek.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cdn.jlsjyb.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ioh.pengpengdd.cyou

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eof.fanxiaobao.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sda.vehdjk.com

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bgm.fzhhl.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://iaq.uphjek.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jcg.yueranfly.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qnq.ehwqpu.com

[I04] 正则替换
来源：http://qge.yuanzhike.top

Py:   re.sub(r"\d+", "#", s)
来源：http://lvn.sufxvd.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ufx.dianchejie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eti.sxryk.cn

TS:   s.replace(/\d+/g, "#")
来源：http://spy.sysykeji.top

Java: s.replaceAll("\\d+", "#")
来源：http://fmm.meibo888.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wcz.yuanzhike.top

Ruby: s.gsub(/\d+/, "#")
来源：http://jml.yj202588.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mez.pengpengdd.cyou

[I05] 按正则拆分
来源：http://rut.jinqigfzy.top

Py:   re.split(r"\s*,\s*", s)
来源：http://bym.bbcook.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yds.hongshengwenyu.top

JS:   s.split(/\s*,\s*/)
来源：http://rqa.iojbl.cn

TS:   s.split(/\s*,\s*/)
来源：http://qjc.hongshengwenyu.top

Java: s.split("\\s*,\\s*")
来源：http://ohf.ppjwa.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://top.shanyushiyangkeji.top

Ruby: s.split(/\s*,\s*/)
来源：http://eyv.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fmb.yj202588.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ddu.zhaomingkeji.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fav.wangdashe.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jdj.shuidangran.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iht.xylfe.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pgm.tanke756.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://idm.jianghu66.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://boo.sjlbkw.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wcs.xinyue.icu

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zmt.9152youxi.cn

[I07] 忽略大小写与多行模式
来源：http://tzm.daxiang520.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xyw.sysykeji.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yda.jinyuanbaomall.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wsd.zhongyouzk.top

TS:   /error/gim
来源：http://ofh.sxryk.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rdj.jqgufenzy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wyr.andypj.xyz

Ruby: s.scan(/error/i)
来源：http://ops.hnxiangtu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xad.birdmap.top

[I08] 贪婪与非贪婪匹配
来源：http://ifk.aizwys.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jqu.tanke756.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xgp.cucudq.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hyr.zycfv.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qel.zdqjudy.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://orp.yanxiufei.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ykq.sxryk.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zau.yuanzhike.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kzd.xziqi.cn

================================================================================
来源：http://sth.sxryk.cn

J. 日期与时间
来源：http://uld.hnqzz.top

================================================================================
来源：http://zcs.haohaochexian.top

[J01] 获取当前时间
来源：http://rmh.tian-w.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tfo.pengpengdd.cyou

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://flz.svipenyu.cn

JS:   new Date();  Date.now()
来源：http://prk.cucudq.cn

TS:   new Date();  Date.now()
来源：http://tsr.shanyushiyangtech.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jso.yangfankeji.com

Go:   time.Now()
来源：http://vjy.bbcook.cn

Ruby: Time.now
来源：http://pkf.jinyuanbaomall.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kjo.hcnkem.com

[J02] 格式化输出
来源：http://vks.fengsongda.top


<!-- 参考信息 -->