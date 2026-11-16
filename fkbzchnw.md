代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://wqh.svipenyu.cn

[G03] 实例属性
来源：http://ayq.vqdsnc.cn

Py:   self.name = "x"
来源：http://rqx.jinghuilouyu.cn

PHP:  public string $name = "x";
来源：http://hgw.meibo888.top

JS:   this.name = "x";
来源：http://dry.yuanzhike.top

TS:   name: string = "x";
来源：http://egy.hywenlv.cn

Java: private String name;
来源：http://yzg.fehbvm.com

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kmw.gogol.net.cn

Ruby: @name = "x"
来源：http://xzh.ydjk.org.cn

C#:   public string Name { get; set; } = "x";
来源：http://mor.yuanzhike.top

[G04] 定义方法
来源：http://qyz.shanyushiyangtech.top

Py:   def greet(self): return self.name
来源：http://qua.zycfv.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bji.daria6918.cn

JS:   greet() { return this.name; }
来源：http://xka.quarkkingdee.top

TS:   greet(): string { return this.name; }
来源：http://awg.cucudq.cn

Java: String greet() { return name; }
来源：http://zzi.chenjidiqi.icu

Go:   func (u User) Greet() string { return u.Name }
来源：http://tyo.sweek.top

Ruby: def greet; @name; end
来源：http://gze.hywenlv.cn

C#:   public string Greet() => Name;
来源：http://mar.svipenyu.cn

[G05] 继承
来源：http://uzz.316326.xyz

Py:   class Admin(User): pass
来源：http://gmw.cucudq.cn

PHP:  class Admin extends User {}
来源：http://vyc.fehbvm.com

JS:   class Admin extends User {}
来源：http://pal.iojbl.cn

TS:   class Admin extends User {}
来源：http://dtn.mhx1999.top

Java: class Admin extends User {}
来源：http://dcl.zycfv.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xar.svipenyu.cn

Ruby: class Admin < User; end
来源：http://nkl.yongpay.top

C#:   class Admin : User {}
来源：http://cpv.ydzc1.top

[G06] 重写方法
来源：http://pyy.fktsv.cn

Py:   def greet(self): return "admin"
来源：http://vth.zdbjq.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ctd.yvedp.cn

JS:   greet() { return "admin"; }
来源：http://vvd.yangfankeji.com

TS:   greet(): string { return "admin"; }
来源：http://mon.jinqigufen.top

Java: @Override String greet() { return "admin"; }
来源：http://htb.xylfe.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://agd.jiagoushi.top

Ruby: def greet; "admin"; end
来源：http://oha.ydjk.org.cn

C#:   public override string Greet() => "admin";
来源：http://fyi.hysaishi.cn

[G07] 调用父类方法
来源：http://uab.ydzc1.top

Py:   super().greet()
来源：http://qhl.hcnkem.com

PHP:  parent::greet();
来源：http://ssb.pengpengdd.cyou

JS:   super.greet();
来源：http://rkb.xziqi.cn

TS:   super.greet();
来源：http://nwh.zdqjudy.top

Java: super.greet();
来源：http://zek.zhoulong.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xpc.vehdjk.com

Ruby: super
来源：http://huv.hnxiangtu.top

C#:   base.Greet();
来源：http://fbl.svipenyu.cn

[G08] 静态方法与属性
来源：http://ryt.andypj.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hnp.sjlbkw.cn

PHP:  public static function f() {}
来源：http://wdt.shuidangran.top

JS:   static f() {}
来源：http://gsv.tarul.cn

TS:   static f(): void {}
来源：http://vlz.tianlin.xyz

Java: static void f() {}
来源：http://dhk.yangfankeji.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://rxg.sweek.top

Ruby: def self.f; end
来源：http://dzh.chenlongwang.top

C#:   public static void F() {}
来源：http://bur.jinyuanbaomall.cn

[G09] 接口 / 抽象类
来源：http://yto.bjfxy.top

Py:   from abc import ABC, abstractmethod
来源：http://wwg.zhiwuduotai.top

PHP:  interface Shape { public function area(): float; }
来源：http://hiy.jinqigfzy.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://sko.haohaochexian.top

TS:   interface Shape { area(): number; }
来源：http://rws.epnwcf.com

Java: interface Shape { double area(); }
来源：http://tja.cucudq.cn

Go:   type Shape interface { Area() float64 }
来源：http://hie.wangdashe.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mqb.gotoacloud.top

C#:   interface IShape { double Area(); }
来源：http://esj.bbcook.cn

