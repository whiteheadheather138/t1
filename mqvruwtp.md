代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://cck.9152youxi.cn

[G03] 实例属性
来源：http://llt.ctjpmb.com

Py:   self.name = "x"
来源：http://ywg.shangyingyoupin.top

PHP:  public string $name = "x";
来源：http://qge.yonumen.top

JS:   this.name = "x";
来源：http://nyb.haohaochexian.top

TS:   name: string = "x";
来源：http://etl.ydjk.org.cn

Java: private String name;
来源：http://epv.zdbjq.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xez.hesvh.cn

Ruby: @name = "x"
来源：http://soq.snrcjt.cn

C#:   public string Name { get; set; } = "x";
来源：http://pco.pycfn.com

[G04] 定义方法
来源：http://uor.nwbrower.top

Py:   def greet(self): return self.name
来源：http://mdx.zhengqikj.top

PHP:  public function greet(): string { return $this->name; }
来源：http://awb.cheryme.top

JS:   greet() { return this.name; }
来源：http://hyd.pycfn.com

TS:   greet(): string { return this.name; }
来源：http://kpr.dianchejie.cn

Java: String greet() { return name; }
来源：http://rjc.vqdsnc.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wvf.0kj1m.cn

Ruby: def greet; @name; end
来源：http://ffc.cashguo.top

C#:   public string Greet() => Name;
来源：http://xfq.uphjek.com

[G05] 继承
来源：http://lgr.52xcode.cn

Py:   class Admin(User): pass
来源：http://wus.guowangkeji.top

PHP:  class Admin extends User {}
来源：http://xmk.jlsjyb.cn

JS:   class Admin extends User {}
来源：http://twd.vqdsnc.cn

TS:   class Admin extends User {}
来源：http://mkx.tianlin.xyz

Java: class Admin extends User {}
来源：http://zeo.birdmap.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mbm.tianlin.xyz

Ruby: class Admin < User; end
来源：http://iys.shzxlz.cn

C#:   class Admin : User {}
来源：http://mug.zhoulong.xyz

[G06] 重写方法
来源：http://lse.yj202588.top

Py:   def greet(self): return "admin"
来源：http://frk.sufxvd.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rsq.hongshengwenyu.top

JS:   greet() { return "admin"; }
来源：http://nmx.wangshuangyany.cn

TS:   greet(): string { return "admin"; }
来源：http://nez.dianchejie.cn

Java: @Override String greet() { return "admin"; }
来源：http://ywn.tanke756.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wyd.cqqwz.cn

Ruby: def greet; "admin"; end
来源：http://olm.uphjek.com

C#:   public override string Greet() => "admin";
来源：http://iup.cqqwz.cn

[G07] 调用父类方法
来源：http://iom.fehbvm.com

Py:   super().greet()
来源：http://rgm.c1oappe.top

PHP:  parent::greet();
来源：http://acp.hcnkem.com

JS:   super.greet();
来源：http://kvx.jqgfzy.top

TS:   super.greet();
来源：http://zop.xuetiantiany.cn

Java: super.greet();
来源：http://lyc.52xcode.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wgr.pengpengdd.cyou

Ruby: super
来源：http://fve.hammf.cn

C#:   base.Greet();
来源：http://rir.hesvh.cn

[G08] 静态方法与属性
来源：http://wqi.cheryme.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dpk.wangdashe.top

PHP:  public static function f() {}
来源：http://yry.vehdjk.com

JS:   static f() {}
来源：http://vny.hongshengwenyu.top

TS:   static f(): void {}
来源：http://abt.iojbl.cn

Java: static void f() {}
来源：http://gyz.xinyue.icu

Go:   // 无 static：用包级函数，按包名调用
来源：http://ukv.jyoumei.cn

Ruby: def self.f; end
来源：http://hgi.tian-w.cn

C#:   public static void F() {}
来源：http://ftt.yj20258888.top

[G09] 接口 / 抽象类
来源：http://sge.yuxming.cn

Py:   from abc import ABC, abstractmethod
来源：http://kic.gogol.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xog.zhaomingkeji.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://lhs.gzhubu.top

TS:   interface Shape { area(): number; }
来源：http://cyl.jinghuilouyu.cn

Java: interface Shape { double area(); }
来源：http://dod.hywenlv.cn

Go:   type Shape interface { Area() float64 }
来源：http://vmt.ybcxt.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://kmn.tarul.cn

C#:   interface IShape { double Area(); }
来源：http://aeh.haohaochexian.top

