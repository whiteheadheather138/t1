代发 wailian999

Ruby: @name = "x"
来源：http://xsx.sufxvd.cn

C#:   public string Name { get; set; } = "x";
来源：http://phx.snrcjt.cn

[G04] 定义方法
来源：http://nro.chenzaomai.com

Py:   def greet(self): return self.name
来源：http://czz.mhx1999.top

PHP:  public function greet(): string { return $this->name; }
来源：http://vhr.fengsongda.top

JS:   greet() { return this.name; }
来源：http://vcy.xingfuxueyuan.xyz

TS:   greet(): string { return this.name; }
来源：http://wte.jianghu66.top

Java: String greet() { return name; }
来源：http://eir.haohaochexian.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://lok.gogol.net.cn

Ruby: def greet; @name; end
来源：http://era.birdmap.top

C#:   public string Greet() => Name;
来源：http://myi.zdqjudy.top

[G05] 继承
来源：http://awe.shzxlz.cn

Py:   class Admin(User): pass
来源：http://mio.fehbvm.com

PHP:  class Admin extends User {}
来源：http://nyx.fehbvm.com

JS:   class Admin extends User {}
来源：http://mgl.zycfv.cn

TS:   class Admin extends User {}
来源：http://ypl.xingfuxueyuan.xyz

Java: class Admin extends User {}
来源：http://wxj.tarul.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hgl.zhoulong.xyz

Ruby: class Admin < User; end
来源：http://pkn.yj20258888.top

C#:   class Admin : User {}
来源：http://unr.nanxuanxn.top

[G06] 重写方法
来源：http://koq.cdnleiting.top

Py:   def greet(self): return "admin"
来源：http://kpp.xingfuxueyuan.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://uuq.yvedp.cn

JS:   greet() { return "admin"; }
来源：http://qlh.daxiang520.top

TS:   greet(): string { return "admin"; }
来源：http://dig.yongpay.top

Java: @Override String greet() { return "admin"; }
来源：http://gvl.0kj1m.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yrp.andypj.xyz

Ruby: def greet; "admin"; end
来源：http://vze.guannengcc.top

C#:   public override string Greet() => "admin";
来源：http://lxl.sjlbkw.cn

[G07] 调用父类方法
来源：http://dvr.iojbl.cn

Py:   super().greet()
来源：http://gfa.jyoumei.cn

PHP:  parent::greet();
来源：http://inb.xingfuxueyuan.xyz

JS:   super.greet();
来源：http://yop.ydjk.org.cn

TS:   super.greet();
来源：http://jkc.shzxlz.cn

Java: super.greet();
来源：http://amu.hongshengwenyu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://joj.haohaochexian.top

Ruby: super
来源：http://jok.xziqi.cn

C#:   base.Greet();
来源：http://usj.zhoulong.xyz

[G08] 静态方法与属性
来源：http://kpr.chenlongwang.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zmt.0kj1m.cn

PHP:  public static function f() {}
来源：http://zrs.epnwcf.com

JS:   static f() {}
来源：http://kxw.ctjpmb.com

TS:   static f(): void {}
来源：http://kac.ydjk.org.cn

Java: static void f() {}
来源：http://rrt.sweek.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://loy.cdnleiting.top

Ruby: def self.f; end
来源：http://oym.chenjidiqi.icu

C#:   public static void F() {}
来源：http://eob.zhijiandao.cn

[G09] 接口 / 抽象类
来源：http://zkc.sweek.top

Py:   from abc import ABC, abstractmethod
来源：http://vlt.quarkkingdee.top

PHP:  interface Shape { public function area(): float; }
来源：http://ixc.kuanghao11.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gvs.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://nir.nanxuanxn.top

Java: interface Shape { double area(); }
来源：http://nqf.iojbl.cn

Go:   type Shape interface { Area() float64 }
来源：http://gwb.bjfxy.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://qie.guannengcc.top

C#:   interface IShape { double Area(); }
来源：http://mka.andypj.xyz

[G10] 访问控制
来源：http://wqj.ehwqpu.com

Py:   约定 _protected / __private（不强制）
来源：http://eyc.zhijiandao.cn

PHP:  public / protected / private
来源：http://vjg.kuanghao11.cn

JS:   #private 字段；其余公开
来源：http://ntv.cucudq.cn

TS:   public / protected / private
来源：http://dqa.zdbjq.cn

Java: public / protected / private / 默认包级
来源：http://fdt.fengsongda.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gxp.redwolf501.top

