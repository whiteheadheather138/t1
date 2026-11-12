代发 wailian999

TS:   constructor(public name: string) {}
来源：http://ubk.yanxiufei.cn

Java: User(String name) { this.name = name; }
来源：http://gsj.jiagoushi.top

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rrd.fanxiaobao.xyz

Ruby: def initialize(name); @name = name; end
来源：http://ycv.hnqzz.top

C#:   public User(string name) { Name = name; }
来源：http://kid.hfpthk.cn

[G03] 实例属性
来源：http://grd.gaohongyu789.top

Py:   self.name = "x"
来源：http://zws.chenlongwang.top

PHP:  public string $name = "x";
来源：http://tkf.andypj.xyz

JS:   this.name = "x";
来源：http://idv.yj20258.top

TS:   name: string = "x";
来源：http://ygd.andypj.xyz

Java: private String name;
来源：http://itc.yonumen.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bfr.zhengqikj.top

Ruby: @name = "x"
来源：http://zfm.sjlbkw.cn

C#:   public string Name { get; set; } = "x";
来源：http://yrw.ydzc1.top

[G04] 定义方法
来源：http://lxi.svipenyu.cn

Py:   def greet(self): return self.name
来源：http://puq.uphjek.com

PHP:  public function greet(): string { return $this->name; }
来源：http://giq.uphjek.com

JS:   greet() { return this.name; }
来源：http://jqd.yj202588.top

TS:   greet(): string { return this.name; }
来源：http://xgk.pycfn.com

Java: String greet() { return name; }
来源：http://fan.shangyingyoupin.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://shp.52xcode.cn

Ruby: def greet; @name; end
来源：http://iyc.haohaochexian.top

C#:   public string Greet() => Name;
来源：http://vis.tarul.cn

[G05] 继承
来源：http://xob.gotoacloud.top

Py:   class Admin(User): pass
来源：http://qwr.chenzaomai.com

PHP:  class Admin extends User {}
来源：http://ppn.fzhhl.top

JS:   class Admin extends User {}
来源：http://tvc.fzhhl.top

TS:   class Admin extends User {}
来源：http://jap.ydjk.org.cn

Java: class Admin extends User {}
来源：http://cyk.shanyushiyangtech.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kdz.zdbjq.cn

Ruby: class Admin < User; end
来源：http://woz.ybcxt.top

C#:   class Admin : User {}
来源：http://hdh.hfpthk.cn

[G06] 重写方法
来源：http://oqr.xuetiantiany.cn

Py:   def greet(self): return "admin"
来源：http://iuc.redwolf501.top

PHP:  public function greet(): string { return "admin"; }
来源：http://hdd.sufxvd.cn

JS:   greet() { return "admin"; }
来源：http://cqb.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://ndm.yj202588.top

Java: @Override String greet() { return "admin"; }
来源：http://yod.cqqwz.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nba.ydzc1.top

Ruby: def greet; "admin"; end
来源：http://ytt.yonumen.top

C#:   public override string Greet() => "admin";
来源：http://wuk.zhijiandao.cn

[G07] 调用父类方法
来源：http://cut.cqqwz.cn

Py:   super().greet()
来源：http://ysc.sjlbkw.cn

PHP:  parent::greet();
来源：http://uih.0kj1m.cn

JS:   super.greet();
来源：http://cop.0kj1m.cn

TS:   super.greet();
来源：http://vre.jyoumei.cn

Java: super.greet();
来源：http://ojh.hnxiangtu.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gan.yangfankeji.com

Ruby: super
来源：http://fmb.yongpay.top

C#:   base.Greet();
来源：http://xoc.andypj.xyz

[G08] 静态方法与属性
来源：http://dij.cheryme.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tfz.jinqigfzy.top

PHP:  public static function f() {}
来源：http://lha.jinqigfzy.top

JS:   static f() {}
来源：http://ovb.tarul.cn

TS:   static f(): void {}
来源：http://izk.haohaochexian.top

Java: static void f() {}
来源：http://quh.xuetiantiany.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://whe.vehdjk.com

Ruby: def self.f; end
来源：http://aey.jiagoushi.top

C#:   public static void F() {}
来源：http://zxo.tanke756.top

[G09] 接口 / 抽象类
来源：http://vvd.fengsongda.top

Py:   from abc import ABC, abstractmethod
来源：http://irn.cdnleiting.top

PHP:  interface Shape { public function area(): float; }
来源：http://vzq.chenzaomai.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://wsf.sjlbkw.cn

TS:   interface Shape { area(): number; }
来源：http://wyj.pengpengdd.cyou

