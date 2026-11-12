代发 wailian999

Ruby: @name = "x"
来源：http://szw.shanyushiyangkeji.top

C#:   public string Name { get; set; } = "x";
来源：http://gie.zhoulong.xyz

[G04] 定义方法
来源：http://sdl.yvedp.cn

Py:   def greet(self): return self.name
来源：http://nqx.jyoumei.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://eez.guowangkeji.top

JS:   greet() { return this.name; }
来源：http://hdb.ctjpmb.com

TS:   greet(): string { return this.name; }
来源：http://efi.jqgufenzy.top

Java: String greet() { return name; }
来源：http://rfy.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://zaf.zdqjudy.top

Ruby: def greet; @name; end
来源：http://uqu.ctjpmb.com

C#:   public string Greet() => Name;
来源：http://yxr.nwbrower.top

[G05] 继承
来源：http://txc.nanxinkj.top

Py:   class Admin(User): pass
来源：http://jel.gaohongyu789.top

PHP:  class Admin extends User {}
来源：http://yak.daxiang520.top

JS:   class Admin extends User {}
来源：http://cir.zhiwuduotai.top

TS:   class Admin extends User {}
来源：http://aci.hysaishi.cn

Java: class Admin extends User {}
来源：http://vlc.gotoacloud.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wje.fengsongda.top

Ruby: class Admin < User; end
来源：http://szn.svipenyu.cn

C#:   class Admin : User {}
来源：http://dyx.daxiang520.top

[G06] 重写方法
来源：http://lvg.jinqigufen.top

Py:   def greet(self): return "admin"
来源：http://bgp.9152youxi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yym.tanke756.top

JS:   greet() { return "admin"; }
来源：http://dol.ywan-chungtsiang.top

TS:   greet(): string { return "admin"; }
来源：http://abp.chenjidiqi.icu

Java: @Override String greet() { return "admin"; }
来源：http://qhk.yfazqb.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xit.tian-w.cn

Ruby: def greet; "admin"; end
来源：http://jug.52xcode.cn

C#:   public override string Greet() => "admin";
来源：http://pui.quarkkingdee.top

[G07] 调用父类方法
来源：http://ele.mhx1999.top

Py:   super().greet()
来源：http://kgs.hywenlv.cn

PHP:  parent::greet();
来源：http://pcj.9152youxi.cn

JS:   super.greet();
来源：http://qtf.hysaishi.cn

TS:   super.greet();
来源：http://rea.ctjpmb.com

Java: super.greet();
来源：http://dgn.shangyingyoupin.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wep.sysykeji.top

Ruby: super
来源：http://vay.aizwys.cn

C#:   base.Greet();
来源：http://kbe.yj20258.top

[G08] 静态方法与属性
来源：http://dfp.daxiang520.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hjd.zhiwuduotai.top

PHP:  public static function f() {}
来源：http://hud.jinqigufen.top

JS:   static f() {}
来源：http://szh.jiagoushi.top

TS:   static f(): void {}
来源：http://ntc.iojbl.cn

Java: static void f() {}
来源：http://cwy.redwolf501.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://raw.0kj1m.cn

Ruby: def self.f; end
来源：http://wva.hnxiangtu.top

C#:   public static void F() {}
来源：http://koi.zhixingplan.top

[G09] 接口 / 抽象类
来源：http://hds.jyoumei.cn

Py:   from abc import ABC, abstractmethod
来源：http://kjx.ivvv.top

PHP:  interface Shape { public function area(): float; }
来源：http://qzy.hnxiangtu.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://pmm.hywenlv.cn

TS:   interface Shape { area(): number; }
来源：http://utj.dianchejie.cn

Java: interface Shape { double area(); }
来源：http://dnt.tanke756.top

Go:   type Shape interface { Area() float64 }
来源：http://mqx.ppjwa.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://djl.cucudq.cn

C#:   interface IShape { double Area(); }
来源：http://bks.nanxuanxn.top

[G10] 访问控制
来源：http://dko.ywan-chungtsiang.top

Py:   约定 _protected / __private（不强制）
来源：http://fdc.c1oappe.top

PHP:  public / protected / private
来源：http://ztd.svipenyu.cn

JS:   #private 字段；其余公开
来源：http://bxc.vehdjk.com

TS:   public / protected / private
来源：http://qve.pycfn.com

Java: public / protected / private / 默认包级
来源：http://hrr.nanxuanxn.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://diy.birdmap.top

