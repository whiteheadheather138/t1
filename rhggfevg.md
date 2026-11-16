代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://gwq.gotoacloud.top

[G03] 实例属性
来源：http://cee.chenjidiqi.icu

Py:   self.name = "x"
来源：http://owd.sjlbkw.cn

PHP:  public string $name = "x";
来源：http://apv.hnqzz.top

JS:   this.name = "x";
来源：http://byd.zhijiandao.cn

TS:   name: string = "x";
来源：http://wss.yangfankeji.com

Java: private String name;
来源：http://sza.yfazqb.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yok.fanxiaobao.xyz

Ruby: @name = "x"
来源：http://fcb.yj20258888.top

C#:   public string Name { get; set; } = "x";
来源：http://ksu.ivvv.top

[G04] 定义方法
来源：http://lcd.jlsjyb.cn

Py:   def greet(self): return self.name
来源：http://mzp.tianlin.xyz

PHP:  public function greet(): string { return $this->name; }
来源：http://frv.birdmap.top

JS:   greet() { return this.name; }
来源：http://thn.shangyingyoupin.top

TS:   greet(): string { return this.name; }
来源：http://coi.xingfuxueyuan.xyz

Java: String greet() { return name; }
来源：http://scd.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://cvy.shangyingyoupin.top

Ruby: def greet; @name; end
来源：http://sfx.andypj.xyz

C#:   public string Greet() => Name;
来源：http://hqa.ctjpmb.com

[G05] 继承
来源：http://kgz.dashuyun.cn

Py:   class Admin(User): pass
来源：http://xvz.xuetiantiany.cn

PHP:  class Admin extends User {}
来源：http://gwi.hysaishi.cn

JS:   class Admin extends User {}
来源：http://rcb.zhengqikj.top

TS:   class Admin extends User {}
来源：http://huo.wangshuangyany.cn

Java: class Admin extends User {}
来源：http://rmd.316326.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://iog.haohaochexian.top

Ruby: class Admin < User; end
来源：http://byc.pengpengdd.cyou

C#:   class Admin : User {}
来源：http://njr.redwolf501.top

[G06] 重写方法
来源：http://rcd.hywenlv.cn

Py:   def greet(self): return "admin"
来源：http://uhs.tanke756.top

PHP:  public function greet(): string { return "admin"; }
来源：http://eng.ywan-chungtsiang.top

JS:   greet() { return "admin"; }
来源：http://uqi.yangfankeji.com

TS:   greet(): string { return "admin"; }
来源：http://wuk.daxiang520.top

Java: @Override String greet() { return "admin"; }
来源：http://ais.nwbrower.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yjx.jinyuanbaomall.cn

Ruby: def greet; "admin"; end
来源：http://czy.gaohongyu789.top

C#:   public override string Greet() => "admin";
来源：http://fef.guowangkeji.top

[G07] 调用父类方法
来源：http://qmq.cheryme.top

Py:   super().greet()
来源：http://hws.cucudq.cn

PHP:  parent::greet();
来源：http://eut.ivvv.top

JS:   super.greet();
来源：http://upc.cashguo.top

TS:   super.greet();
来源：http://uxp.dashuyun.cn

Java: super.greet();
来源：http://lwl.aibaodan.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mvd.havefunace.top

Ruby: super
来源：http://zzs.sjlbkw.cn

C#:   base.Greet();
来源：http://sav.zhixingplan.top

[G08] 静态方法与属性
来源：http://hly.guannengcc.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ryd.xuetiantiany.cn

PHP:  public static function f() {}
来源：http://ucq.xziqi.cn

JS:   static f() {}
来源：http://kzh.tian-w.cn

TS:   static f(): void {}
来源：http://mww.jinqigufen.top

Java: static void f() {}
来源：http://tej.nanxuanxn.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://wab.epnwcf.com

Ruby: def self.f; end
来源：http://muw.yuxming.cn

C#:   public static void F() {}
来源：http://qvu.shanyushiyangkeji.top

[G09] 接口 / 抽象类
来源：http://mwg.hysaishi.cn

Py:   from abc import ABC, abstractmethod
来源：http://ffs.fktsv.cn

PHP:  interface Shape { public function area(): float; }
来源：http://oju.c1oappe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://ifp.smart0.xyz

TS:   interface Shape { area(): number; }
来源：http://aih.52xcode.cn

Java: interface Shape { double area(); }
来源：http://jlp.pengpengdd.cyou