Java: interface Shape { double area(); }
来源：http://hed.zhiwuduotai.top

Go:   type Shape interface { Area() float64 }
来源：http://wbw.tanke756.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://erf.ctjpmb.com

C#:   interface IShape { double Area(); }
来源：http://abc.xziqi.cn

[G10] 访问控制
来源：http://lgq.shangyingyoupin.top

Py:   约定 _protected / __private（不强制）
来源：http://yie.shzxlz.cn

PHP:  public / protected / private
来源：http://vtu.fzhhl.top

JS:   #private 字段；其余公开
来源：http://gxa.pengpengdd.cyou

TS:   public / protected / private
来源：http://pbf.vqdsnc.cn

Java: public / protected / private / 默认包级
来源：http://pdq.aibaodan.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jbu.nwbrower.top

Ruby: public / protected / private
来源：http://viq.hnxiangtu.top

C#:   public / protected / private / internal
来源：http://poh.zhoulong.xyz

[G11] getter / setter
来源：http://ret.yuanzhike.top

Py:   @property 与 @x.setter
来源：http://tfd.cqqwz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pmj.meibo888.top

JS:   get name() { return this._name; }
来源：http://dcf.fanxiaobao.xyz

TS:   get name(): string { return this._name; }
来源：http://jbk.hysaishi.cn

Java: public String getName() { return name; }
来源：http://oce.fzhhl.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://uix.uphjek.com

Ruby: attr_accessor :name
来源：http://rda.bjfxy.top

C#:   public string Name { get; set; }
来源：http://bjp.hongshengwenyu.top

[G12] 对象转字符串
来源：http://pvl.cashguo.top

Py:   def __str__(self): return self.name
来源：http://fda.zycfv.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fzo.jqgufenzy.top

JS:   toString() { return this.name; }
来源：http://wwo.ehwqpu.com

TS:   toString(): string { return this.name; }
来源：http://dww.jinqigufen.top

Java: @Override public String toString() { return name; }
来源：http://fjl.hfpthk.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ehi.tarul.cn

Ruby: def to_s; @name; end
来源：http://zvq.yuanzhike.top

C#:   public override string ToString() => Name;
来源：http://sab.chenzaomai.com

[G13] 判断对象类型
来源：http://ejb.zhengqikj.top

Py:   isinstance(u, User)
来源：http://zyp.ywan-chungtsiang.top

PHP:  $u instanceof User
来源：http://vmm.bbcook.cn

JS:   u instanceof User
来源：http://gam.ydjk.org.cn

TS:   u instanceof User
来源：http://ixp.tian-w.cn

Java: u instanceof User
来源：http://oin.cucudq.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://eug.nanxuanxn.top

Ruby: u.is_a?(User)
来源：http://xfi.shanyushiyangkeji.top

C#:   u is User
来源：http://wiu.fengsongda.top

[G14] 数据类 / record
来源：http://dhg.jiagoushi.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kvw.shanyushiyangkeji.top

PHP:  // 用 readonly 属性模拟
来源：http://rbn.gotoacloud.top

JS:   // 无内置：普通类或对象字面量
来源：http://ais.gzhubu.top

TS:   type User = { name: string; age: number };
来源：http://red.feifeiyinyue.top

Java: record User(String name, int age) {}
来源：http://ydb.ydzc1.top

Go:   type User struct { Name string; Age int }
来源：http://sdx.feifeiyinyue.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pah.nwbrower.top

C#:   record User(string Name, int Age);
来源：http://sdv.hcnkem.com

[G15] 枚举
来源：http://uci.meibo888.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://znn.hesvh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ufy.haohaochexian.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://whx.52xcode.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gdj.hesvh.cn

Java: enum Color { RED, GREEN }
来源：http://lsj.yfazqb.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yjc.vehdjk.com

Ruby: Color = %i[red green].freeze
来源：http://vnp.yuanzhike.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rbg.birdmap.top

[G16] 对象转数组 / 字典
来源：http://ydt.yueranfly.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ony.hfpthk.cn

PHP:  get_object_vars($obj);
来源：http://dyl.yfazqb.com

JS:   Object.entries(obj)
来源：http://hbg.chenjidiqi.icu

TS:   Object.entries(obj)
来源：http://jxc.bjfxy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gxy.yonumen.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://jxh.zhixingplan.top

Ruby: obj.instance_variables
来源：http://cgj.uphjek.com

C#:   // 用反射或 System.Text.Json
来源：http://jvc.xuetiantiany.cn