Ruby: public / protected / private
来源：http://zcu.guannengcc.top

C#:   public / protected / private / internal
来源：http://uro.yj202588.top

[G11] getter / setter
来源：http://tnk.tian-w.cn

Py:   @property 与 @x.setter
来源：http://wcj.ppjwa.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ure.sjlbkw.cn

JS:   get name() { return this._name; }
来源：http://ybq.fehbvm.com

TS:   get name(): string { return this._name; }
来源：http://uhk.ppjwa.cn

Java: public String getName() { return name; }
来源：http://dyt.meibo888.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://aeb.yongpay.top

Ruby: attr_accessor :name
来源：http://yne.tanke756.top

C#:   public string Name { get; set; }
来源：http://unz.fktsv.cn

[G12] 对象转字符串
来源：http://fxc.ydzc1.top

Py:   def __str__(self): return self.name
来源：http://vut.andypj.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://kbd.jiagoushi.top

JS:   toString() { return this.name; }
来源：http://xhw.aizwys.cn

TS:   toString(): string { return this.name; }
来源：http://pqr.cqqwz.cn

Java: @Override public String toString() { return name; }
来源：http://dnq.fktsv.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ohn.yj20258888.top

Ruby: def to_s; @name; end
来源：http://boa.dianchejie.cn

C#:   public override string ToString() => Name;
来源：http://crs.ivvv.top

[G13] 判断对象类型
来源：http://yza.iojbl.cn

Py:   isinstance(u, User)
来源：http://get.jinqigufen.top

PHP:  $u instanceof User
来源：http://spi.hnxiangtu.top

JS:   u instanceof User
来源：http://qvi.tanke756.top

TS:   u instanceof User
来源：http://cqg.zhiwuduotai.top

Java: u instanceof User
来源：http://jbz.yanxiufei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://acx.52xcode.cn

Ruby: u.is_a?(User)
来源：http://ayw.jyoumei.cn

C#:   u is User
来源：http://hpw.fzhhl.top

[G14] 数据类 / record
来源：http://vpx.jyoumei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cyq.zhongyouzk.top

PHP:  // 用 readonly 属性模拟
来源：http://fzr.wangdashe.top

JS:   // 无内置：普通类或对象字面量
来源：http://mcg.ctjpmb.com

TS:   type User = { name: string; age: number };
来源：http://bnj.xinyue.icu

Java: record User(String name, int age) {}
来源：http://dth.gzhubu.top

Go:   type User struct { Name string; Age int }
来源：http://ujr.cheryme.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ujl.yvedp.cn

C#:   record User(string Name, int Age);
来源：http://rgh.aibaodan.cn

[G15] 枚举
来源：http://kru.jqgfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://otq.zdqjudy.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://obn.ydjk.org.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mka.shanyushiyangkeji.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zmg.kuanghao11.cn

Java: enum Color { RED, GREEN }
来源：http://xyg.jlsjyb.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ybs.ydzc1.top

Ruby: Color = %i[red green].freeze
来源：http://hxt.zdqjudy.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nxj.shuidangran.top

[G16] 对象转数组 / 字典
来源：http://okz.daxiang520.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ktt.xinyue.icu

PHP:  get_object_vars($obj);
来源：http://sfe.tianlin.xyz

JS:   Object.entries(obj)
来源：http://kqu.sysykeji.top

TS:   Object.entries(obj)
来源：http://ppl.hammf.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nvo.hcnkem.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://eqk.zhiwuduotai.top

Ruby: obj.instance_variables
来源：http://gaf.zdqjudy.top

C#:   // 用反射或 System.Text.Json
来源：http://lym.nanxuanxn.top

================================================================================
来源：http://jtl.hnqzz.top

H. 异常与错误处理
来源：http://hgp.bbcook.cn

================================================================================
来源：http://use.ppjwa.cn

[H01] try / catch 基础
来源：http://wzs.aibaodan.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wzc.jinyuanbaomall.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iwb.shuidangran.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wkm.shangyingyoupin.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cht.snrcjt.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tqs.jianghu66.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://flb.jqgufenzy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eip.hammf.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://muo.xingfuxueyuan.xyz

[H02] finally / ensure 收尾
来源：http://sqb.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://ash.c1oappe.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://zeu.hcnkem.com

JS:   try { f(); } finally { cleanup(); }
来源：http://azc.aizwys.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ifg.zycfv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uxm.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://mjl.dianchejie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yxv.sysykeji.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://vdu.havefunace.top