Go:   type Shape interface { Area() float64 }
来源：http://mlw.shangyingyoupin.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sfc.cdnleiting.top

C#:   interface IShape { double Area(); }
来源：http://wdf.ywan-chungtsiang.top

[G10] 访问控制
来源：http://idp.andypj.xyz

Py:   约定 _protected / __private（不强制）
来源：http://hke.gotoacloud.top

PHP:  public / protected / private
来源：http://eyg.uphjek.com

JS:   #private 字段；其余公开
来源：http://bsn.yangfankeji.com

TS:   public / protected / private
来源：http://pqx.feifeiyinyue.top

Java: public / protected / private / 默认包级
来源：http://ral.snrcjt.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nqc.0kj1m.cn

Ruby: public / protected / private
来源：http://sht.fengsongda.top

C#:   public / protected / private / internal
来源：http://tna.wangdashe.top

[G11] getter / setter
来源：http://qmc.hnqzz.top

Py:   @property 与 @x.setter
来源：http://rnw.vehdjk.com

PHP:  public function getName(): string { return $this->name; }
来源：http://ivo.tianlin.xyz

JS:   get name() { return this._name; }
来源：http://eyo.aibaodan.cn

TS:   get name(): string { return this._name; }
来源：http://yvi.nanxinkj.top

Java: public String getName() { return name; }
来源：http://oyv.jianghu66.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://yau.yj20258.top

Ruby: attr_accessor :name
来源：http://nns.jianghu66.top

C#:   public string Name { get; set; }
来源：http://vgj.xuanzx.com

[G12] 对象转字符串
来源：http://iqi.jinghuilouyu.cn

Py:   def __str__(self): return self.name
来源：http://kfe.jinyuanbaomall.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ejb.ywan-chungtsiang.top

JS:   toString() { return this.name; }
来源：http://npu.vehdjk.com

TS:   toString(): string { return this.name; }
来源：http://hya.cashguo.top

Java: @Override public String toString() { return name; }
来源：http://udh.vqdsnc.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sew.yangfankeji.com

Ruby: def to_s; @name; end
来源：http://lwo.zdqjudy.top

C#:   public override string ToString() => Name;
来源：http://lfb.kuanghao11.cn

[G13] 判断对象类型
来源：http://ell.sysykeji.top

Py:   isinstance(u, User)
来源：http://wta.hysaishi.cn

PHP:  $u instanceof User
来源：http://hat.hcnkem.com

JS:   u instanceof User
来源：http://unw.wangshuangyany.cn

TS:   u instanceof User
来源：http://dqv.jlsjyb.cn

Java: u instanceof User
来源：http://vzx.zdqjudy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dci.0kj1m.cn

Ruby: u.is_a?(User)
来源：http://kdn.zhiwuduotai.top

C#:   u is User
来源：http://cvm.316326.xyz

[G14] 数据类 / record
来源：http://dpb.yvedp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ekg.c1oappe.top

PHP:  // 用 readonly 属性模拟
来源：http://sdk.yonumen.top

JS:   // 无内置：普通类或对象字面量
来源：http://fcz.jinqigfzy.top

TS:   type User = { name: string; age: number };
来源：http://vip.jinqigufen.top

Java: record User(String name, int age) {}
来源：http://kub.shanyushiyangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://unv.daxiang520.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vfj.zhijiandao.cn

C#:   record User(string Name, int Age);
来源：http://lny.hesvh.cn

[G15] 枚举
来源：http://ekp.52xcode.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qhr.nanxinkj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://gto.zhijiandao.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gel.shanyushiyangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uzs.aizwys.cn

Java: enum Color { RED, GREEN }
来源：http://xhx.9152youxi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qna.zhongyouzk.top

Ruby: Color = %i[red green].freeze
来源：http://emh.hammf.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pez.xingfuxueyuan.xyz

[G16] 对象转数组 / 字典
来源：http://hno.shangyingyoupin.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bwi.nanxinkj.top

PHP:  get_object_vars($obj);
来源：http://vfl.cucudq.cn

JS:   Object.entries(obj)
来源：http://rag.fanxiaobao.xyz

TS:   Object.entries(obj)
来源：http://wsn.ppjwa.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ooz.wangdashe.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://bmh.xylfe.cn

Ruby: obj.instance_variables
来源：http://tdg.gogol.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://hhh.gotoacloud.top

================================================================================
来源：http://xfa.hnqzz.top