================================================================================
来源：http://trj.jlsjyb.cn

H. 异常与错误处理
来源：http://guf.sysykeji.top

================================================================================
来源：http://dmn.feifeiyinyue.top

[H01] try / catch 基础
来源：http://agh.kuanghao11.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ekw.feifeiyinyue.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xmu.hysaishi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oyw.vehdjk.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cql.sxryk.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://svm.hywenlv.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cru.zhengqikj.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wcv.vehdjk.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ogh.yonumen.top

[H02] finally / ensure 收尾
来源：http://imu.andypj.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://jlp.cucudq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://byq.cheryme.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rbl.mhx1999.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ksm.hnqzz.top

Java: try { f(); } finally { cleanup(); }
来源：http://qwj.aizwys.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ziv.smart0.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://dhj.chenjidiqi.icu

C#:   try { F(); } finally { Cleanup(); }
来源：http://bte.shanyushiyangkeji.top

[H03] 主动抛出异常
来源：http://nvy.shzxlz.cn

Py:   raise ValueError("错误信息")
来源：http://ogb.haohaochexian.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cmb.vqdsnc.cn

JS:   throw new Error("错误信息");
来源：http://pty.fanxiaobao.xyz

TS:   throw new Error("错误信息");
来源：http://fbv.shanyushiyangtech.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://ksa.yj202588.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jfq.ywan-chungtsiang.top

Ruby: raise ArgumentError, "错误信息"
来源：http://rbv.52xcode.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dza.xuanzx.com

[H04] 自定义异常类型
来源：http://hqv.havefunace.top

Py:   class MyError(Exception): pass
来源：http://bzu.fehbvm.com

PHP:  class MyError extends RuntimeException {}
来源：http://hpq.snrcjt.cn

JS:   class MyError extends Error {}
来源：http://klm.yvedp.cn

TS:   class MyError extends Error {}
来源：http://mod.dianchejie.cn

Java: class MyException extends RuntimeException {}
来源：http://jty.hnqzz.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dpu.havefunace.top

Ruby: class MyError < StandardError; end
来源：http://bww.xuanzx.com

C#:   class MyException : Exception {}
来源：http://fof.hysaishi.cn

[H05] 捕获特定类型
来源：http://efr.ydzc1.top

Py:   except ValueError as e:
来源：http://emw.sweek.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ujf.shangyingyoupin.top

JS:   if (e instanceof TypeError) {}
来源：http://hwe.xingfuxueyuan.xyz

TS:   if (e instanceof TypeError) {}
来源：http://wbm.aibaodan.cn

Java: catch (IOException | SQLException e) {}
来源：http://bpk.tanke756.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wde.guannengcc.top

Ruby: rescue ArgumentError => e
来源：http://eah.wangshuangyany.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pqi.zhiwuduotai.top

[H06] 可选值 / 空值安全访问
来源：http://ock.cashguo.top

Py:   value = d.get("k") or default
来源：http://udq.cqqwz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://btg.hongshengwenyu.top

JS:   obj?.a?.b;  d ?? default
来源：http://uly.ehwqpu.com

TS:   obj?.a?.b;  d ?? default
来源：http://afh.quarkkingdee.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cha.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mht.zhaomingkeji.xyz

Ruby: d&.dig(:a, :b)
来源：http://grb.zhijiandao.cn

C#:   obj?.A?.B ?? default
来源：http://hay.vehdjk.com

[H07] 断言
来源：http://mff.uphjek.com

Py:   assert x > 0, "必须为正"
来源：http://fba.wangshuangyany.cn

PHP:  assert($x > 0);
来源：http://lep.feifeiyinyue.top

JS:   console.assert(x > 0);
来源：http://fuh.jyoumei.cn

TS:   console.assert(x > 0);
来源：http://das.yj20258.top

Java: assert x > 0 : "必须为正";
来源：http://ogz.wangdashe.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hmj.xuanzx.com

Ruby: raise "必须为正" unless x > 0
来源：http://ywc.zdbjq.cn

C#:   Debug.Assert(x > 0);
来源：http://mgr.ctjpmb.com

[H08] 获取错误信息与堆栈
来源：http://twd.shanyushiyangtech.top

Py:   str(e);  traceback.format_exc()
来源：http://sgn.guannengcc.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://obk.gotoacloud.top

JS:   e.message;  e.stack
来源：http://xwz.gotoacloud.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ehp.sufxvd.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xpf.0kj1m.cn

Go:   err.Error()
来源：http://ogx.dianchejie.cn

Ruby: e.message;  e.backtrace
来源：http://zsf.jinqigfzy.top

