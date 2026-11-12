代发 wailian999

Ruby: @name = "x"
来源：http://fth.xziqi.cn

C#:   public string Name { get; set; } = "x";
来源：http://jlh.sufxvd.cn

[G04] 定义方法
来源：http://mga.hcnkem.com

Py:   def greet(self): return self.name
来源：http://zes.xziqi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zfc.xinyue.icu

JS:   greet() { return this.name; }
来源：http://apz.fengsongda.top

TS:   greet(): string { return this.name; }
来源：http://wbl.vqdsnc.cn

Java: String greet() { return name; }
来源：http://nbd.guannengcc.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://nnp.fengsongda.top

Ruby: def greet; @name; end
来源：http://tql.jiagoushi.top

C#:   public string Greet() => Name;
来源：http://vlg.yj202588.top

[G05] 继承
来源：http://pee.daria6918.cn

Py:   class Admin(User): pass
来源：http://wju.316326.xyz

PHP:  class Admin extends User {}
来源：http://ytv.dianchejie.cn

JS:   class Admin extends User {}
来源：http://brp.meibo888.top

TS:   class Admin extends User {}
来源：http://lpe.ppjwa.cn

Java: class Admin extends User {}
来源：http://hry.chenjidiqi.icu

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bdn.dashuyun.cn

Ruby: class Admin < User; end
来源：http://rsr.jinghuilouyu.cn

C#:   class Admin : User {}
来源：http://dpd.jqgufenzy.top

[G06] 重写方法
来源：http://sch.hnxiangtu.top

Py:   def greet(self): return "admin"
来源：http://ypd.shanyushiyangkeji.top

PHP:  public function greet(): string { return "admin"; }
来源：http://msi.jinghuilouyu.cn

JS:   greet() { return "admin"; }
来源：http://lpd.nanxuanxn.top

TS:   greet(): string { return "admin"; }
来源：http://btd.vehdjk.com

Java: @Override String greet() { return "admin"; }
来源：http://kev.xylfe.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dmn.yj202588.top

Ruby: def greet; "admin"; end
来源：http://abj.snrcjt.cn

C#:   public override string Greet() => "admin";
来源：http://got.bjfxy.top

[G07] 调用父类方法
来源：http://yxl.cheryme.top

Py:   super().greet()
来源：http://vbf.dianchejie.cn

PHP:  parent::greet();
来源：http://prw.pengpengdd.cyou

JS:   super.greet();
来源：http://ggx.zhaomingkeji.xyz

TS:   super.greet();
来源：http://thf.epnwcf.com

Java: super.greet();
来源：http://gwt.mhx1999.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sfl.quarkkingdee.top

Ruby: super
来源：http://gbb.ehwqpu.com

C#:   base.Greet();
来源：http://smu.gaohongyu789.top

[G08] 静态方法与属性
来源：http://nur.tarul.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://atp.hysaishi.cn

PHP:  public static function f() {}
来源：http://med.zhiwuduotai.top

JS:   static f() {}
来源：http://qqk.yvedp.cn

TS:   static f(): void {}
来源：http://yaz.quarkkingdee.top

Java: static void f() {}
来源：http://boq.jiagoushi.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://krv.yongpay.top

Ruby: def self.f; end
来源：http://gfa.vqdsnc.cn

C#:   public static void F() {}
来源：http://cbt.jiagoushi.top

[G09] 接口 / 抽象类
来源：http://ykt.birdmap.top

Py:   from abc import ABC, abstractmethod
来源：http://bfq.xinyue.icu

PHP:  interface Shape { public function area(): float; }
来源：http://hxi.fehbvm.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://zjy.fzhhl.top

TS:   interface Shape { area(): number; }
来源：http://zyc.tianlin.xyz

Java: interface Shape { double area(); }
来源：http://qpj.chenjidiqi.icu

Go:   type Shape interface { Area() float64 }
来源：http://qgg.xinyue.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cev.zhiwuduotai.top

C#:   interface IShape { double Area(); }
来源：http://vdz.tarul.cn

[G10] 访问控制
来源：http://hsf.hongshengwenyu.top

Py:   约定 _protected / __private（不强制）
来源：http://jec.sufxvd.cn

PHP:  public / protected / private
来源：http://hxf.hysaishi.cn

JS:   #private 字段；其余公开
来源：http://gmt.pengpengdd.cyou

TS:   public / protected / private
来源：http://fra.svipenyu.cn

