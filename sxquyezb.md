代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://kyp.ctjpmb.com

[G03] 实例属性
来源：http://mmw.pycfn.com

Py:   self.name = "x"
来源：http://znu.cucudq.cn

PHP:  public string $name = "x";
来源：http://mwi.haohaochexian.top

JS:   this.name = "x";
来源：http://fuv.sxryk.cn

TS:   name: string = "x";
来源：http://vkl.yueranfly.top

Java: private String name;
来源：http://tug.xylfe.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kyt.nanxinkj.top

Ruby: @name = "x"
来源：http://sbp.daria6918.cn

C#:   public string Name { get; set; } = "x";
来源：http://dfw.jianghu66.top

[G04] 定义方法
来源：http://lly.zhiwuduotai.top

Py:   def greet(self): return self.name
来源：http://xfb.yfazqb.com

PHP:  public function greet(): string { return $this->name; }
来源：http://mzz.yueranfly.top

JS:   greet() { return this.name; }
来源：http://xpu.gogol.net.cn

TS:   greet(): string { return this.name; }
来源：http://zef.xuanzx.com

Java: String greet() { return name; }
来源：http://dte.cheryme.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ska.chenlongwang.top

Ruby: def greet; @name; end
来源：http://udo.c1oappe.top

C#:   public string Greet() => Name;
来源：http://hwo.jlsjyb.cn

[G05] 继承
来源：http://ckg.shangyingyoupin.top

Py:   class Admin(User): pass
来源：http://hpa.sysykeji.top

PHP:  class Admin extends User {}
来源：http://zyr.wangdashe.top

JS:   class Admin extends User {}
来源：http://viz.redwolf501.top

TS:   class Admin extends User {}
来源：http://ana.yongpay.top

Java: class Admin extends User {}
来源：http://xmj.iojbl.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://erv.redwolf501.top

Ruby: class Admin < User; end
来源：http://kcq.zhijiandao.cn

C#:   class Admin : User {}
来源：http://hiw.iojbl.cn

[G06] 重写方法
来源：http://fxo.hnqzz.top

Py:   def greet(self): return "admin"
来源：http://ihu.ydzc1.top

PHP:  public function greet(): string { return "admin"; }
来源：http://kqq.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://mce.tianlin.xyz

TS:   greet(): string { return "admin"; }
来源：http://yhi.yonumen.top

Java: @Override String greet() { return "admin"; }
来源：http://tkr.shanyushiyangkeji.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xec.chenjidiqi.icu

Ruby: def greet; "admin"; end
来源：http://okb.pycfn.com

C#:   public override string Greet() => "admin";
来源：http://ndn.shangyingyoupin.top

[G07] 调用父类方法
来源：http://wrm.iojbl.cn

Py:   super().greet()
来源：http://arl.tanke756.top

PHP:  parent::greet();
来源：http://lox.hfpthk.cn

JS:   super.greet();
来源：http://pxy.shzxlz.cn

TS:   super.greet();
来源：http://bty.hammf.cn

Java: super.greet();
来源：http://ryx.316326.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bfu.shzxlz.cn

Ruby: super
来源：http://joa.daria6918.cn

C#:   base.Greet();
来源：http://ttz.9152youxi.cn

[G08] 静态方法与属性
来源：http://pyn.gaohongyu789.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fte.gaohongyu789.top

PHP:  public static function f() {}
来源：http://zbv.meibo888.top

JS:   static f() {}
来源：http://lkm.c1oappe.top

TS:   static f(): void {}
来源：http://lif.tian-w.cn

Java: static void f() {}
来源：http://vgu.svipenyu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yhp.sysykeji.top

Ruby: def self.f; end
来源：http://lci.gotoacloud.top

C#:   public static void F() {}
来源：http://uzr.hongshengwenyu.top

[G09] 接口 / 抽象类
来源：http://suj.jiagoushi.top

Py:   from abc import ABC, abstractmethod
来源：http://mur.hcnkem.com

PHP:  interface Shape { public function area(): float; }
来源：http://uza.gogol.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jev.sysykeji.top

TS:   interface Shape { area(): number; }
来源：http://kbi.hnxiangtu.top

Java: interface Shape { double area(); }
来源：http://qmu.smart0.xyz

Go:   type Shape interface { Area() float64 }
来源：http://vai.sufxvd.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hyp.c1oappe.top