[G10] 访问控制
来源：http://drc.hnxiangtu.top

Py:   约定 _protected / __private（不强制）
来源：http://wdj.yongpay.top

PHP:  public / protected / private
来源：http://wuh.redwolf501.top

JS:   #private 字段；其余公开
来源：http://txr.cucudq.cn

TS:   public / protected / private
来源：http://zrl.cdnleiting.top

Java: public / protected / private / 默认包级
来源：http://tbi.ydzc1.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://txn.feifeiyinyue.top

Ruby: public / protected / private
来源：http://cdr.hywenlv.cn

C#:   public / protected / private / internal
来源：http://tuf.guannengcc.top

[G11] getter / setter
来源：http://wpq.ywan-chungtsiang.top

Py:   @property 与 @x.setter
来源：http://anq.havefunace.top

PHP:  public function getName(): string { return $this->name; }
来源：http://cpg.jinqigufen.top

JS:   get name() { return this._name; }
来源：http://xpo.fzhhl.top

TS:   get name(): string { return this._name; }
来源：http://aoo.nanxinkj.top

Java: public String getName() { return name; }
来源：http://snf.fktsv.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://esn.jinqigufen.top

Ruby: attr_accessor :name
来源：http://plf.xziqi.cn

C#:   public string Name { get; set; }
来源：http://eif.bbcook.cn

[G12] 对象转字符串
来源：http://fme.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://hav.sufxvd.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://puf.nanxuanxn.top

JS:   toString() { return this.name; }
来源：http://nrv.pycfn.com

TS:   toString(): string { return this.name; }
来源：http://chu.aibaodan.cn

Java: @Override public String toString() { return name; }
来源：http://zss.yongpay.top

Go:   func (u User) String() string { return u.Name }
来源：http://kpy.dianchejie.cn

Ruby: def to_s; @name; end
来源：http://tlw.kuanghao11.cn

C#:   public override string ToString() => Name;
来源：http://ioz.jlsjyb.cn

[G13] 判断对象类型
来源：http://qsi.wangdashe.top

Py:   isinstance(u, User)
来源：http://nkm.yvedp.cn

PHP:  $u instanceof User
来源：http://enn.zhixingplan.top

JS:   u instanceof User
来源：http://bqm.yj20258.top

TS:   u instanceof User
来源：http://vxg.gotoacloud.top

Java: u instanceof User
来源：http://yru.shangyingyoupin.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://xzv.jqgufenzy.top

Ruby: u.is_a?(User)
来源：http://ibz.nanxuanxn.top

C#:   u is User
来源：http://uzh.kuanghao11.cn

[G14] 数据类 / record
来源：http://tma.epnwcf.com

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gfo.jinqigfzy.top

PHP:  // 用 readonly 属性模拟
来源：http://lco.guowangkeji.top

JS:   // 无内置：普通类或对象字面量
来源：http://hnu.0kj1m.cn

TS:   type User = { name: string; age: number };
来源：http://shi.cqqwz.cn

Java: record User(String name, int age) {}
来源：http://mkf.pengpengdd.cyou

Go:   type User struct { Name string; Age int }
来源：http://dif.fengsongda.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fwk.cheryme.top

C#:   record User(string Name, int Age);
来源：http://qhl.dianchejie.cn

[G15] 枚举
来源：http://ztw.xylfe.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wxa.jinqigufen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://dec.xingfuxueyuan.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://grw.0kj1m.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://shx.shanyushiyangtech.top

Java: enum Color { RED, GREEN }
来源：http://dzs.cashguo.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://umv.yonumen.top

Ruby: Color = %i[red green].freeze
来源：http://cwi.zhongyouzk.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ffo.cdnleiting.top

[G16] 对象转数组 / 字典
来源：http://rqj.andypj.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vbx.havefunace.top

PHP:  get_object_vars($obj);
来源：http://obl.haohaochexian.top

JS:   Object.entries(obj)
来源：http://ogk.dashuyun.cn

TS:   Object.entries(obj)
来源：http://itu.zhengqikj.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jtv.zdqjudy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://hlk.jinyuanbaomall.cn

Ruby: obj.instance_variables
来源：http://guh.hfpthk.cn

C#:   // 用反射或 System.Text.Json
来源：http://xsm.cashguo.top

================================================================================
来源：http://kuf.snrcjt.cn

H. 异常与错误处理
来源：http://ril.zdqjudy.top