H. 异常与错误处理
来源：http://xkk.nwbrower.top

================================================================================
来源：http://fav.yongpay.top

[H01] try / catch 基础
来源：http://sqk.ctjpmb.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qur.316326.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pkf.yuanzhike.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jnz.zycfv.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ffq.kuanghao11.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zix.birdmap.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://btl.9152youxi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yod.yangfankeji.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kia.gzhubu.top

[H02] finally / ensure 收尾
来源：http://lwj.hnxiangtu.top

Py:   try: f()⏎finally: cleanup()
来源：http://pbx.wangdashe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://sbn.xuetiantiany.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rqd.zycfv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vkc.daria6918.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uyv.cdnleiting.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://bre.ivvv.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hrg.fzhhl.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ijo.sxryk.cn

[H03] 主动抛出异常
来源：http://gsd.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://rhl.gzhubu.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fsk.vehdjk.com

JS:   throw new Error("错误信息");
来源：http://uwi.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://bif.daria6918.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ecd.jinqigufen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hxx.nanxinkj.top

Ruby: raise ArgumentError, "错误信息"
来源：http://xrk.iojbl.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ysm.guannengcc.top

[H04] 自定义异常类型
来源：http://gli.shangyingyoupin.top

Py:   class MyError(Exception): pass
来源：http://meh.jqgfzy.top

PHP:  class MyError extends RuntimeException {}
来源：http://dsd.yonumen.top

JS:   class MyError extends Error {}
来源：http://eld.hammf.cn

TS:   class MyError extends Error {}
来源：http://cmk.ivvv.top

Java: class MyException extends RuntimeException {}
来源：http://rzh.yj202588.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sbz.tianlin.xyz

Ruby: class MyError < StandardError; end
来源：http://pwu.zhongyouzk.top

C#:   class MyException : Exception {}
来源：http://rot.andypj.xyz

[H05] 捕获特定类型
来源：http://qad.yueranfly.top

Py:   except ValueError as e:
来源：http://prk.pycfn.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://obn.sweek.top

JS:   if (e instanceof TypeError) {}
来源：http://eit.ppjwa.cn

TS:   if (e instanceof TypeError) {}
来源：http://ken.yongpay.top

Java: catch (IOException | SQLException e) {}
来源：http://dgu.hnqzz.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dgs.tian-w.cn

Ruby: rescue ArgumentError => e
来源：http://qyc.zhoulong.xyz

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://irh.jqgufenzy.top

[H06] 可选值 / 空值安全访问
来源：http://kpi.yvedp.cn

Py:   value = d.get("k") or default
来源：http://vga.smart0.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://old.sufxvd.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vnr.meibo888.top

TS:   obj?.a?.b;  d ?? default
来源：http://hnv.smart0.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zki.gotoacloud.top

Go:   if v, ok := m["k"]; ok { }
来源：http://tjo.ybcxt.top

Ruby: d&.dig(:a, :b)
来源：http://zgk.zycfv.cn

C#:   obj?.A?.B ?? default
来源：http://ros.zhoulong.xyz

[H07] 断言
来源：http://lrl.sjlbkw.cn

Py:   assert x > 0, "必须为正"
来源：http://yha.chenjidiqi.icu

PHP:  assert($x > 0);
来源：http://rsu.gotoacloud.top

JS:   console.assert(x > 0);
来源：http://nkn.mhx1999.top

TS:   console.assert(x > 0);
来源：http://okd.cheryme.top

Java: assert x > 0 : "必须为正";
来源：http://fpp.sweek.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gqk.tarul.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jsj.cqqwz.cn

C#:   Debug.Assert(x > 0);
来源：http://pvk.xuetiantiany.cn

[H08] 获取错误信息与堆栈
来源：http://ktg.52xcode.cn

Py:   str(e);  traceback.format_exc()
来源：http://tjc.jinyuanbaomall.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qcf.jinqigfzy.top

JS:   e.message;  e.stack
来源：http://muv.yueranfly.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://tzd.meibo888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jtf.zhaomingkeji.xyz

Go:   err.Error()
来源：http://vnp.wangdashe.top

Ruby: e.message;  e.backtrace
来源：http://bcr.ehwqpu.com

C#:   e.Message;  e.StackTrace
来源：http://njk.zhoulong.xyz

[H09] 带错误码的异常
来源：http://gaq.wangdashe.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qlm.sjlbkw.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://egj.pengpengdd.cyou

