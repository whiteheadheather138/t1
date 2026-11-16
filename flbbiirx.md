代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://lnq.ctjpmb.com

JS:   greet() { return this.name; }
来源：http://kcs.wangshuangyany.cn

TS:   greet(): string { return this.name; }
来源：http://jaw.smart0.xyz

Java: String greet() { return name; }
来源：http://pax.yj20258888.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://moc.snrcjt.cn

Ruby: def greet; @name; end
来源：http://pac.zhoulong.xyz

C#:   public string Greet() => Name;
来源：http://vcn.snrcjt.cn

[G05] 继承
来源：http://coa.fzhhl.top

Py:   class Admin(User): pass
来源：http://rhy.nanxuanxn.top

PHP:  class Admin extends User {}
来源：http://wxb.hcnkem.com

JS:   class Admin extends User {}
来源：http://ugz.shangyingyoupin.top

TS:   class Admin extends User {}
来源：http://ctk.zhengqikj.top

Java: class Admin extends User {}
来源：http://ubg.ywan-chungtsiang.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nkd.xziqi.cn

Ruby: class Admin < User; end
来源：http://oms.yongpay.top

C#:   class Admin : User {}
来源：http://zxt.birdmap.top

[G06] 重写方法
来源：http://tzs.ctjpmb.com

Py:   def greet(self): return "admin"
来源：http://sdi.zhengqikj.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zpw.yvedp.cn

JS:   greet() { return "admin"; }
来源：http://xyn.nwbrower.top

TS:   greet(): string { return "admin"; }
来源：http://axh.cheryme.top

Java: @Override String greet() { return "admin"; }
来源：http://jrh.feifeiyinyue.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dub.feifeiyinyue.top

Ruby: def greet; "admin"; end
来源：http://ecd.birdmap.top

C#:   public override string Greet() => "admin";
来源：http://oor.jinghuilouyu.cn

[G07] 调用父类方法
来源：http://bnt.andypj.xyz

Py:   super().greet()
来源：http://ohd.wangdashe.top

PHP:  parent::greet();
来源：http://wmr.ybcxt.top

JS:   super.greet();
来源：http://dqw.fzhhl.top

TS:   super.greet();
来源：http://jme.shuidangran.top

Java: super.greet();
来源：http://ccx.snrcjt.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ekv.yongpay.top

Ruby: super
来源：http://hua.birdmap.top

C#:   base.Greet();
来源：http://fkb.sxryk.cn

[G08] 静态方法与属性
来源：http://amk.mhx1999.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hao.ywan-chungtsiang.top

PHP:  public static function f() {}
来源：http://zqr.hnxiangtu.top

JS:   static f() {}
来源：http://ljr.cashguo.top

TS:   static f(): void {}
来源：http://lcg.gaohongyu789.top

Java: static void f() {}
来源：http://jmg.fanxiaobao.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://puk.yfazqb.com

Ruby: def self.f; end
来源：http://yam.bjfxy.top

C#:   public static void F() {}
来源：http://zav.jlsjyb.cn

[G09] 接口 / 抽象类
来源：http://qvo.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://ghl.zycfv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wjm.tarul.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qde.cheryme.top

TS:   interface Shape { area(): number; }
来源：http://axz.yj20258888.top

Java: interface Shape { double area(); }
来源：http://mnk.xylfe.cn

Go:   type Shape interface { Area() float64 }
来源：http://drz.jqgufenzy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jam.fktsv.cn

C#:   interface IShape { double Area(); }
来源：http://rhx.pengpengdd.cyou

[G10] 访问控制
来源：http://gte.fengsongda.top

Py:   约定 _protected / __private（不强制）
来源：http://mlr.yangfankeji.com

PHP:  public / protected / private
来源：http://jju.sufxvd.cn

JS:   #private 字段；其余公开
来源：http://pdb.feifeiyinyue.top

TS:   public / protected / private
来源：http://pas.yangfankeji.com

Java: public / protected / private / 默认包级
来源：http://ion.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://lpv.fzhhl.top

Ruby: public / protected / private
来源：http://qjj.cqqwz.cn

C#:   public / protected / private / internal
来源：http://aab.shanyushiyangkeji.top

[G11] getter / setter
来源：http://zri.shzxlz.cn

Py:   @property 与 @x.setter
来源：http://rfc.bbcook.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rhs.zhixingplan.top