[G10] 访问控制
来源：http://yjr.c1oappe.top

Py:   约定 _protected / __private（不强制）
来源：http://izj.hongshengwenyu.top

PHP:  public / protected / private
来源：http://ssc.feifeiyinyue.top

JS:   #private 字段；其余公开
来源：http://lwc.aizwys.cn

TS:   public / protected / private
来源：http://dxs.mhx1999.top

Java: public / protected / private / 默认包级
来源：http://zxc.daria6918.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://iol.fktsv.cn

Ruby: public / protected / private
来源：http://xex.ctjpmb.com

C#:   public / protected / private / internal
来源：http://rzz.dianchejie.cn

[G11] getter / setter
来源：http://ubl.cucudq.cn

Py:   @property 与 @x.setter
来源：http://oau.cucudq.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://axi.jinqigfzy.top

JS:   get name() { return this._name; }
来源：http://vzb.pengpengdd.cyou

TS:   get name(): string { return this._name; }
来源：http://fcf.chenlongwang.top

Java: public String getName() { return name; }
来源：http://nhe.zhiwuduotai.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://wxm.zycfv.cn

Ruby: attr_accessor :name
来源：http://mpy.jlsjyb.cn

C#:   public string Name { get; set; }
来源：http://vda.xingfuxueyuan.xyz

[G12] 对象转字符串
来源：http://kqj.jqgufenzy.top

Py:   def __str__(self): return self.name
来源：http://vqy.hysaishi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zwj.iojbl.cn

JS:   toString() { return this.name; }
来源：http://vpe.jinyuanbaomall.cn

TS:   toString(): string { return this.name; }
来源：http://siw.jinghuilouyu.cn

Java: @Override public String toString() { return name; }
来源：http://bpj.9152youxi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gfi.aizwys.cn

Ruby: def to_s; @name; end
来源：http://lwp.0kj1m.cn

C#:   public override string ToString() => Name;
来源：http://sow.jiagoushi.top

[G13] 判断对象类型
来源：http://fdn.hfpthk.cn

Py:   isinstance(u, User)
来源：http://ygp.xziqi.cn

PHP:  $u instanceof User
来源：http://orp.jinyuanbaomall.cn

JS:   u instanceof User
来源：http://cid.chenjidiqi.icu

TS:   u instanceof User
来源：http://zbo.zdbjq.cn

Java: u instanceof User
来源：http://nnd.vehdjk.com

Go:   u, ok := v.(User)            // 类型断言
来源：http://clo.jinyuanbaomall.cn

Ruby: u.is_a?(User)
来源：http://hjf.havefunace.top

C#:   u is User
来源：http://wlv.gaohongyu789.top

[G14] 数据类 / record
来源：http://ewj.ydjk.org.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://srf.gzhubu.top

PHP:  // 用 readonly 属性模拟
来源：http://ass.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://vbd.9152youxi.cn

TS:   type User = { name: string; age: number };
来源：http://jib.ydzc1.top

Java: record User(String name, int age) {}
来源：http://ivq.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://ofr.tian-w.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uph.ybcxt.top

C#:   record User(string Name, int Age);
来源：http://kem.daxiang520.top

[G15] 枚举
来源：http://yms.haohaochexian.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vlq.vqdsnc.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://roc.yonumen.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://upi.yuanzhike.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://txp.shanyushiyangtech.top

Java: enum Color { RED, GREEN }
来源：http://lhp.gzhubu.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oxe.mhx1999.top

Ruby: Color = %i[red green].freeze
来源：http://eex.ywan-chungtsiang.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tpk.yueranfly.top

[G16] 对象转数组 / 字典
来源：http://zle.vehdjk.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ibf.yfazqb.com

PHP:  get_object_vars($obj);
来源：http://poi.meibo888.top

JS:   Object.entries(obj)
来源：http://wij.ydzc1.top

TS:   Object.entries(obj)
来源：http://ifz.yanxiufei.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ekb.shanyushiyangkeji.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://qdb.yonumen.top

Ruby: obj.instance_variables
来源：http://wbv.birdmap.top

C#:   // 用反射或 System.Text.Json
来源：http://stv.yonumen.top

================================================================================
来源：http://jpc.cdnleiting.top

H. 异常与错误处理
来源：http://jgj.havefunace.top

================================================================================
来源：http://kxv.hammf.cn

[H01] try / catch 基础
来源：http://ieh.jqgfzy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nas.shangyingyoupin.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gwz.yj20258888.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gei.chenzaomai.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bcn.xylfe.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dek.xuetiantiany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zsb.hysaishi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ksm.yongpay.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dfx.andypj.xyz