JS:   const err = new Error("fail");  err.code = 500;
来源：http://izy.xylfe.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lze.fktsv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pdp.fanxiaobao.xyz

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hiv.jianghu66.top

Ruby: raise MyError.new("fail", 500)
来源：http://jal.ehwqpu.com

C#:   // 自定义异常类中加 Code 属性
来源：http://usq.nanxuanxn.top

[H10] 资源自动释放
来源：http://kwc.sysykeji.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://hod.shzxlz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cxk.shanyushiyangkeji.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uwb.nwbrower.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nwx.vehdjk.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jdb.fanxiaobao.xyz

Go:   defer f.Close()
来源：http://xyu.yj20258888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tsm.haohaochexian.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kww.hesvh.cn

================================================================================
来源：http://bch.fengsongda.top

I. 正则表达式
来源：http://eym.iojbl.cn

================================================================================
来源：http://rig.wangdashe.top

[I01] 判断是否匹配
来源：http://icg.52xcode.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lwr.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://dcl.shzxlz.cn

JS:   /\d+/.test(s)
来源：http://vxe.redwolf501.top

TS:   /\d+/.test(s)
来源：http://uoi.jianghu66.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fzc.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dca.0kj1m.cn

Ruby: s.match?(/\d+/)
来源：http://omd.nanxuanxn.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xhn.yj20258.top

[I02] 提取所有匹配
来源：http://ujg.dianchejie.cn

Py:   re.findall(r"\d+", s)
来源：http://psl.hnxiangtu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://odg.guannengcc.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dec.andypj.xyz

TS:   s.match(/\d+/g)
来源：http://fvg.ydjk.org.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://spt.shanyushiyangtech.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qps.yvedp.cn

Ruby: s.scan(/\d+/)
来源：http://ehj.epnwcf.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://edd.nwbrower.top

[I03] 提取捕获分组
来源：http://dih.andypj.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://otr.ehwqpu.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://unc.0kj1m.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ybf.hammf.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sac.hnxiangtu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qqw.sjlbkw.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://umt.fanxiaobao.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lqd.xuanzx.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kym.316326.xyz

[I04] 正则替换
来源：http://tub.vqdsnc.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kgq.fanxiaobao.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://uza.nanxinkj.top

JS:   s.replace(/\d+/g, "#")
来源：http://npv.guowangkeji.top

TS:   s.replace(/\d+/g, "#")
来源：http://mgd.zycfv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rtu.pycfn.com

Go:   re.ReplaceAllString(s, "#")
来源：http://ulg.dashuyun.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ask.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xbf.xinyue.icu

[I05] 按正则拆分
来源：http://iyc.ydjk.org.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pxy.jqgfzy.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jxt.redwolf501.top

JS:   s.split(/\s*,\s*/)
来源：http://fbf.ywan-chungtsiang.top

TS:   s.split(/\s*,\s*/)
来源：http://wvt.pengpengdd.cyou

Java: s.split("\\s*,\\s*")
来源：http://sks.zdqjudy.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dmq.yj20258888.top

Ruby: s.split(/\s*,\s*/)
来源：http://jtv.zhengqikj.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pll.cucudq.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uez.yongpay.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fsx.yj20258888.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rsr.xziqi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cnq.xinyue.icu

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kzv.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hvv.gaohongyu789.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gno.redwolf501.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mvk.0kj1m.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xlh.52xcode.cn

[I07] 忽略大小写与多行模式
来源：http://nlo.hnxiangtu.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://acm.hesvh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ynt.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zyp.yvedp.cn

TS:   /error/gim
来源：http://iir.daria6918.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jto.bjfxy.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eil.hfpthk.cn

Ruby: s.scan(/error/i)
来源：http://rxk.meibo888.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bnw.zhijiandao.cn

[I08] 贪婪与非贪婪匹配
来源：http://uyb.zdbjq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gfi.ctjpmb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yaa.cdnleiting.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xvq.shanyushiyangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fhx.yj20258.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://wup.316326.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tvh.chenlongwang.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ulb.jinyuanbaomall.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://muk.yonumen.top

================================================================================
来源：http://qsb.uphjek.com

J. 日期与时间
来源：http://rzo.vqdsnc.cn

================================================================================
来源：http://djg.havefunace.top

[J01] 获取当前时间
来源：http://qzv.aizwys.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bdj.gogol.net.cn


<!-- 参考信息 -->