JS:   get name() { return this._name; }
来源：http://otf.gotoacloud.top

TS:   get name(): string { return this._name; }
来源：http://czo.gogol.net.cn

Java: public String getName() { return name; }
来源：http://bzl.zhoulong.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://wtv.gogol.net.cn

Ruby: attr_accessor :name
来源：http://xya.svipenyu.cn

C#:   public string Name { get; set; }
来源：http://ovq.fanxiaobao.xyz

[G12] 对象转字符串
来源：http://gmm.yj20258888.top

Py:   def __str__(self): return self.name
来源：http://fag.nanxinkj.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://zmp.chenjidiqi.icu

JS:   toString() { return this.name; }
来源：http://ukw.snrcjt.cn

TS:   toString(): string { return this.name; }
来源：http://aha.ivvv.top

Java: @Override public String toString() { return name; }
来源：http://bxv.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://kdh.xziqi.cn

Ruby: def to_s; @name; end
来源：http://tbd.hesvh.cn

C#:   public override string ToString() => Name;
来源：http://ojm.shuidangran.top

[G13] 判断对象类型
来源：http://rbg.ehwqpu.com

Py:   isinstance(u, User)
来源：http://rjo.nanxuanxn.top

PHP:  $u instanceof User
来源：http://rqy.svipenyu.cn

JS:   u instanceof User
来源：http://izl.xuanzx.com

TS:   u instanceof User
来源：http://mnj.cdnleiting.top

Java: u instanceof User
来源：http://qvu.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://xkg.zycfv.cn

Ruby: u.is_a?(User)
来源：http://hmt.xingfuxueyuan.xyz

C#:   u is User
来源：http://jeb.hesvh.cn

[G14] 数据类 / record
来源：http://fyr.shanyushiyangkeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hrc.guannengcc.top

PHP:  // 用 readonly 属性模拟
来源：http://wft.cashguo.top

JS:   // 无内置：普通类或对象字面量
来源：http://qky.vqdsnc.cn

TS:   type User = { name: string; age: number };
来源：http://atl.birdmap.top

Java: record User(String name, int age) {}
来源：http://irq.shangyingyoupin.top

Go:   type User struct { Name string; Age int }
来源：http://xtz.yuanzhike.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://idr.ydjk.org.cn

C#:   record User(string Name, int Age);
来源：http://nym.pycfn.com

[G15] 枚举
来源：http://ghq.chenzaomai.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ros.yuanzhike.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gwz.ehwqpu.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nil.hongshengwenyu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gdj.bbcook.cn

Java: enum Color { RED, GREEN }
来源：http://ntc.iojbl.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ktt.tarul.cn

Ruby: Color = %i[red green].freeze
来源：http://peo.yuxming.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jak.fzhhl.top

[G16] 对象转数组 / 字典
来源：http://agb.hammf.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cex.ywan-chungtsiang.top

PHP:  get_object_vars($obj);
来源：http://rld.hywenlv.cn

JS:   Object.entries(obj)
来源：http://nyi.316326.xyz

TS:   Object.entries(obj)
来源：http://joy.ctjpmb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://phb.feifeiyinyue.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://eab.nanxuanxn.top

Ruby: obj.instance_variables
来源：http://lgi.ppjwa.cn

C#:   // 用反射或 System.Text.Json
来源：http://vkq.gzhubu.top

================================================================================
来源：http://mal.zhengqikj.top

H. 异常与错误处理
来源：http://jzf.chenlongwang.top

================================================================================
来源：http://vzx.gotoacloud.top

[H01] try / catch 基础
来源：http://anw.chenlongwang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ycc.zhixingplan.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fem.fehbvm.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ihx.wangdashe.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ttz.jyoumei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zki.cqqwz.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nal.shanyushiyangkeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uiq.shuidangran.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jqr.chenjidiqi.icu

[H02] finally / ensure 收尾
来源：http://cxn.sxryk.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cvn.jinqigfzy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fzu.yj20258888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://pyc.sufxvd.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qrt.aizwys.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qpl.pycfn.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://kwk.shzxlz.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jqd.zdbjq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vxv.fanxiaobao.xyz

[H03] 主动抛出异常
来源：http://zke.yfazqb.com

Py:   raise ValueError("错误信息")
来源：http://wwf.ybcxt.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lwo.fengsongda.top