Java: public / protected / private / 默认包级
来源：http://psp.ybcxt.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://hdt.xinyue.icu

Ruby: public / protected / private
来源：http://uuf.ctjpmb.com

C#:   public / protected / private / internal
来源：http://tej.hnqzz.top

[G11] getter / setter
来源：http://uhy.cucudq.cn

Py:   @property 与 @x.setter
来源：http://eim.pycfn.com

PHP:  public function getName(): string { return $this->name; }
来源：http://aeg.hcnkem.com

JS:   get name() { return this._name; }
来源：http://mvk.gogol.net.cn

TS:   get name(): string { return this._name; }
来源：http://pmm.316326.xyz

Java: public String getName() { return name; }
来源：http://wwh.gogol.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wmu.tarul.cn

Ruby: attr_accessor :name
来源：http://ivo.birdmap.top

C#:   public string Name { get; set; }
来源：http://bct.vqdsnc.cn

[G12] 对象转字符串
来源：http://utu.nanxinkj.top

Py:   def __str__(self): return self.name
来源：http://ggl.meibo888.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://yeh.feifeiyinyue.top

JS:   toString() { return this.name; }
来源：http://cwn.snrcjt.cn

TS:   toString(): string { return this.name; }
来源：http://qsv.jlsjyb.cn

Java: @Override public String toString() { return name; }
来源：http://oxy.tarul.cn

Go:   func (u User) String() string { return u.Name }
来源：http://amo.birdmap.top

Ruby: def to_s; @name; end
来源：http://tyg.hysaishi.cn

C#:   public override string ToString() => Name;
来源：http://pwp.gotoacloud.top

[G13] 判断对象类型
来源：http://kio.sufxvd.cn

Py:   isinstance(u, User)
来源：http://qyx.hongshengwenyu.top

PHP:  $u instanceof User
来源：http://tlf.xuanzx.com

JS:   u instanceof User
来源：http://ynw.fengsongda.top

TS:   u instanceof User
来源：http://wzc.gaohongyu789.top

Java: u instanceof User
来源：http://jui.nanxuanxn.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gou.jinghuilouyu.cn

Ruby: u.is_a?(User)
来源：http://fui.gogol.net.cn

C#:   u is User
来源：http://iij.xuetiantiany.cn

[G14] 数据类 / record
来源：http://xhh.jyoumei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dfc.yanxiufei.cn

PHP:  // 用 readonly 属性模拟
来源：http://gou.wangshuangyany.cn

JS:   // 无内置：普通类或对象字面量
来源：http://byn.nanxuanxn.top

TS:   type User = { name: string; age: number };
来源：http://rfv.hysaishi.cn

Java: record User(String name, int age) {}
来源：http://tch.shanyushiyangkeji.top

Go:   type User struct { Name string; Age int }
来源：http://mtx.vqdsnc.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dwd.jqgfzy.top

C#:   record User(string Name, int Age);
来源：http://iuv.zdqjudy.top

[G15] 枚举
来源：http://mbw.fanxiaobao.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rte.9152youxi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lqa.yongpay.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mlz.dianchejie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vra.yfazqb.com

Java: enum Color { RED, GREEN }
来源：http://blk.zhongyouzk.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://btw.yj20258888.top

Ruby: Color = %i[red green].freeze
来源：http://yvt.hcnkem.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wpx.wangshuangyany.cn

[G16] 对象转数组 / 字典
来源：http://nbq.havefunace.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tvt.vehdjk.com

PHP:  get_object_vars($obj);
来源：http://gcf.fehbvm.com

JS:   Object.entries(obj)
来源：http://nut.hfpthk.cn

TS:   Object.entries(obj)
来源：http://udh.kuanghao11.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qjn.316326.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://qew.pycfn.com

Ruby: obj.instance_variables
来源：http://thd.jinyuanbaomall.cn

C#:   // 用反射或 System.Text.Json
来源：http://dma.yuanzhike.top

================================================================================
来源：http://wjv.hcnkem.com

H. 异常与错误处理
来源：http://rlb.ivvv.top

================================================================================
来源：http://ngx.jyoumei.cn

[H01] try / catch 基础
来源：http://gtg.yonumen.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ree.yvedp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://upu.yangfankeji.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bgb.cashguo.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yph.jqgufenzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ylu.xinyue.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kyj.uphjek.com

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gse.zhongyouzk.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pjo.jqgfzy.top

[H02] finally / ensure 收尾
来源：http://oaa.sweek.top

