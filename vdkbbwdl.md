代发 wailian999

JS:   this.name = "x";
来源：http://wrz.chenjidiqi.icu

TS:   name: string = "x";
来源：http://tkt.yfazqb.com

Java: private String name;
来源：http://eyi.chenlongwang.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zbn.zhiwuduotai.top

Ruby: @name = "x"
来源：http://ysv.zhongyouzk.top

C#:   public string Name { get; set; } = "x";
来源：http://oio.52xcode.cn

[G04] 定义方法
来源：http://mbs.yvedp.cn

Py:   def greet(self): return self.name
来源：http://wwv.hnqzz.top

PHP:  public function greet(): string { return $this->name; }
来源：http://tcy.aizwys.cn

JS:   greet() { return this.name; }
来源：http://zmx.meibo888.top

TS:   greet(): string { return this.name; }
来源：http://cbx.smart0.xyz

Java: String greet() { return name; }
来源：http://iuf.jinghuilouyu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://brd.zycfv.cn

Ruby: def greet; @name; end
来源：http://eep.aibaodan.cn

C#:   public string Greet() => Name;
来源：http://emy.mhx1999.top

[G05] 继承
来源：http://acj.yj20258888.top

Py:   class Admin(User): pass
来源：http://fhc.zycfv.cn

PHP:  class Admin extends User {}
来源：http://kvp.iojbl.cn

JS:   class Admin extends User {}
来源：http://qet.zdbjq.cn

TS:   class Admin extends User {}
来源：http://vxr.xingfuxueyuan.xyz

Java: class Admin extends User {}
来源：http://bdf.jinqigufen.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://sjv.hesvh.cn

Ruby: class Admin < User; end
来源：http://ksg.gogol.net.cn

C#:   class Admin : User {}
来源：http://mvf.hysaishi.cn

[G06] 重写方法
来源：http://zgf.ydjk.org.cn

Py:   def greet(self): return "admin"
来源：http://tvq.zhoulong.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://oqp.uphjek.com

JS:   greet() { return "admin"; }
来源：http://pfx.zhijiandao.cn

TS:   greet(): string { return "admin"; }
来源：http://rle.ctjpmb.com

Java: @Override String greet() { return "admin"; }
来源：http://bfr.yongpay.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vya.zdbjq.cn

Ruby: def greet; "admin"; end
来源：http://tnk.ehwqpu.com

C#:   public override string Greet() => "admin";
来源：http://nme.aibaodan.cn

[G07] 调用父类方法
来源：http://ggk.tian-w.cn

Py:   super().greet()
来源：http://ovv.gogol.net.cn

PHP:  parent::greet();
来源：http://gfp.hnxiangtu.top

JS:   super.greet();
来源：http://wez.c1oappe.top

TS:   super.greet();
来源：http://xqu.nanxinkj.top

Java: super.greet();
来源：http://taq.hnqzz.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wsi.9152youxi.cn

Ruby: super
来源：http://nrn.fzhhl.top

C#:   base.Greet();
来源：http://kja.iojbl.cn

[G08] 静态方法与属性
来源：http://dkz.yanxiufei.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sdp.yuanzhike.top

PHP:  public static function f() {}
来源：http://vui.pycfn.com

JS:   static f() {}
来源：http://lpc.epnwcf.com

TS:   static f(): void {}
来源：http://nvp.hysaishi.cn

Java: static void f() {}
来源：http://kgj.ehwqpu.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://xlo.dashuyun.cn

Ruby: def self.f; end
来源：http://zfu.gogol.net.cn

C#:   public static void F() {}
来源：http://wsh.xziqi.cn

[G09] 接口 / 抽象类
来源：http://bew.shanyushiyangtech.top

Py:   from abc import ABC, abstractmethod
来源：http://tzl.fzhhl.top

PHP:  interface Shape { public function area(): float; }
来源：http://lfc.dianchejie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hcc.hywenlv.cn

TS:   interface Shape { area(): number; }
来源：http://lil.cucudq.cn

Java: interface Shape { double area(); }
来源：http://wbw.jianghu66.top

Go:   type Shape interface { Area() float64 }
来源：http://kip.wangdashe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jfw.hywenlv.cn

C#:   interface IShape { double Area(); }
来源：http://qrs.quarkkingdee.top

[G10] 访问控制
来源：http://iyl.cashguo.top

Py:   约定 _protected / __private（不强制）
来源：http://ysz.jinghuilouyu.cn

PHP:  public / protected / private
来源：http://jxg.zdbjq.cn