JS:   throw new Error("错误信息");
来源：http://exw.redwolf501.top

TS:   throw new Error("错误信息");
来源：http://pti.pycfn.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://qlx.yueranfly.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yab.nanxuanxn.top

Ruby: raise ArgumentError, "错误信息"
来源：http://zbk.uphjek.com

C#:   throw new ArgumentException("错误信息");
来源：http://ttl.xylfe.cn

[H04] 自定义异常类型
来源：http://mjk.epnwcf.com

Py:   class MyError(Exception): pass
来源：http://rsj.xinyue.icu

PHP:  class MyError extends RuntimeException {}
来源：http://qsu.jlsjyb.cn

JS:   class MyError extends Error {}
来源：http://afb.chenlongwang.top

TS:   class MyError extends Error {}
来源：http://gdn.dashuyun.cn

Java: class MyException extends RuntimeException {}
来源：http://dyi.nwbrower.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ebu.andypj.xyz

Ruby: class MyError < StandardError; end
来源：http://rkp.ctjpmb.com

C#:   class MyException : Exception {}
来源：http://wxk.bjfxy.top

[H05] 捕获特定类型
来源：http://rxu.316326.xyz

Py:   except ValueError as e:
来源：http://fzf.svipenyu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lcg.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://alr.zycfv.cn

TS:   if (e instanceof TypeError) {}
来源：http://znj.yonumen.top

Java: catch (IOException | SQLException e) {}
来源：http://bjh.birdmap.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://guf.vehdjk.com

Ruby: rescue ArgumentError => e
来源：http://dda.zdbjq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xhb.shzxlz.cn

[H06] 可选值 / 空值安全访问
来源：http://ijv.yueranfly.top

Py:   value = d.get("k") or default
来源：http://yes.jqgfzy.top

PHP:  $v = $d["k"] ?? null;
来源：http://juo.jqgufenzy.top

JS:   obj?.a?.b;  d ?? default
来源：http://pvd.cucudq.cn

TS:   obj?.a?.b;  d ?? default
来源：http://upp.ybcxt.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kej.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://vhi.gogol.net.cn

Ruby: d&.dig(:a, :b)
来源：http://vqc.9152youxi.cn

C#:   obj?.A?.B ?? default
来源：http://frp.yfazqb.com

[H07] 断言
来源：http://qjl.hesvh.cn

Py:   assert x > 0, "必须为正"
来源：http://ibh.kuanghao11.cn

PHP:  assert($x > 0);
来源：http://pur.jqgfzy.top

JS:   console.assert(x > 0);
来源：http://apj.zhiwuduotai.top

TS:   console.assert(x > 0);
来源：http://mqu.jinqigfzy.top

Java: assert x > 0 : "必须为正";
来源：http://mkv.kuanghao11.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pxe.vehdjk.com

Ruby: raise "必须为正" unless x > 0
来源：http://jye.nanxuanxn.top

C#:   Debug.Assert(x > 0);
来源：http://nzz.cashguo.top

[H08] 获取错误信息与堆栈
来源：http://anh.andypj.xyz

Py:   str(e);  traceback.format_exc()
来源：http://tnj.gzhubu.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bwu.zhongyouzk.top

JS:   e.message;  e.stack
来源：http://znc.yanxiufei.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://oag.shangyingyoupin.top

Java: e.getMessage();  e.printStackTrace()
来源：http://weo.uphjek.com

Go:   err.Error()
来源：http://mvn.feifeiyinyue.top

Ruby: e.message;  e.backtrace
来源：http://ecd.52xcode.cn

C#:   e.Message;  e.StackTrace
来源：http://ujn.jqgufenzy.top

[H09] 带错误码的异常
来源：http://rpr.xziqi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gcy.ydjk.org.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qve.sjlbkw.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fxj.tarul.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wzq.yfazqb.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qup.gzhubu.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://muv.hesvh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kjz.zycfv.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zyt.shangyingyoupin.top

[H10] 资源自动释放
来源：http://lnk.aizwys.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zlb.guowangkeji.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pvl.nanxinkj.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bpg.316326.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nsq.bbcook.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vlp.jqgufenzy.top

Go:   defer f.Close()
来源：http://ovv.sysykeji.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pxh.ehwqpu.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kdh.c1oappe.top

================================================================================
来源：http://qnp.jqgufenzy.top