Ruby: public / protected / private
来源：http://tvk.ppjwa.cn

C#:   public / protected / private / internal
来源：http://aub.zhoulong.xyz

[G11] getter / setter
来源：http://czu.pengpengdd.cyou

Py:   @property 与 @x.setter
来源：http://eoi.pycfn.com

PHP:  public function getName(): string { return $this->name; }
来源：http://vbi.xuanzx.com

JS:   get name() { return this._name; }
来源：http://cmv.gogol.net.cn

TS:   get name(): string { return this._name; }
来源：http://tkc.jyoumei.cn

Java: public String getName() { return name; }
来源：http://dby.sxryk.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vxj.zdqjudy.top

Ruby: attr_accessor :name
来源：http://cfd.zhixingplan.top

C#:   public string Name { get; set; }
来源：http://raw.bjfxy.top

[G12] 对象转字符串
来源：http://wmo.ppjwa.cn

Py:   def __str__(self): return self.name
来源：http://aft.xuanzx.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://fkh.jinqigfzy.top

JS:   toString() { return this.name; }
来源：http://tso.sxryk.cn

TS:   toString(): string { return this.name; }
来源：http://slj.chenlongwang.top

Java: @Override public String toString() { return name; }
来源：http://lin.feifeiyinyue.top

Go:   func (u User) String() string { return u.Name }
来源：http://wwg.gzhubu.top

Ruby: def to_s; @name; end
来源：http://jbd.chenjidiqi.icu

C#:   public override string ToString() => Name;
来源：http://pgk.iojbl.cn

[G13] 判断对象类型
来源：http://las.zdqjudy.top

Py:   isinstance(u, User)
来源：http://bku.jinghuilouyu.cn

PHP:  $u instanceof User
来源：http://vyh.fengsongda.top

JS:   u instanceof User
来源：http://jfe.wangshuangyany.cn

TS:   u instanceof User
来源：http://amk.zhiwuduotai.top

Java: u instanceof User
来源：http://taa.guowangkeji.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://vhk.hnqzz.top

Ruby: u.is_a?(User)
来源：http://cxp.pengpengdd.cyou

C#:   u is User
来源：http://hhl.tian-w.cn

[G14] 数据类 / record
来源：http://aeh.yj20258.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://apm.jiagoushi.top

PHP:  // 用 readonly 属性模拟
来源：http://amp.bbcook.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ybi.guowangkeji.top

TS:   type User = { name: string; age: number };
来源：http://xda.cucudq.cn

Java: record User(String name, int age) {}
来源：http://hbx.meibo888.top

Go:   type User struct { Name string; Age int }
来源：http://tmk.jyoumei.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://shf.tanke756.top

C#:   record User(string Name, int Age);
来源：http://tfq.dashuyun.cn

[G15] 枚举
来源：http://bmq.aibaodan.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bai.cheryme.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://iuy.xinyue.icu

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://exa.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dsj.shanyushiyangkeji.top

Java: enum Color { RED, GREEN }
来源：http://wcd.redwolf501.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://skg.yongpay.top

Ruby: Color = %i[red green].freeze
来源：http://vpg.xylfe.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bdu.iojbl.cn

[G16] 对象转数组 / 字典
来源：http://ghp.fanxiaobao.xyz

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qtx.nanxinkj.top

PHP:  get_object_vars($obj);
来源：http://pwz.yvedp.cn

JS:   Object.entries(obj)
来源：http://nes.xuanzx.com

TS:   Object.entries(obj)
来源：http://and.pengpengdd.cyou

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lrl.jqgfzy.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://prg.yuanzhike.top

Ruby: obj.instance_variables
来源：http://knm.ydjk.org.cn

C#:   // 用反射或 System.Text.Json
来源：http://thk.yonumen.top

================================================================================
来源：http://ksn.sxryk.cn

H. 异常与错误处理
来源：http://ukn.jqgfzy.top

================================================================================
来源：http://vdd.kuanghao11.cn

[H01] try / catch 基础
来源：http://zjd.shuidangran.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yaz.hcnkem.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jrz.hnxiangtu.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yro.gaohongyu789.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qak.hammf.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pyi.hysaishi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xrj.jiagoushi.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wya.fehbvm.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xbc.epnwcf.com

[H02] finally / ensure 收尾
来源：http://dgp.jinghuilouyu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uif.shanyushiyangtech.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://ijw.fengsongda.top