C#:   e.Message;  e.StackTrace
来源：http://eum.jinqigufen.top

[H09] 带错误码的异常
来源：http://riv.chenzaomai.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yxq.shanyushiyangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://lev.redwolf501.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jqm.dianchejie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bpe.andypj.xyz

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qlt.hammf.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://taf.0kj1m.cn

Ruby: raise MyError.new("fail", 500)
来源：http://quz.gaohongyu789.top

C#:   // 自定义异常类中加 Code 属性
来源：http://djp.zhengqikj.top

[H10] 资源自动释放
来源：http://rnn.52xcode.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vrx.yongpay.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zeo.gogol.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xer.epnwcf.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bos.shangyingyoupin.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pco.nanxuanxn.top

Go:   defer f.Close()
来源：http://pok.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wke.cheryme.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bqs.yj20258888.top

================================================================================
来源：http://hbt.hnxiangtu.top

I. 正则表达式
来源：http://ewv.shanyushiyangkeji.top

================================================================================
来源：http://lbr.fehbvm.com

[I01] 判断是否匹配
来源：http://rzj.zhongyouzk.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rmq.jinyuanbaomall.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hma.52xcode.cn

JS:   /\d+/.test(s)
来源：http://abt.gzhubu.top

TS:   /\d+/.test(s)
来源：http://cug.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://roo.nwbrower.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://upx.sufxvd.cn

Ruby: s.match?(/\d+/)
来源：http://vzu.zhengqikj.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zji.xuanzx.com

[I02] 提取所有匹配
来源：http://uik.hnxiangtu.top

Py:   re.findall(r"\d+", s)
来源：http://jhx.hongshengwenyu.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yrd.dianchejie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rxw.jiagoushi.top

TS:   s.match(/\d+/g)
来源：http://lpb.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dxt.wangshuangyany.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ygp.ehwqpu.com

Ruby: s.scan(/\d+/)
来源：http://uwt.fengsongda.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://srx.tanke756.top

[I03] 提取捕获分组
来源：http://oju.fengsongda.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hqw.nwbrower.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cln.sweek.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yxj.yj20258.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hyf.hywenlv.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tjn.ywan-chungtsiang.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yxr.fktsv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jka.hcnkem.com

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cda.xuanzx.com

[I04] 正则替换
来源：http://dvz.nanxinkj.top

Py:   re.sub(r"\d+", "#", s)
来源：http://chx.andypj.xyz

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://muz.yonumen.top

JS:   s.replace(/\d+/g, "#")
来源：http://lkc.fanxiaobao.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://lyl.hnqzz.top

Java: s.replaceAll("\\d+", "#")
来源：http://tey.sxryk.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hhk.sysykeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://sos.pengpengdd.cyou

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zby.zhoulong.xyz

[I05] 按正则拆分
来源：http://yuw.hongshengwenyu.top

Py:   re.split(r"\s*,\s*", s)
来源：http://zru.yanxiufei.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wra.mhx1999.top

JS:   s.split(/\s*,\s*/)
来源：http://nvw.cheryme.top

TS:   s.split(/\s*,\s*/)
来源：http://bpt.haohaochexian.top

Java: s.split("\\s*,\\s*")
来源：http://rfp.ctjpmb.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vnq.gaohongyu789.top

Ruby: s.split(/\s*,\s*/)
来源：http://rfo.bjfxy.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vyb.jyoumei.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://stn.jinyuanbaomall.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jbq.xingfuxueyuan.xyz

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wmb.shanyushiyangtech.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ujf.yueranfly.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tuj.jyoumei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hka.jiagoushi.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oox.xziqi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vgw.uphjek.com

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wdq.cucudq.cn

[I07] 忽略大小写与多行模式
来源：http://psi.fehbvm.com

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rxd.uphjek.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wlj.hysaishi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bnw.xingfuxueyuan.xyz

TS:   /error/gim
来源：http://byu.zhixingplan.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://key.vehdjk.com

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tgm.tian-w.cn

Ruby: s.scan(/error/i)
来源：http://xqu.xingfuxueyuan.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hiw.nwbrower.top

[I08] 贪婪与非贪婪匹配
来源：http://ucm.hesvh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yia.9152youxi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ons.kuanghao11.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bbi.hesvh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eyy.zhixingplan.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://yqc.fengsongda.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://pkl.jinghuilouyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://utg.xinyue.icu

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hkf.shanyushiyangkeji.top

================================================================================
来源：http://tjs.ctjpmb.com


<!-- 参考信息 -->