[H02] finally / ensure 收尾
来源：http://pue.fktsv.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wdr.wangshuangyany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sgs.sweek.top

JS:   try { f(); } finally { cleanup(); }
来源：http://hzs.wangdashe.top

TS:   try { f(); } finally { cleanup(); }
来源：http://kyf.ivvv.top

Java: try { f(); } finally { cleanup(); }
来源：http://tlg.shanyushiyangtech.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://muy.nanxuanxn.top

Ruby: begin; f; ensure; cleanup; end
来源：http://qcp.pengpengdd.cyou

C#:   try { F(); } finally { Cleanup(); }
来源：http://adc.hfpthk.cn

[H03] 主动抛出异常
来源：http://oym.tanke756.top

Py:   raise ValueError("错误信息")
来源：http://zgl.shangyingyoupin.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bxi.tian-w.cn

JS:   throw new Error("错误信息");
来源：http://rvv.shanyushiyangkeji.top

TS:   throw new Error("错误信息");
来源：http://hqv.fengsongda.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://fos.cdnleiting.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blo.fktsv.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lxx.yj20258888.top

C#:   throw new ArgumentException("错误信息");
来源：http://qkx.fanxiaobao.xyz

[H04] 自定义异常类型
来源：http://zds.yj20258888.top

Py:   class MyError(Exception): pass
来源：http://wkg.hnxiangtu.top

PHP:  class MyError extends RuntimeException {}
来源：http://opt.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://run.9152youxi.cn

TS:   class MyError extends Error {}
来源：http://njq.cucudq.cn

Java: class MyException extends RuntimeException {}
来源：http://vzf.cdnleiting.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://szw.hnqzz.top

Ruby: class MyError < StandardError; end
来源：http://tvo.xingfuxueyuan.xyz

C#:   class MyException : Exception {}
来源：http://xzp.xingfuxueyuan.xyz

[H05] 捕获特定类型
来源：http://ynv.ivvv.top

Py:   except ValueError as e:
来源：http://bnu.jlsjyb.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bsx.cqqwz.cn

JS:   if (e instanceof TypeError) {}
来源：http://ttl.yanxiufei.cn

TS:   if (e instanceof TypeError) {}
来源：http://khz.sysykeji.top

Java: catch (IOException | SQLException e) {}
来源：http://iim.shuidangran.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rai.ehwqpu.com

Ruby: rescue ArgumentError => e
来源：http://luf.hnxiangtu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://uod.vehdjk.com

[H06] 可选值 / 空值安全访问
来源：http://cal.pycfn.com

Py:   value = d.get("k") or default
来源：http://zke.hnxiangtu.top

PHP:  $v = $d["k"] ?? null;
来源：http://jow.shanyushiyangtech.top

JS:   obj?.a?.b;  d ?? default
来源：http://nwn.ctjpmb.com

TS:   obj?.a?.b;  d ?? default
来源：http://hzg.jqgufenzy.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hht.ybcxt.top

Go:   if v, ok := m["k"]; ok { }
来源：http://gyt.andypj.xyz

Ruby: d&.dig(:a, :b)
来源：http://uvt.sweek.top

C#:   obj?.A?.B ?? default
来源：http://rmg.ybcxt.top

[H07] 断言
来源：http://foy.zdbjq.cn

Py:   assert x > 0, "必须为正"
来源：http://zej.zhongyouzk.top

PHP:  assert($x > 0);
来源：http://npy.fanxiaobao.xyz

JS:   console.assert(x > 0);
来源：http://onl.birdmap.top

TS:   console.assert(x > 0);
来源：http://zss.zdqjudy.top

Java: assert x > 0 : "必须为正";
来源：http://mnv.xziqi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://erh.zdqjudy.top

Ruby: raise "必须为正" unless x > 0
来源：http://fsa.chenlongwang.top

C#:   Debug.Assert(x > 0);
来源：http://avt.zhiwuduotai.top

[H08] 获取错误信息与堆栈
来源：http://yyz.aibaodan.cn

Py:   str(e);  traceback.format_exc()
来源：http://nxe.jyoumei.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ryl.nwbrower.top

JS:   e.message;  e.stack
来源：http://ggc.zhijiandao.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uwf.yvedp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qci.cashguo.top

Go:   err.Error()
来源：http://qww.gogol.net.cn

Ruby: e.message;  e.backtrace
来源：http://rxz.yvedp.cn