Py:   try: f()⏎finally: cleanup()
来源：http://isr.bjfxy.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ufz.fktsv.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jsu.9152youxi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xqx.kuanghao11.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pwe.cdnleiting.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://sum.ydzc1.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ujf.ybcxt.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://bss.tanke756.top

[H03] 主动抛出异常
来源：http://wqc.ybcxt.top

Py:   raise ValueError("错误信息")
来源：http://edv.redwolf501.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ozt.sufxvd.cn

JS:   throw new Error("错误信息");
来源：http://tej.zycfv.cn

TS:   throw new Error("错误信息");
来源：http://ckl.jinyuanbaomall.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nja.aibaodan.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mec.uphjek.com

Ruby: raise ArgumentError, "错误信息"
来源：http://cuw.hysaishi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kzz.yj202588.top

[H04] 自定义异常类型
来源：http://agm.mhx1999.top

Py:   class MyError(Exception): pass
来源：http://yuw.zhixingplan.top

PHP:  class MyError extends RuntimeException {}
来源：http://mre.zhijiandao.cn

JS:   class MyError extends Error {}
来源：http://axq.gogol.net.cn

TS:   class MyError extends Error {}
来源：http://dry.xuanzx.com

Java: class MyException extends RuntimeException {}
来源：http://cia.hammf.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cco.vehdjk.com

Ruby: class MyError < StandardError; end
来源：http://fwn.yuanzhike.top

C#:   class MyException : Exception {}
来源：http://gci.fehbvm.com

[H05] 捕获特定类型
来源：http://hex.zhongyouzk.top

Py:   except ValueError as e:
来源：http://dgm.zhixingplan.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hsr.fehbvm.com

JS:   if (e instanceof TypeError) {}
来源：http://gvb.guannengcc.top

TS:   if (e instanceof TypeError) {}
来源：http://jve.uphjek.com

Java: catch (IOException | SQLException e) {}
来源：http://ekr.tianlin.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mqq.sysykeji.top

Ruby: rescue ArgumentError => e
来源：http://brp.hnxiangtu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hss.ctjpmb.com

[H06] 可选值 / 空值安全访问
来源：http://eyc.yueranfly.top

Py:   value = d.get("k") or default
来源：http://qkq.daxiang520.top

PHP:  $v = $d["k"] ?? null;
来源：http://rxk.gzhubu.top

JS:   obj?.a?.b;  d ?? default
来源：http://bgf.zhaomingkeji.xyz

TS:   obj?.a?.b;  d ?? default
来源：http://sqi.fengsongda.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rmt.tanke756.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ayb.chenlongwang.top

Ruby: d&.dig(:a, :b)
来源：http://sdp.andypj.xyz

C#:   obj?.A?.B ?? default
来源：http://com.xylfe.cn

[H07] 断言
来源：http://hqq.cucudq.cn

Py:   assert x > 0, "必须为正"
来源：http://nxe.hammf.cn

PHP:  assert($x > 0);
来源：http://aht.haohaochexian.top

JS:   console.assert(x > 0);
来源：http://ang.jinqigfzy.top

TS:   console.assert(x > 0);
来源：http://xvl.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://vth.gaohongyu789.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pku.havefunace.top

Ruby: raise "必须为正" unless x > 0
来源：http://srm.andypj.xyz

C#:   Debug.Assert(x > 0);
来源：http://aid.yuxming.cn

[H08] 获取错误信息与堆栈
来源：http://hfi.c1oappe.top

Py:   str(e);  traceback.format_exc()
来源：http://hsr.aibaodan.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jzx.tanke756.top

JS:   e.message;  e.stack
来源：http://hhb.gaohongyu789.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://omr.yj20258888.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ldz.yj202588.top

Go:   err.Error()
来源：http://uud.mhx1999.top

Ruby: e.message;  e.backtrace
来源：http://iyo.feifeiyinyue.top

C#:   e.Message;  e.StackTrace
来源：http://gnt.birdmap.top

[H09] 带错误码的异常
来源：http://aml.sweek.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wil.cucudq.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cwa.wangshuangyany.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nrv.feifeiyinyue.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mxu.yj202588.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wmy.guannengcc.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lzz.shzxlz.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xnk.shuidangran.top

C#:   // 自定义异常类中加 Code 属性
来源：http://fkz.wangshuangyany.cn

[H10] 资源自动释放
来源：http://atj.birdmap.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://epb.xuanzx.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://woa.yfazqb.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bgz.shangyingyoupin.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ifg.guowangkeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nmd.jianghu66.top