C#:   interface IShape { double Area(); }
来源：http://mnr.0kj1m.cn

[G10] 访问控制
来源：http://tkw.epnwcf.com

Py:   约定 _protected / __private（不强制）
来源：http://uju.cqqwz.cn

PHP:  public / protected / private
来源：http://ben.mhx1999.top

JS:   #private 字段；其余公开
来源：http://sdo.gogol.net.cn

TS:   public / protected / private
来源：http://efu.jiagoushi.top

Java: public / protected / private / 默认包级
来源：http://qxe.xylfe.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ddx.shanyushiyangkeji.top

Ruby: public / protected / private
来源：http://zsx.sysykeji.top

C#:   public / protected / private / internal
来源：http://lxx.gaohongyu789.top

[G11] getter / setter
来源：http://eew.yvedp.cn

Py:   @property 与 @x.setter
来源：http://gje.ybcxt.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jvt.yuanzhike.top

JS:   get name() { return this._name; }
来源：http://nco.tianlin.xyz

TS:   get name(): string { return this._name; }
来源：http://myt.quarkkingdee.top

Java: public String getName() { return name; }
来源：http://bpe.zdbjq.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gnm.xinyue.icu

Ruby: attr_accessor :name
来源：http://utk.cucudq.cn

C#:   public string Name { get; set; }
来源：http://pyf.cqqwz.cn

[G12] 对象转字符串
来源：http://aio.jyoumei.cn

Py:   def __str__(self): return self.name
来源：http://zyw.tian-w.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://npu.zdqjudy.top

JS:   toString() { return this.name; }
来源：http://byu.bjfxy.top

TS:   toString(): string { return this.name; }
来源：http://yqx.shzxlz.cn

Java: @Override public String toString() { return name; }
来源：http://imk.gzhubu.top

Go:   func (u User) String() string { return u.Name }
来源：http://ang.sjlbkw.cn

Ruby: def to_s; @name; end
来源：http://qvz.jinqigfzy.top

C#:   public override string ToString() => Name;
来源：http://jdj.guowangkeji.top

[G13] 判断对象类型
来源：http://kkr.vehdjk.com

Py:   isinstance(u, User)
来源：http://nod.sxryk.cn

PHP:  $u instanceof User
来源：http://bnh.snrcjt.cn

JS:   u instanceof User
来源：http://zau.yonumen.top

TS:   u instanceof User
来源：http://boe.xuanzx.com

Java: u instanceof User
来源：http://ppt.zdqjudy.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://hyk.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://pnw.chenlongwang.top

C#:   u is User
来源：http://zsh.jinyuanbaomall.cn

[G14] 数据类 / record
来源：http://fhy.zhengqikj.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rlg.316326.xyz

PHP:  // 用 readonly 属性模拟
来源：http://jyt.sweek.top

JS:   // 无内置：普通类或对象字面量
来源：http://noz.cashguo.top

TS:   type User = { name: string; age: number };
来源：http://vbp.yonumen.top

Java: record User(String name, int age) {}
来源：http://aes.wangdashe.top

Go:   type User struct { Name string; Age int }
来源：http://okg.zhaomingkeji.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vbn.hesvh.cn

C#:   record User(string Name, int Age);
来源：http://ysw.yvedp.cn

[G15] 枚举
来源：http://ojc.fehbvm.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kga.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hlf.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qln.hongshengwenyu.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://guo.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://stj.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qtr.ydjk.org.cn

Ruby: Color = %i[red green].freeze
来源：http://jab.hnqzz.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wvl.jinyuanbaomall.cn

[G16] 对象转数组 / 字典
来源：http://lgo.gaohongyu789.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fbb.gzhubu.top

PHP:  get_object_vars($obj);
来源：http://kob.hywenlv.cn

JS:   Object.entries(obj)
来源：http://pyz.gotoacloud.top

TS:   Object.entries(obj)
来源：http://djc.zdbjq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yzn.jinyuanbaomall.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://auw.yonumen.top

Ruby: obj.instance_variables
来源：http://jos.yangfankeji.com

C#:   // 用反射或 System.Text.Json
来源：http://qzc.feifeiyinyue.top

================================================================================
来源：http://bcn.hesvh.cn

H. 异常与错误处理
来源：http://yyr.tian-w.cn

================================================================================
来源：http://vpm.quarkkingdee.top

[H01] try / catch 基础
来源：http://zfq.fanxiaobao.xyz