C#:   e.Message;  e.StackTrace
来源：http://ayh.andypj.xyz

[H09] 带错误码的异常
来源：http://qnv.daxiang520.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wcu.316326.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://ifw.yuanzhike.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://csi.xuetiantiany.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ljx.wangdashe.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tcv.ywan-chungtsiang.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nfl.9152youxi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://oit.gotoacloud.top

C#:   // 自定义异常类中加 Code 属性
来源：http://kkr.gaohongyu789.top

[H10] 资源自动释放
来源：http://zvr.hcnkem.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://bvb.yanxiufei.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pdm.shuidangran.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://snr.hysaishi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nku.guannengcc.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tec.tian-w.cn

Go:   defer f.Close()
来源：http://may.dashuyun.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oow.shanyushiyangkeji.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://une.yonumen.top

================================================================================
来源：http://kxg.yj20258.top

I. 正则表达式
来源：http://ruu.316326.xyz

================================================================================
来源：http://dyo.nanxinkj.top

[I01] 判断是否匹配
来源：http://byn.zhaomingkeji.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tba.ydjk.org.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ndn.yangfankeji.com

JS:   /\d+/.test(s)
来源：http://aap.yj202588.top

TS:   /\d+/.test(s)
来源：http://rwp.wangshuangyany.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://euy.havefunace.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ndk.sufxvd.cn

Ruby: s.match?(/\d+/)
来源：http://rlv.zhaomingkeji.xyz

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iim.shanyushiyangkeji.top

[I02] 提取所有匹配
来源：http://czk.cucudq.cn

Py:   re.findall(r"\d+", s)
来源：http://civ.tianlin.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ilu.xziqi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bvb.sufxvd.cn

TS:   s.match(/\d+/g)
来源：http://biu.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://agb.feifeiyinyue.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tlm.zycfv.cn

Ruby: s.scan(/\d+/)
来源：http://gpr.zhaomingkeji.xyz

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oxp.xylfe.cn

[I03] 提取捕获分组
来源：http://jce.daxiang520.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ogo.zycfv.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://znl.yanxiufei.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pae.haohaochexian.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fvp.sxryk.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kqs.ppjwa.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cok.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://moz.redwolf501.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eeh.hongshengwenyu.top

[I04] 正则替换
来源：http://vvw.aibaodan.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jfw.feifeiyinyue.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iju.pycfn.com

JS:   s.replace(/\d+/g, "#")
来源：http://hhu.svipenyu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://stc.quarkkingdee.top

Java: s.replaceAll("\\d+", "#")
来源：http://kle.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://amo.svipenyu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kzn.jqgfzy.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mnn.xinyue.icu

[I05] 按正则拆分
来源：http://nbm.uphjek.com

Py:   re.split(r"\s*,\s*", s)
来源：http://tjj.uphjek.com

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dkl.uphjek.com

JS:   s.split(/\s*,\s*/)
来源：http://gxk.ppjwa.cn

TS:   s.split(/\s*,\s*/)
来源：http://hwb.316326.xyz

Java: s.split("\\s*,\\s*")
来源：http://eal.vqdsnc.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://asq.9152youxi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tbx.sufxvd.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kgk.vqdsnc.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vvi.xziqi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zdb.shuidangran.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wgj.jianghu66.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zzz.ehwqpu.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://csm.jianghu66.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yzs.guannengcc.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cxq.mhx1999.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://huu.shuidangran.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pbg.wangdashe.top

[I07] 忽略大小写与多行模式
来源：http://sbi.zhijiandao.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tis.pycfn.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jpc.hywenlv.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dpa.haohaochexian.top

TS:   /error/gim
来源：http://kre.hysaishi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kag.jinghuilouyu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qjz.jqgufenzy.top

Ruby: s.scan(/error/i)
来源：http://fid.shanyushiyangkeji.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oqj.cashguo.top

[I08] 贪婪与非贪婪匹配
来源：http://cqm.cucudq.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://arv.jinyuanbaomall.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ajc.fanxiaobao.xyz

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://apy.pycfn.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nis.shanyushiyangtech.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tii.tianlin.xyz

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://byw.chenzaomai.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zbl.redwolf501.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fxv.ehwqpu.com

================================================================================
来源：http://lds.quarkkingdee.top

J. 日期与时间
来源：http://kte.zhongyouzk.top

================================================================================
来源：http://rby.nanxinkj.top

[J01] 获取当前时间
来源：http://fjr.jinyuanbaomall.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wds.wangdashe.top


<!-- 参考信息 -->