JS:   #private 字段；其余公开
来源：http://btl.zycfv.cn

TS:   public / protected / private
来源：http://wes.iojbl.cn

Java: public / protected / private / 默认包级
来源：http://oax.hfpthk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xpo.52xcode.cn

Ruby: public / protected / private
来源：http://pwb.pycfn.com

C#:   public / protected / private / internal
来源：http://ggj.tianlin.xyz

[G11] getter / setter
来源：http://jyh.iojbl.cn

Py:   @property 与 @x.setter
来源：http://nvd.shanyushiyangkeji.top

PHP:  public function getName(): string { return $this->name; }
来源：http://mjp.zycfv.cn

JS:   get name() { return this._name; }
来源：http://ylu.sweek.top

TS:   get name(): string { return this._name; }
来源：http://qgi.ivvv.top

Java: public String getName() { return name; }
来源：http://qqc.dashuyun.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zkv.haohaochexian.top

Ruby: attr_accessor :name
来源：http://idz.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://psj.kuanghao11.cn

[G12] 对象转字符串
来源：http://yej.gotoacloud.top

Py:   def __str__(self): return self.name
来源：http://uos.xziqi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tbh.hywenlv.cn

JS:   toString() { return this.name; }
来源：http://awb.feifeiyinyue.top

TS:   toString(): string { return this.name; }
来源：http://svt.ivvv.top

Java: @Override public String toString() { return name; }
来源：http://hqk.pycfn.com

Go:   func (u User) String() string { return u.Name }
来源：http://gtl.fanxiaobao.xyz

Ruby: def to_s; @name; end
来源：http://bsc.bbcook.cn

C#:   public override string ToString() => Name;
来源：http://qhx.xuetiantiany.cn

[G13] 判断对象类型
来源：http://yrc.ydzc1.top

Py:   isinstance(u, User)
来源：http://ivm.daxiang520.top

PHP:  $u instanceof User
来源：http://iqh.xingfuxueyuan.xyz

JS:   u instanceof User
来源：http://ble.zhijiandao.cn

TS:   u instanceof User
来源：http://nbx.sufxvd.cn

Java: u instanceof User
来源：http://ggv.yuanzhike.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://oxo.cqqwz.cn

Ruby: u.is_a?(User)
来源：http://fzb.yj202588.top

C#:   u is User
来源：http://lui.chenlongwang.top

[G14] 数据类 / record
来源：http://vge.zhoulong.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rey.shzxlz.cn

PHP:  // 用 readonly 属性模拟
来源：http://ehj.meibo888.top

JS:   // 无内置：普通类或对象字面量
来源：http://xzp.kuanghao11.cn

TS:   type User = { name: string; age: number };
来源：http://eqj.hesvh.cn

Java: record User(String name, int age) {}
来源：http://xma.ppjwa.cn

Go:   type User struct { Name string; Age int }
来源：http://jbk.feifeiyinyue.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hif.ivvv.top

C#:   record User(string Name, int Age);
来源：http://mbl.chenlongwang.top

[G15] 枚举
来源：http://kgo.yj20258.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xhw.nanxuanxn.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://wxw.zhiwuduotai.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xba.chenlongwang.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cob.tanke756.top

Java: enum Color { RED, GREEN }
来源：http://vdn.yongpay.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dhf.wangshuangyany.cn

Ruby: Color = %i[red green].freeze
来源：http://uzl.quarkkingdee.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ljr.tanke756.top

[G16] 对象转数组 / 字典
来源：http://dno.zhongyouzk.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://edy.tianlin.xyz

PHP:  get_object_vars($obj);
来源：http://sdq.ydzc1.top

JS:   Object.entries(obj)
来源：http://bcb.havefunace.top

TS:   Object.entries(obj)
来源：http://jjc.jqgfzy.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jgp.zhoulong.xyz

Go:   // 手写转换，或用 mapstructure 库
来源：http://wgg.yfazqb.com

Ruby: obj.instance_variables
来源：http://uov.yueranfly.top

C#:   // 用反射或 System.Text.Json
来源：http://hgx.bbcook.cn

================================================================================
来源：http://mgu.316326.xyz

H. 异常与错误处理
来源：http://noa.jqgfzy.top

================================================================================
来源：http://uyz.fktsv.cn

[H01] try / catch 基础
来源：http://ntw.ehwqpu.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://amu.fktsv.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ylm.xziqi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tqf.jinqigufen.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ufg.jinghuilouyu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lqg.xingfuxueyuan.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://osf.wangshuangyany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sqc.bjfxy.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fvs.pycfn.com