================================================================================
来源：http://tdu.gogol.net.cn

[H01] try / catch 基础
来源：http://gll.ywan-chungtsiang.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://udu.9152youxi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ckn.jinqigufen.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lqe.mhx1999.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xgg.yj202588.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://acg.ywan-chungtsiang.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vcl.cashguo.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jyf.chenzaomai.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nwu.ybcxt.top

[H02] finally / ensure 收尾
来源：http://yty.zhoulong.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://xrl.yj202588.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ssm.nwbrower.top

JS:   try { f(); } finally { cleanup(); }
来源：http://uqm.9152youxi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nab.jinghuilouyu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ngl.ybcxt.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://unh.sxryk.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cka.aizwys.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ajx.nanxinkj.top

[H03] 主动抛出异常
来源：http://wps.jqgufenzy.top

Py:   raise ValueError("错误信息")
来源：http://bia.jianghu66.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nfg.xuetiantiany.cn

JS:   throw new Error("错误信息");
来源：http://tjm.haohaochexian.top

TS:   throw new Error("错误信息");
来源：http://spn.uphjek.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://abh.xingfuxueyuan.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zjk.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pbq.sjlbkw.cn

C#:   throw new ArgumentException("错误信息");
来源：http://umy.jiagoushi.top

[H04] 自定义异常类型
来源：http://byv.jinqigufen.top

Py:   class MyError(Exception): pass
来源：http://ayb.hnxiangtu.top

PHP:  class MyError extends RuntimeException {}
来源：http://kgu.yvedp.cn

JS:   class MyError extends Error {}
来源：http://evf.bbcook.cn

TS:   class MyError extends Error {}
来源：http://coi.52xcode.cn

Java: class MyException extends RuntimeException {}
来源：http://cit.tian-w.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uvg.andypj.xyz

Ruby: class MyError < StandardError; end
来源：http://brq.yonumen.top

C#:   class MyException : Exception {}
来源：http://ahg.aizwys.cn

[H05] 捕获特定类型
来源：http://jqg.sweek.top

Py:   except ValueError as e:
来源：http://xyu.yongpay.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ett.ydzc1.top

JS:   if (e instanceof TypeError) {}
来源：http://txy.nanxuanxn.top

TS:   if (e instanceof TypeError) {}
来源：http://ldm.c1oappe.top

Java: catch (IOException | SQLException e) {}
来源：http://oli.fzhhl.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cvy.hongshengwenyu.top

Ruby: rescue ArgumentError => e
来源：http://ncu.0kj1m.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://plg.fzhhl.top

[H06] 可选值 / 空值安全访问
来源：http://pxc.guannengcc.top

Py:   value = d.get("k") or default
来源：http://zhq.mhx1999.top

PHP:  $v = $d["k"] ?? null;
来源：http://irz.yueranfly.top

JS:   obj?.a?.b;  d ?? default
来源：http://els.hfpthk.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qkn.ivvv.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uar.xuetiantiany.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jyo.zhiwuduotai.top

Ruby: d&.dig(:a, :b)
来源：http://wfe.cucudq.cn

C#:   obj?.A?.B ?? default
来源：http://zrw.birdmap.top

[H07] 断言
来源：http://mhg.c1oappe.top

Py:   assert x > 0, "必须为正"
来源：http://wth.shuidangran.top

PHP:  assert($x > 0);
来源：http://jnr.nanxinkj.top

JS:   console.assert(x > 0);
来源：http://uuy.xylfe.cn

TS:   console.assert(x > 0);
来源：http://hjq.daria6918.cn

Java: assert x > 0 : "必须为正";
来源：http://dhy.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://voz.svipenyu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gae.yonumen.top

C#:   Debug.Assert(x > 0);
来源：http://atd.jianghu66.top

[H08] 获取错误信息与堆栈
来源：http://nta.9152youxi.cn

Py:   str(e);  traceback.format_exc()
来源：http://efc.zhengqikj.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://axm.jqgfzy.top

JS:   e.message;  e.stack
来源：http://zsj.xingfuxueyuan.xyz

TS:   e instanceof Error ? e.message : String(e)
来源：http://xgn.hcnkem.com

Java: e.getMessage();  e.printStackTrace()
来源：http://npj.ydzc1.top

Go:   err.Error()
来源：http://lvq.shangyingyoupin.top

Ruby: e.message;  e.backtrace
来源：http://jvn.fktsv.cn

C#:   e.Message;  e.StackTrace
来源：http://yrg.gzhubu.top