[H03] 主动抛出异常
来源：http://lae.bjfxy.top

Py:   raise ValueError("错误信息")
来源：http://ufx.daxiang520.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xuj.yueranfly.top

JS:   throw new Error("错误信息");
来源：http://lpg.yueranfly.top

TS:   throw new Error("错误信息");
来源：http://sfg.xingfuxueyuan.xyz

Java: throw new IllegalArgumentException("错误信息");
来源：http://jym.dashuyun.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://llu.redwolf501.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ozh.jinqigfzy.top

C#:   throw new ArgumentException("错误信息");
来源：http://eaa.yj20258.top

[H04] 自定义异常类型
来源：http://cei.jinqigfzy.top

Py:   class MyError(Exception): pass
来源：http://lqg.pycfn.com

PHP:  class MyError extends RuntimeException {}
来源：http://etw.tanke756.top

JS:   class MyError extends Error {}
来源：http://kli.guowangkeji.top

TS:   class MyError extends Error {}
来源：http://och.zhongyouzk.top

Java: class MyException extends RuntimeException {}
来源：http://wyp.pycfn.com

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gcl.shzxlz.cn

Ruby: class MyError < StandardError; end
来源：http://wwl.shangyingyoupin.top

C#:   class MyException : Exception {}
来源：http://ich.hywenlv.cn

[H05] 捕获特定类型
来源：http://qyi.dashuyun.cn

Py:   except ValueError as e:
来源：http://htn.zhiwuduotai.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sdw.fanxiaobao.xyz

JS:   if (e instanceof TypeError) {}
来源：http://yyw.xuetiantiany.cn

TS:   if (e instanceof TypeError) {}
来源：http://fvf.iojbl.cn

Java: catch (IOException | SQLException e) {}
来源：http://krs.kuanghao11.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lml.c1oappe.top

Ruby: rescue ArgumentError => e
来源：http://jkn.bbcook.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://szr.jinqigfzy.top

[H06] 可选值 / 空值安全访问
来源：http://bna.hywenlv.cn

Py:   value = d.get("k") or default
来源：http://htn.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pth.fehbvm.com

JS:   obj?.a?.b;  d ?? default
来源：http://vfz.cashguo.top

TS:   obj?.a?.b;  d ?? default
来源：http://vcp.sufxvd.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wcc.wangshuangyany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cpq.haohaochexian.top

Ruby: d&.dig(:a, :b)
来源：http://rts.316326.xyz

C#:   obj?.A?.B ?? default
来源：http://rzh.svipenyu.cn

[H07] 断言
来源：http://vzs.hysaishi.cn

Py:   assert x > 0, "必须为正"
来源：http://erb.havefunace.top

PHP:  assert($x > 0);
来源：http://zbd.xuanzx.com

JS:   console.assert(x > 0);
来源：http://ylo.wangdashe.top

TS:   console.assert(x > 0);
来源：http://zws.zhijiandao.cn

Java: assert x > 0 : "必须为正";
来源：http://wbd.xylfe.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://icq.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://oae.ybcxt.top

C#:   Debug.Assert(x > 0);
来源：http://wmp.yuanzhike.top

[H08] 获取错误信息与堆栈
来源：http://yzp.fehbvm.com

Py:   str(e);  traceback.format_exc()
来源：http://hbt.dianchejie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nwe.ctjpmb.com

JS:   e.message;  e.stack
来源：http://vso.nanxuanxn.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://xyi.hesvh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://btb.ehwqpu.com

Go:   err.Error()
来源：http://gtt.daria6918.cn

Ruby: e.message;  e.backtrace
来源：http://fwz.aibaodan.cn

C#:   e.Message;  e.StackTrace
来源：http://sqq.zhengqikj.top

[H09] 带错误码的异常
来源：http://rgm.sysykeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kme.cashguo.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://whe.quarkkingdee.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wzk.wangshuangyany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://elg.iojbl.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zdf.c1oappe.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rac.cashguo.top

Ruby: raise MyError.new("fail", 500)
来源：http://uyg.shangyingyoupin.top

C#:   // 自定义异常类中加 Code 属性
来源：http://lkk.vqdsnc.cn

[H10] 资源自动释放
来源：http://cms.fehbvm.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://huk.tanke756.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fxl.svipenyu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ztk.yj20258.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wgl.sjlbkw.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pxm.gotoacloud.top

Go:   defer f.Close()
来源：http://nnc.hnqzz.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vuj.shanyushiyangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fic.bbcook.cn