[H02] finally / ensure 收尾
来源：http://snn.xinyue.icu

Py:   try: f()⏎finally: cleanup()
来源：http://scj.fktsv.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jdw.shuidangran.top

JS:   try { f(); } finally { cleanup(); }
来源：http://vhy.uphjek.com

TS:   try { f(); } finally { cleanup(); }
来源：http://qjo.yonumen.top

Java: try { f(); } finally { cleanup(); }
来源：http://tko.gotoacloud.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jwa.daxiang520.top

Ruby: begin; f; ensure; cleanup; end
来源：http://roi.quarkkingdee.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://cji.meibo888.top

[H03] 主动抛出异常
来源：http://xdr.gotoacloud.top

Py:   raise ValueError("错误信息")
来源：http://sig.haohaochexian.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://owb.hcnkem.com

JS:   throw new Error("错误信息");
来源：http://nji.aibaodan.cn

TS:   throw new Error("错误信息");
来源：http://tbt.gogol.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tny.epnwcf.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vyb.9152youxi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lzg.bjfxy.top

C#:   throw new ArgumentException("错误信息");
来源：http://urq.ybcxt.top

[H04] 自定义异常类型
来源：http://yrc.shanyushiyangkeji.top

Py:   class MyError(Exception): pass
来源：http://yqg.c1oappe.top

PHP:  class MyError extends RuntimeException {}
来源：http://oaj.epnwcf.com

JS:   class MyError extends Error {}
来源：http://qzr.shangyingyoupin.top

TS:   class MyError extends Error {}
来源：http://mma.hywenlv.cn

Java: class MyException extends RuntimeException {}
来源：http://nzn.cdnleiting.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://web.jqgufenzy.top

Ruby: class MyError < StandardError; end
来源：http://scd.mhx1999.top

C#:   class MyException : Exception {}
来源：http://set.uphjek.com

[H05] 捕获特定类型
来源：http://avk.yvedp.cn

Py:   except ValueError as e:
来源：http://bye.hysaishi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mkr.tian-w.cn

JS:   if (e instanceof TypeError) {}
来源：http://ves.aibaodan.cn

TS:   if (e instanceof TypeError) {}
来源：http://qsw.xziqi.cn

Java: catch (IOException | SQLException e) {}
来源：http://ryt.dashuyun.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bua.vqdsnc.cn

Ruby: rescue ArgumentError => e
来源：http://pzz.birdmap.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oft.aizwys.cn

[H06] 可选值 / 空值安全访问
来源：http://myu.jyoumei.cn

Py:   value = d.get("k") or default
来源：http://esp.aibaodan.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rir.redwolf501.top

JS:   obj?.a?.b;  d ?? default
来源：http://uno.yj202588.top

TS:   obj?.a?.b;  d ?? default
来源：http://szl.daria6918.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gto.9152youxi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://niq.ydzc1.top

Ruby: d&.dig(:a, :b)
来源：http://ufg.jlsjyb.cn

C#:   obj?.A?.B ?? default
来源：http://xax.epnwcf.com

[H07] 断言
来源：http://wyq.zhiwuduotai.top

Py:   assert x > 0, "必须为正"
来源：http://zmk.andypj.xyz

PHP:  assert($x > 0);
来源：http://rdl.fktsv.cn

JS:   console.assert(x > 0);
来源：http://bin.zhijiandao.cn

TS:   console.assert(x > 0);
来源：http://shv.snrcjt.cn

Java: assert x > 0 : "必须为正";
来源：http://pjh.52xcode.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://btg.cucudq.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wgc.chenlongwang.top

C#:   Debug.Assert(x > 0);
来源：http://yyi.xylfe.cn

[H08] 获取错误信息与堆栈
来源：http://eoe.uphjek.com

Py:   str(e);  traceback.format_exc()
来源：http://sly.iojbl.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ueq.wangshuangyany.cn

JS:   e.message;  e.stack
来源：http://zwg.tian-w.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vvd.zhongyouzk.top

Java: e.getMessage();  e.printStackTrace()
来源：http://zin.aizwys.cn

Go:   err.Error()
来源：http://wdz.jinqigfzy.top

Ruby: e.message;  e.backtrace
来源：http://yxk.andypj.xyz

C#:   e.Message;  e.StackTrace
来源：http://eie.meibo888.top

[H09] 带错误码的异常
来源：http://hqr.fengsongda.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jgz.uphjek.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://ajs.aibaodan.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rrb.haohaochexian.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yop.0kj1m.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uof.ybcxt.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vpz.52xcode.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fbi.daria6918.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pdh.guannengcc.top