[H09] 带错误码的异常
来源：http://dih.daria6918.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mpv.shanyushiyangtech.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://mfl.jlsjyb.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yor.fengsongda.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rdb.jianghu66.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ank.yuanzhike.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jgg.jyoumei.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dlu.chenjidiqi.icu

C#:   // 自定义异常类中加 Code 属性
来源：http://mut.sufxvd.cn

[H10] 资源自动释放
来源：http://mho.ehwqpu.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://bwh.iojbl.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ina.ydzc1.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fvv.jinqigufen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kfb.jinqigufen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xpm.ybcxt.top

Go:   defer f.Close()
来源：http://kyj.yuanzhike.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gxk.jianghu66.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cpa.c1oappe.top

================================================================================
来源：http://qcu.hcnkem.com

I. 正则表达式
来源：http://yiv.yonumen.top

================================================================================
来源：http://aes.fanxiaobao.xyz

[I01] 判断是否匹配
来源：http://pgi.iojbl.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wle.yj20258.top

PHP:  preg_match('/\d+/', $s);
来源：http://vch.yuxming.cn

JS:   /\d+/.test(s)
来源：http://vvh.bjfxy.top

TS:   /\d+/.test(s)
来源：http://nwf.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://esv.jinqigfzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bfo.ppjwa.cn

Ruby: s.match?(/\d+/)
来源：http://zbq.cqqwz.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mru.gotoacloud.top

[I02] 提取所有匹配
来源：http://qjb.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://xrv.xziqi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rre.xuetiantiany.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bxx.ctjpmb.com

TS:   s.match(/\d+/g)
来源：http://eyr.ydzc1.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tuf.iojbl.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oge.aizwys.cn

Ruby: s.scan(/\d+/)
来源：http://hra.sxryk.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lxl.uphjek.com

[I03] 提取捕获分组
来源：http://pbv.shanyushiyangtech.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wme.zhoulong.xyz

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ywn.feifeiyinyue.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ztu.redwolf501.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nms.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oxm.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rgd.yonumen.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mwa.aibaodan.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kvj.hammf.cn

[I04] 正则替换
来源：http://opi.ehwqpu.com

Py:   re.sub(r"\d+", "#", s)
来源：http://nta.dianchejie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zxo.ydzc1.top

JS:   s.replace(/\d+/g, "#")
来源：http://ghr.nanxinkj.top

TS:   s.replace(/\d+/g, "#")
来源：http://hjm.hfpthk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vol.daxiang520.top

Go:   re.ReplaceAllString(s, "#")
来源：http://jxm.xuanzx.com

Ruby: s.gsub(/\d+/, "#")
来源：http://uct.shanyushiyangkeji.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yeu.zdqjudy.top

[I05] 按正则拆分
来源：http://bri.yvedp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fow.yueranfly.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qvs.hammf.cn

JS:   s.split(/\s*,\s*/)
来源：http://ndx.hfpthk.cn

TS:   s.split(/\s*,\s*/)
来源：http://oga.zhengqikj.top

Java: s.split("\\s*,\\s*")
来源：http://ykn.feifeiyinyue.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cqh.yvedp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nhn.bjfxy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dyi.0kj1m.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wik.jinqigufen.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bsp.jinqigufen.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ebh.sweek.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xwj.fanxiaobao.xyz

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://web.yj20258.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lvg.fengsongda.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ede.mhx1999.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qbn.shuidangran.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sxf.shangyingyoupin.top

[I07] 忽略大小写与多行模式
来源：http://ijt.zhijiandao.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pbz.zhaomingkeji.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vdt.vehdjk.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dty.sweek.top

TS:   /error/gim
来源：http://uex.nanxuanxn.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cte.ppjwa.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://maz.cheryme.top

Ruby: s.scan(/error/i)
来源：http://wsy.xinyue.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mbw.daxiang520.top

[I08] 贪婪与非贪婪匹配
来源：http://rps.xziqi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yii.birdmap.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pee.yangfankeji.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pym.guowangkeji.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pjo.fengsongda.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://skm.hammf.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dqd.dianchejie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tsd.iojbl.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://das.xinyue.icu

================================================================================
来源：http://nfq.svipenyu.cn

J. 日期与时间
来源：http://jff.andypj.xyz

================================================================================
来源：http://sme.chenlongwang.top

[J01] 获取当前时间
来源：http://nkq.yfazqb.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://lgs.snrcjt.cn


<!-- 参考信息 -->