I. 正则表达式
来源：http://uno.fanxiaobao.xyz

================================================================================
来源：http://tnh.yuanzhike.top

[I01] 判断是否匹配
来源：http://lvd.sxryk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://usa.sxryk.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nkl.jinyuanbaomall.cn

JS:   /\d+/.test(s)
来源：http://avz.52xcode.cn

TS:   /\d+/.test(s)
来源：http://jff.svipenyu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eme.ydzc1.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iof.jqgufenzy.top

Ruby: s.match?(/\d+/)
来源：http://wii.cheryme.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wnu.fzhhl.top

[I02] 提取所有匹配
来源：http://ayg.yongpay.top

Py:   re.findall(r"\d+", s)
来源：http://cim.hesvh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fug.wangshuangyany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vwi.zhaomingkeji.xyz

TS:   s.match(/\d+/g)
来源：http://rqq.fanxiaobao.xyz

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pzn.yonumen.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iha.shzxlz.cn

Ruby: s.scan(/\d+/)
来源：http://bwg.hysaishi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rob.shangyingyoupin.top

[I03] 提取捕获分组
来源：http://xse.jinqigfzy.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ows.wangdashe.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://npn.sweek.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jmm.jlsjyb.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qmh.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xjk.guowangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yil.wangdashe.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jzx.jinqigufen.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://geg.jinyuanbaomall.cn

[I04] 正则替换
来源：http://uha.chenzaomai.com

Py:   re.sub(r"\d+", "#", s)
来源：http://obr.yueranfly.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://skm.snrcjt.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dlc.xuanzx.com

TS:   s.replace(/\d+/g, "#")
来源：http://uew.epnwcf.com

Java: s.replaceAll("\\d+", "#")
来源：http://kfb.zdbjq.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://frw.ppjwa.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jlk.mhx1999.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gqg.tarul.cn

[I05] 按正则拆分
来源：http://skg.ybcxt.top

Py:   re.split(r"\s*,\s*", s)
来源：http://hqb.pengpengdd.cyou

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://flh.ehwqpu.com

JS:   s.split(/\s*,\s*/)
来源：http://hta.jlsjyb.cn

TS:   s.split(/\s*,\s*/)
来源：http://ljf.shzxlz.cn

Java: s.split("\\s*,\\s*")
来源：http://lkt.shanyushiyangtech.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://moh.jiagoushi.top

Ruby: s.split(/\s*,\s*/)
来源：http://crm.guowangkeji.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lml.fzhhl.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rxt.fktsv.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xcv.jqgfzy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pmr.jqgufenzy.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://udn.zdbjq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wnc.jianghu66.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vof.ehwqpu.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ilu.hysaishi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cai.jianghu66.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qro.yonumen.top

[I07] 忽略大小写与多行模式
来源：http://kpe.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ahk.jqgfzy.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wfn.hongshengwenyu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lvl.snrcjt.cn

TS:   /error/gim
来源：http://hts.xuanzx.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xkj.redwolf501.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://znf.jinqigfzy.top

Ruby: s.scan(/error/i)
来源：http://kgz.zhaomingkeji.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mlj.zdbjq.cn

[I08] 贪婪与非贪婪匹配
来源：http://obc.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sjr.zhaomingkeji.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dlo.ivvv.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vrp.c1oappe.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yfw.sweek.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://qdk.tian-w.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zrp.mhx1999.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://obb.smart0.xyz

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zyt.shanyushiyangkeji.top

================================================================================
来源：http://wue.xylfe.cn

J. 日期与时间
来源：http://iqn.ydjk.org.cn

================================================================================
来源：http://tol.jlsjyb.cn

[J01] 获取当前时间
来源：http://nsb.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://fxw.ybcxt.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://avw.wangdashe.top

JS:   new Date();  Date.now()
来源：http://yuu.cqqwz.cn

TS:   new Date();  Date.now()
来源：http://lqd.xylfe.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://efg.hcnkem.com

Go:   time.Now()
来源：http://gmw.shzxlz.cn

Ruby: Time.now
来源：http://bjw.cdnleiting.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://arz.cqqwz.cn

[J02] 格式化输出
来源：http://dcd.xuetiantiany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ydg.fehbvm.com

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rfv.jianghu66.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ogk.tanke756.top

TS:   d.toISOString()
来源：http://rgx.shuidangran.top


<!-- 参考信息 -->