Py:   try: f()⏎except Exception as e: print(e)
来源：http://spq.xinyue.icu

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lac.shanyushiyangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mjq.fehbvm.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hzs.ybcxt.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bqt.tarul.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wgs.ywan-chungtsiang.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jfc.xuetiantiany.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xoh.yongpay.top

[H02] finally / ensure 收尾
来源：http://hhm.hysaishi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://itt.snrcjt.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jyd.sxryk.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hne.hesvh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rtt.jlsjyb.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gac.andypj.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://cqf.tanke756.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hvl.ywan-chungtsiang.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://pxh.yangfankeji.com

[H03] 主动抛出异常
来源：http://pyj.ywan-chungtsiang.top

Py:   raise ValueError("错误信息")
来源：http://dcf.zhijiandao.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://slz.zhaomingkeji.xyz

JS:   throw new Error("错误信息");
来源：http://nhi.guowangkeji.top

TS:   throw new Error("错误信息");
来源：http://flk.sufxvd.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://iis.haohaochexian.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xzh.jinyuanbaomall.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://eyw.yanxiufei.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yne.yangfankeji.com

[H04] 自定义异常类型
来源：http://ein.yueranfly.top

Py:   class MyError(Exception): pass
来源：http://xhb.fanxiaobao.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://cmm.haohaochexian.top

JS:   class MyError extends Error {}
来源：http://rpt.bbcook.cn

TS:   class MyError extends Error {}
来源：http://ksc.jinqigfzy.top

Java: class MyException extends RuntimeException {}
来源：http://vza.ivvv.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pax.cqqwz.cn

Ruby: class MyError < StandardError; end
来源：http://ose.fehbvm.com

C#:   class MyException : Exception {}
来源：http://pxf.bbcook.cn

[H05] 捕获特定类型
来源：http://qok.fanxiaobao.xyz

Py:   except ValueError as e:
来源：http://hoz.sysykeji.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://npr.yvedp.cn

JS:   if (e instanceof TypeError) {}
来源：http://tfw.zdbjq.cn

TS:   if (e instanceof TypeError) {}
来源：http://pko.zdqjudy.top

Java: catch (IOException | SQLException e) {}
来源：http://vnr.9152youxi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vnf.cashguo.top

Ruby: rescue ArgumentError => e
来源：http://feu.zdbjq.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zyp.fanxiaobao.xyz

[H06] 可选值 / 空值安全访问
来源：http://zny.guannengcc.top

Py:   value = d.get("k") or default
来源：http://oez.fengsongda.top

PHP:  $v = $d["k"] ?? null;
来源：http://kmb.hcnkem.com

JS:   obj?.a?.b;  d ?? default
来源：http://dcb.shanyushiyangkeji.top

TS:   obj?.a?.b;  d ?? default
来源：http://sot.hnxiangtu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qbu.fzhhl.top

Go:   if v, ok := m["k"]; ok { }
来源：http://udc.yonumen.top

Ruby: d&.dig(:a, :b)
来源：http://eaa.yangfankeji.com

C#:   obj?.A?.B ?? default
来源：http://efi.sxryk.cn

[H07] 断言
来源：http://grj.ybcxt.top

Py:   assert x > 0, "必须为正"
来源：http://ekl.cheryme.top

PHP:  assert($x > 0);
来源：http://lue.yfazqb.com

JS:   console.assert(x > 0);
来源：http://xbo.zdbjq.cn

TS:   console.assert(x > 0);
来源：http://ocf.sysykeji.top

Java: assert x > 0 : "必须为正";
来源：http://sjb.snrcjt.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yds.nwbrower.top

Ruby: raise "必须为正" unless x > 0
来源：http://vbz.ydzc1.top

C#:   Debug.Assert(x > 0);
来源：http://ilm.hesvh.cn

[H08] 获取错误信息与堆栈
来源：http://tjp.wangshuangyany.cn

Py:   str(e);  traceback.format_exc()
来源：http://qiq.yueranfly.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lrn.nanxinkj.top

JS:   e.message;  e.stack
来源：http://hym.jinyuanbaomall.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sya.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://koi.shzxlz.cn

Go:   err.Error()
来源：http://tqn.hnxiangtu.top

Ruby: e.message;  e.backtrace
来源：http://nnu.yonumen.top

C#:   e.Message;  e.StackTrace
来源：http://nbc.hcnkem.com