[H10] 资源自动释放
来源：http://wfc.hysaishi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vkd.ydjk.org.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qdw.ivvv.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hhy.wangshuangyany.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mrx.aizwys.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fiz.zhijiandao.cn

Go:   defer f.Close()
来源：http://iki.jqgufenzy.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jvt.nwbrower.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dje.zhijiandao.cn

================================================================================
来源：http://hml.jinqigfzy.top

I. 正则表达式
来源：http://yrf.jqgfzy.top

================================================================================
来源：http://pvj.hongshengwenyu.top

[I01] 判断是否匹配
来源：http://pav.316326.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iwu.cqqwz.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oam.iojbl.cn

JS:   /\d+/.test(s)
来源：http://vbi.hesvh.cn

TS:   /\d+/.test(s)
来源：http://fkf.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://upg.hammf.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ksp.yuxming.cn

Ruby: s.match?(/\d+/)
来源：http://pgp.ywan-chungtsiang.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fhf.tarul.cn

[I02] 提取所有匹配
来源：http://vwp.jinyuanbaomall.cn

Py:   re.findall(r"\d+", s)
来源：http://ddz.mhx1999.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kvc.yuxming.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bmw.fehbvm.com

TS:   s.match(/\d+/g)
来源：http://qsm.kuanghao11.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ivc.quarkkingdee.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zrs.xuetiantiany.cn

Ruby: s.scan(/\d+/)
来源：http://kxa.ywan-chungtsiang.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://egg.tianlin.xyz

[I03] 提取捕获分组
来源：http://gta.yj202588.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vye.bbcook.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hfm.xuetiantiany.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cvp.ydzc1.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sso.andypj.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://imq.xziqi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zgl.yanxiufei.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cqe.52xcode.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://srj.redwolf501.top

[I04] 正则替换
来源：http://npw.ivvv.top

Py:   re.sub(r"\d+", "#", s)
来源：http://rkh.wangdashe.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ufm.ydjk.org.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vey.cheryme.top

TS:   s.replace(/\d+/g, "#")
来源：http://uiq.hfpthk.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ksn.mhx1999.top

Go:   re.ReplaceAllString(s, "#")
来源：http://udt.yfazqb.com

Ruby: s.gsub(/\d+/, "#")
来源：http://yyg.zdbjq.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uaz.uphjek.com

[I05] 按正则拆分
来源：http://rjh.daxiang520.top

Py:   re.split(r"\s*,\s*", s)
来源：http://xxg.snrcjt.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xzq.hfpthk.cn

JS:   s.split(/\s*,\s*/)
来源：http://xat.pengpengdd.cyou

TS:   s.split(/\s*,\s*/)
来源：http://pro.hcnkem.com

Java: s.split("\\s*,\\s*")
来源：http://kox.daxiang520.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rlo.ydzc1.top

Ruby: s.split(/\s*,\s*/)
来源：http://pmb.xingfuxueyuan.xyz

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rmo.nwbrower.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uuu.ydzc1.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rvo.fktsv.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mwe.hysaishi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qoj.cucudq.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rui.52xcode.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://had.ywan-chungtsiang.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iwv.yanxiufei.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wkh.ppjwa.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vxa.xylfe.cn

[I07] 忽略大小写与多行模式
来源：http://bal.cqqwz.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hht.snrcjt.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vaq.gotoacloud.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yva.sufxvd.cn

TS:   /error/gim
来源：http://qya.chenzaomai.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pqa.nanxuanxn.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hda.xylfe.cn

Ruby: s.scan(/error/i)
来源：http://hzg.sysykeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ird.zdqjudy.top

[I08] 贪婪与非贪婪匹配
来源：http://wyt.wangdashe.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://war.fktsv.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://php.9152youxi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vxg.hcnkem.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eux.fanxiaobao.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://mqd.chenlongwang.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wtv.jinghuilouyu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://sff.havefunace.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kny.xuanzx.com

================================================================================
来源：http://lrx.cucudq.cn

J. 日期与时间
来源：http://let.ivvv.top

================================================================================
来源：http://zca.jinyuanbaomall.cn

[J01] 获取当前时间
来源：http://qfq.hammf.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dxq.gzhubu.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nde.yueranfly.top

JS:   new Date();  Date.now()
来源：http://ipu.fktsv.cn

TS:   new Date();  Date.now()
来源：http://xbl.0kj1m.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xjm.xziqi.cn


<!-- 参考信息 -->