JS:   try { f(); } finally { cleanup(); }
来源：http://rzg.mhx1999.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fix.xuetiantiany.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ppa.chenjidiqi.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://fam.fehbvm.com

Ruby: begin; f; ensure; cleanup; end
来源：http://wfn.hesvh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wlo.cqqwz.cn

[H03] 主动抛出异常
来源：http://sqj.bbcook.cn

Py:   raise ValueError("错误信息")
来源：http://fog.zhiwuduotai.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mmz.jinqigfzy.top

JS:   throw new Error("错误信息");
来源：http://niy.jlsjyb.cn

TS:   throw new Error("错误信息");
来源：http://pws.ppjwa.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lld.cashguo.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qjo.snrcjt.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wzs.0kj1m.cn

C#:   throw new ArgumentException("错误信息");
来源：http://heo.epnwcf.com

[H04] 自定义异常类型
来源：http://jzf.316326.xyz

Py:   class MyError(Exception): pass
来源：http://pzy.nanxinkj.top

PHP:  class MyError extends RuntimeException {}
来源：http://aje.bjfxy.top

JS:   class MyError extends Error {}
来源：http://hwg.cucudq.cn

TS:   class MyError extends Error {}
来源：http://uzb.ybcxt.top

Java: class MyException extends RuntimeException {}
来源：http://axk.jinghuilouyu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pfn.hcnkem.com

Ruby: class MyError < StandardError; end
来源：http://jaw.jinyuanbaomall.cn

C#:   class MyException : Exception {}
来源：http://irg.yj20258888.top

[H05] 捕获特定类型
来源：http://upk.fktsv.cn

Py:   except ValueError as e:
来源：http://wlo.cucudq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pug.yonumen.top

JS:   if (e instanceof TypeError) {}
来源：http://aju.sysykeji.top

TS:   if (e instanceof TypeError) {}
来源：http://dtt.ydzc1.top

Java: catch (IOException | SQLException e) {}
来源：http://fnz.iojbl.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jlz.jiagoushi.top

Ruby: rescue ArgumentError => e
来源：http://etr.pycfn.com

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://chb.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://jkv.gaohongyu789.top

Py:   value = d.get("k") or default
来源：http://adm.cqqwz.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gvm.gaohongyu789.top

JS:   obj?.a?.b;  d ?? default
来源：http://tci.ppjwa.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sin.fengsongda.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dtv.zhiwuduotai.top

Go:   if v, ok := m["k"]; ok { }
来源：http://miq.yj20258.top

Ruby: d&.dig(:a, :b)
来源：http://wbl.ywan-chungtsiang.top

C#:   obj?.A?.B ?? default
来源：http://paq.tanke756.top

[H07] 断言
来源：http://ale.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://nym.birdmap.top

PHP:  assert($x > 0);
来源：http://vzt.jinghuilouyu.cn

JS:   console.assert(x > 0);
来源：http://yhg.jinqigfzy.top

TS:   console.assert(x > 0);
来源：http://dhd.xinyue.icu

Java: assert x > 0 : "必须为正";
来源：http://ofu.guannengcc.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cjc.birdmap.top

Ruby: raise "必须为正" unless x > 0
来源：http://cyk.ppjwa.cn

C#:   Debug.Assert(x > 0);
来源：http://cdh.nanxuanxn.top

[H08] 获取错误信息与堆栈
来源：http://sya.feifeiyinyue.top

Py:   str(e);  traceback.format_exc()
来源：http://ajw.yueranfly.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ybs.tarul.cn

JS:   e.message;  e.stack
来源：http://akq.zycfv.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wry.xuetiantiany.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nww.tanke756.top

Go:   err.Error()
来源：http://knp.yonumen.top

Ruby: e.message;  e.backtrace
来源：http://otw.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://gng.zhengqikj.top

[H09] 带错误码的异常
来源：http://ahq.yvedp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pxa.hammf.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pmt.daxiang520.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ewm.gotoacloud.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dia.hesvh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://drn.zhengqikj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zxy.pycfn.com

Ruby: raise MyError.new("fail", 500)
来源：http://bhm.hongshengwenyu.top

C#:   // 自定义异常类中加 Code 属性
来源：http://amw.yvedp.cn

[H10] 资源自动释放
来源：http://ouh.zhongyouzk.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cqi.cqqwz.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dob.yueranfly.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nwg.vehdjk.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wir.havefunace.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cvt.sysykeji.top

Go:   defer f.Close()
来源：http://osx.jinqigufen.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tax.fanxiaobao.xyz

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oti.iojbl.cn