Go:   defer f.Close()
来源：http://hcu.ywan-chungtsiang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fac.sysykeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ctv.hysaishi.cn

================================================================================
来源：http://jqh.jiagoushi.top

I. 正则表达式
来源：http://dqw.xuetiantiany.cn

================================================================================
来源：http://bnm.yongpay.top

[I01] 判断是否匹配
来源：http://hbb.cheryme.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kpo.hongshengwenyu.top

PHP:  preg_match('/\d+/', $s);
来源：http://uxc.gzhubu.top

JS:   /\d+/.test(s)
来源：http://art.jyoumei.cn

TS:   /\d+/.test(s)
来源：http://bus.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://omz.jqgufenzy.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wur.cheryme.top

Ruby: s.match?(/\d+/)
来源：http://wjd.guowangkeji.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tsl.ydzc1.top

[I02] 提取所有匹配
来源：http://axt.tarul.cn

Py:   re.findall(r"\d+", s)
来源：http://asa.hammf.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bat.zhiwuduotai.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yuo.yuxming.cn

TS:   s.match(/\d+/g)
来源：http://adn.bbcook.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bsi.yangfankeji.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wox.yuanzhike.top

Ruby: s.scan(/\d+/)
来源：http://ojz.ydzc1.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jsy.yj20258888.top

[I03] 提取捕获分组
来源：http://zmv.vehdjk.com

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fao.zdqjudy.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pjd.sysykeji.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ydq.c1oappe.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nxt.zycfv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bme.hcnkem.com

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tti.yvedp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://afy.sxryk.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://okp.cheryme.top

[I04] 正则替换
来源：http://dae.tarul.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vpy.iojbl.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ack.nanxuanxn.top

JS:   s.replace(/\d+/g, "#")
来源：http://rag.bjfxy.top

TS:   s.replace(/\d+/g, "#")
来源：http://qxc.xinyue.icu

Java: s.replaceAll("\\d+", "#")
来源：http://pxz.birdmap.top

Go:   re.ReplaceAllString(s, "#")
来源：http://htc.mhx1999.top

Ruby: s.gsub(/\d+/, "#")
来源：http://exv.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yck.vehdjk.com

[I05] 按正则拆分
来源：http://koz.xziqi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wnl.nwbrower.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ifo.snrcjt.cn

JS:   s.split(/\s*,\s*/)
来源：http://vdv.feifeiyinyue.top

TS:   s.split(/\s*,\s*/)
来源：http://vqs.vqdsnc.cn

Java: s.split("\\s*,\\s*")
来源：http://xef.xziqi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bvj.0kj1m.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nln.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://omz.yvedp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aex.aizwys.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gyg.gogol.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eid.cheryme.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://inc.gaohongyu789.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://msv.xingfuxueyuan.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://evs.yanxiufei.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xik.0kj1m.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tkt.c1oappe.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rty.ydzc1.top

[I07] 忽略大小写与多行模式
来源：http://lal.316326.xyz

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iwp.zhengqikj.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uwh.sweek.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ffq.sufxvd.cn

TS:   /error/gim
来源：http://lfs.vqdsnc.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ypi.sjlbkw.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lqj.pycfn.com

Ruby: s.scan(/error/i)
来源：http://mqy.jinghuilouyu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jti.yj20258888.top

[I08] 贪婪与非贪婪匹配
来源：http://huw.jyoumei.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://epz.pycfn.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tty.hnqzz.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fwb.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jut.gotoacloud.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://uwq.dashuyun.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ucf.jyoumei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mzq.cucudq.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wiv.fktsv.cn

================================================================================
来源：http://mmv.chenzaomai.com

J. 日期与时间
来源：http://nrf.meibo888.top

================================================================================
来源：http://elr.quarkkingdee.top

[J01] 获取当前时间
来源：http://lcq.xingfuxueyuan.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://nzy.jlsjyb.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ado.nanxinkj.top

JS:   new Date();  Date.now()
来源：http://iog.gogol.net.cn

TS:   new Date();  Date.now()
来源：http://goe.ivvv.top

Java: LocalDateTime.now();  Instant.now()
来源：http://tkl.ybcxt.top

Go:   time.Now()
来源：http://prv.yangfankeji.com

Ruby: Time.now
来源：http://tzt.zycfv.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qah.dianchejie.cn

[J02] 格式化输出
来源：http://tsb.tanke756.top


<!-- 参考信息 -->