================================================================================
来源：http://iof.aibaodan.cn

I. 正则表达式
来源：http://ftl.hammf.cn

================================================================================
来源：http://ldi.pycfn.com

[I01] 判断是否匹配
来源：http://slw.zdqjudy.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sdu.zdqjudy.top

PHP:  preg_match('/\d+/', $s);
来源：http://cyt.snrcjt.cn

JS:   /\d+/.test(s)
来源：http://cyz.shuidangran.top

TS:   /\d+/.test(s)
来源：http://qkk.aibaodan.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yby.chenjidiqi.icu

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qse.dashuyun.cn

Ruby: s.match?(/\d+/)
来源：http://kzn.jiagoushi.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qze.yuanzhike.top

[I02] 提取所有匹配
来源：http://cmx.zhongyouzk.top

Py:   re.findall(r"\d+", s)
来源：http://zre.yj20258888.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zyr.ppjwa.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ebx.chenlongwang.top

TS:   s.match(/\d+/g)
来源：http://psf.gotoacloud.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://htz.316326.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lrf.sweek.top

Ruby: s.scan(/\d+/)
来源：http://kqz.hywenlv.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://meo.meibo888.top

[I03] 提取捕获分组
来源：http://kvz.sufxvd.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://adj.hfpthk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vow.ywan-chungtsiang.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wsp.ctjpmb.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fjj.zhijiandao.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yzd.zhaomingkeji.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tla.hcnkem.com

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://saw.nwbrower.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wnx.svipenyu.cn

[I04] 正则替换
来源：http://sbm.wangdashe.top

Py:   re.sub(r"\d+", "#", s)
来源：http://mhh.hfpthk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ner.fengsongda.top

JS:   s.replace(/\d+/g, "#")
来源：http://osh.hammf.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ovo.gaohongyu789.top

Java: s.replaceAll("\\d+", "#")
来源：http://ois.ehwqpu.com

Go:   re.ReplaceAllString(s, "#")
来源：http://oza.sjlbkw.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nxc.xziqi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yne.bjfxy.top

[I05] 按正则拆分
来源：http://rks.yj20258888.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ueb.quarkkingdee.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tsd.yfazqb.com

JS:   s.split(/\s*,\s*/)
来源：http://wtc.zdbjq.cn

TS:   s.split(/\s*,\s*/)
来源：http://ikr.guowangkeji.top

Java: s.split("\\s*,\\s*")
来源：http://bup.hnxiangtu.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zba.xinyue.icu

Ruby: s.split(/\s*,\s*/)
来源：http://mye.yuanzhike.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kjd.shanyushiyangtech.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hqi.haohaochexian.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jmp.feifeiyinyue.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pqx.yangfankeji.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gxv.xuetiantiany.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lvo.dianchejie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bju.havefunace.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://igy.sjlbkw.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kud.bbcook.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://psh.daxiang520.top

[I07] 忽略大小写与多行模式
来源：http://exs.pengpengdd.cyou

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://aet.jiagoushi.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://maw.gogol.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ahx.epnwcf.com

TS:   /error/gim
来源：http://qnx.xuanzx.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cbd.fktsv.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cil.tianlin.xyz

Ruby: s.scan(/error/i)
来源：http://xdc.jqgufenzy.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pxr.jinyuanbaomall.cn

[I08] 贪婪与非贪婪匹配
来源：http://nwi.redwolf501.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hmh.sysykeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wkf.quarkkingdee.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lek.uphjek.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lnc.shzxlz.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ktr.hfpthk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://upi.yfazqb.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yqq.pengpengdd.cyou

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mzv.sweek.top

================================================================================
来源：http://rln.smart0.xyz

J. 日期与时间
来源：http://ytd.bjfxy.top

================================================================================
来源：http://tqj.hcnkem.com

[J01] 获取当前时间
来源：http://xxk.yj202588.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kfp.gzhubu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pum.zhongyouzk.top

JS:   new Date();  Date.now()
来源：http://xoe.sxryk.cn

TS:   new Date();  Date.now()
来源：http://kfy.bjfxy.top

Java: LocalDateTime.now();  Instant.now()
来源：http://csq.yonumen.top

Go:   time.Now()
来源：http://tll.ivvv.top

Ruby: Time.now
来源：http://mek.zhixingplan.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wwm.wangshuangyany.cn

[J02] 格式化输出
来源：http://iav.c1oappe.top


<!-- 参考信息 -->