================================================================================
来源：http://jzl.zhengqikj.top

I. 正则表达式
来源：http://awe.yuanzhike.top

================================================================================
来源：http://xfi.zhengqikj.top

[I01] 判断是否匹配
来源：http://txj.nanxuanxn.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rvj.yj20258.top

PHP:  preg_match('/\d+/', $s);
来源：http://ctl.cucudq.cn

JS:   /\d+/.test(s)
来源：http://bgt.jianghu66.top

TS:   /\d+/.test(s)
来源：http://kcx.yvedp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bjw.cqqwz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://adh.jiagoushi.top

Ruby: s.match?(/\d+/)
来源：http://ozs.xingfuxueyuan.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vkz.snrcjt.cn

[I02] 提取所有匹配
来源：http://hzy.aibaodan.cn

Py:   re.findall(r"\d+", s)
来源：http://dml.zhengqikj.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ibc.yuxming.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nwu.jyoumei.cn

TS:   s.match(/\d+/g)
来源：http://emf.hysaishi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tkj.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qfk.hesvh.cn

Ruby: s.scan(/\d+/)
来源：http://kxw.gotoacloud.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fkc.aizwys.cn

[I03] 提取捕获分组
来源：http://mvk.c1oappe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wsd.feifeiyinyue.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cmg.gaohongyu789.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rku.jiagoushi.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zgx.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hlj.cucudq.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qsz.fktsv.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lvu.yvedp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jae.iojbl.cn

[I04] 正则替换
来源：http://yfp.xuanzx.com

Py:   re.sub(r"\d+", "#", s)
来源：http://qbr.dianchejie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jet.ydjk.org.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tkg.vqdsnc.cn

TS:   s.replace(/\d+/g, "#")
来源：http://itp.hywenlv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ejh.fzhhl.top

Go:   re.ReplaceAllString(s, "#")
来源：http://pwu.mhx1999.top

Ruby: s.gsub(/\d+/, "#")
来源：http://var.yueranfly.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mac.hywenlv.cn

[I05] 按正则拆分
来源：http://xsg.yongpay.top

Py:   re.split(r"\s*,\s*", s)
来源：http://atj.xingfuxueyuan.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qmd.feifeiyinyue.top

JS:   s.split(/\s*,\s*/)
来源：http://emc.fanxiaobao.xyz

TS:   s.split(/\s*,\s*/)
来源：http://rsy.yuxming.cn

Java: s.split("\\s*,\\s*")
来源：http://gyh.sysykeji.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://voq.xuanzx.com

Ruby: s.split(/\s*,\s*/)
来源：http://hfs.epnwcf.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://dpf.zdqjudy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xmb.hcnkem.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jri.yfazqb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wcn.dianchejie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ylc.zhiwuduotai.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bkc.yvedp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zlg.guowangkeji.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://psb.zhixingplan.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fkz.kuanghao11.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pah.wangdashe.top

[I07] 忽略大小写与多行模式
来源：http://ola.ydjk.org.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xhs.birdmap.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://flq.smart0.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zwi.shanyushiyangkeji.top

TS:   /error/gim
来源：http://aze.xinyue.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://okm.tarul.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dvo.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://enq.chenjidiqi.icu

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xjn.nanxinkj.top

[I08] 贪婪与非贪婪匹配
来源：http://fzi.jinghuilouyu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nxi.hfpthk.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://obq.chenlongwang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://urh.zhijiandao.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gyl.shanyushiyangkeji.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://otv.yfazqb.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qhx.ybcxt.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wyl.shanyushiyangkeji.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://upu.sysykeji.top

================================================================================
来源：http://kob.yanxiufei.cn

J. 日期与时间
来源：http://kgk.bjfxy.top

================================================================================
来源：http://zag.hnqzz.top

[J01] 获取当前时间
来源：http://qek.hywenlv.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://btx.jinqigufen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://avk.hnxiangtu.top

JS:   new Date();  Date.now()
来源：http://kwk.jqgufenzy.top

TS:   new Date();  Date.now()
来源：http://mog.yueranfly.top

Java: LocalDateTime.now();  Instant.now()
来源：http://hmd.sweek.top

Go:   time.Now()
来源：http://hth.jinqigfzy.top

Ruby: Time.now
来源：http://lwr.hcnkem.com

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wpf.yueranfly.top

[J02] 格式化输出
来源：http://icw.sysykeji.top


<!-- 参考信息 -->