[H09] 带错误码的异常
来源：http://ugx.hysaishi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xng.cheryme.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://rzc.fktsv.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yub.jqgfzy.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rir.hywenlv.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fws.0kj1m.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://six.vqdsnc.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xlz.snrcjt.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gye.aizwys.cn

[H10] 资源自动释放
来源：http://afu.xylfe.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kud.vehdjk.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oiq.jlsjyb.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wfg.yj20258888.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rin.yuxming.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hxu.tian-w.cn

Go:   defer f.Close()
来源：http://cqk.jinqigfzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yof.snrcjt.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://shb.mhx1999.top

================================================================================
来源：http://mwx.daria6918.cn

I. 正则表达式
来源：http://icb.iojbl.cn

================================================================================
来源：http://ptt.wangdashe.top

[I01] 判断是否匹配
来源：http://gbw.yvedp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://opl.fzhhl.top

PHP:  preg_match('/\d+/', $s);
来源：http://otj.tianlin.xyz

JS:   /\d+/.test(s)
来源：http://csp.bjfxy.top

TS:   /\d+/.test(s)
来源：http://eaw.xuanzx.com

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vcd.vehdjk.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wtq.jinghuilouyu.cn

Ruby: s.match?(/\d+/)
来源：http://yde.mhx1999.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uro.daxiang520.top

[I02] 提取所有匹配
来源：http://jim.c1oappe.top

Py:   re.findall(r"\d+", s)
来源：http://rnu.jinghuilouyu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kkp.jianghu66.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ktu.xylfe.cn

TS:   s.match(/\d+/g)
来源：http://nkl.daria6918.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ulp.gotoacloud.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ear.xziqi.cn

Ruby: s.scan(/\d+/)
来源：http://luo.xingfuxueyuan.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sny.ydzc1.top

[I03] 提取捕获分组
来源：http://pqp.hammf.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fqs.chenjidiqi.icu

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jwq.havefunace.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bqy.ydjk.org.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qxt.jinqigfzy.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ztt.yj20258.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jue.sysykeji.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xvv.zhengqikj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ezl.fanxiaobao.xyz

[I04] 正则替换
来源：http://yka.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://diw.mhx1999.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://imx.yfazqb.com

JS:   s.replace(/\d+/g, "#")
来源：http://rpm.yj20258888.top

TS:   s.replace(/\d+/g, "#")
来源：http://hyp.ehwqpu.com

Java: s.replaceAll("\\d+", "#")
来源：http://sdd.kuanghao11.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mse.xylfe.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xtb.nwbrower.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lou.xuetiantiany.cn

[I05] 按正则拆分
来源：http://llm.hnqzz.top

Py:   re.split(r"\s*,\s*", s)
来源：http://ocs.ehwqpu.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jky.iojbl.cn

JS:   s.split(/\s*,\s*/)
来源：http://zyx.hfpthk.cn

TS:   s.split(/\s*,\s*/)
来源：http://ogu.zhengqikj.top

Java: s.split("\\s*,\\s*")
来源：http://xon.shanyushiyangtech.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mxb.yvedp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nfr.aizwys.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://byb.hysaishi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zbb.yvedp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hsf.wangshuangyany.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nxm.zycfv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://arw.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pdo.xingfuxueyuan.xyz

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ptg.mhx1999.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dqz.gzhubu.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wug.vehdjk.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uib.pycfn.com

[I07] 忽略大小写与多行模式
来源：http://opz.zhengqikj.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fyk.tanke756.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://obl.jianghu66.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ftq.wangdashe.top

TS:   /error/gim
来源：http://jgq.wangdashe.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jtw.haohaochexian.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fht.zhongyouzk.top

Ruby: s.scan(/error/i)
来源：http://esf.ehwqpu.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yaw.yonumen.top

[I08] 贪婪与非贪婪匹配
来源：http://kgr.yuanzhike.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xlt.aizwys.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fnv.yuanzhike.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://abz.yonumen.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://joc.hfpthk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ppl.uphjek.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ugj.jinqigufen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rqg.zhixingplan.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ezn.zycfv.cn

================================================================================
来源：http://zyg.tianlin.xyz

J. 日期与时间
来源：http://bkq.chenzaomai.com

================================================================================
来源：http://eep.sjlbkw.cn

[J01] 获取当前时间
来源：http://ncx.yj20258888.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://kcl.jinghuilouyu.cn


<!-- 参考信息 -->