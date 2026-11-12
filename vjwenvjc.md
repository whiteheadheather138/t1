代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://upd.hongshengwenyu.top

JS:   greet() { return this.name; }
来源：http://trt.hfpthk.cn

TS:   greet(): string { return this.name; }
来源：http://dpv.zycfv.cn

Java: String greet() { return name; }
来源：http://jtr.zhengqikj.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://jho.zhoulong.xyz

Ruby: def greet; @name; end
来源：http://geu.hesvh.cn

C#:   public string Greet() => Name;
来源：http://ofa.hcnkem.com

[G05] 继承
来源：http://wat.chenjidiqi.icu

Py:   class Admin(User): pass
来源：http://tue.epnwcf.com

PHP:  class Admin extends User {}
来源：http://dpl.quarkkingdee.top

JS:   class Admin extends User {}
来源：http://cga.haohaochexian.top

TS:   class Admin extends User {}
来源：http://ein.bjfxy.top

Java: class Admin extends User {}
来源：http://bpb.fehbvm.com

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bbt.9152youxi.cn

Ruby: class Admin < User; end
来源：http://kxy.cqqwz.cn

C#:   class Admin : User {}
来源：http://xbm.hnxiangtu.top

[G06] 重写方法
来源：http://ain.yonumen.top

Py:   def greet(self): return "admin"
来源：http://hxp.bjfxy.top

PHP:  public function greet(): string { return "admin"; }
来源：http://axx.yuxming.cn

JS:   greet() { return "admin"; }
来源：http://pnm.jqgufenzy.top

TS:   greet(): string { return "admin"; }
来源：http://vzs.jqgfzy.top

Java: @Override String greet() { return "admin"; }
来源：http://vgd.quarkkingdee.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hdl.zhengqikj.top

Ruby: def greet; "admin"; end
来源：http://mym.zdbjq.cn

C#:   public override string Greet() => "admin";
来源：http://zbx.vqdsnc.cn

[G07] 调用父类方法
来源：http://zzj.bbcook.cn

Py:   super().greet()
来源：http://wsp.fanxiaobao.xyz

PHP:  parent::greet();
来源：http://seg.chenjidiqi.icu

JS:   super.greet();
来源：http://vhv.cqqwz.cn

TS:   super.greet();
来源：http://rzs.c1oappe.top

Java: super.greet();
来源：http://ahh.yonumen.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hxp.cheryme.top

Ruby: super
来源：http://uwk.xziqi.cn

C#:   base.Greet();
来源：http://uod.uphjek.com

[G08] 静态方法与属性
来源：http://tzt.zhijiandao.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vgr.tianlin.xyz

PHP:  public static function f() {}
来源：http://ipk.epnwcf.com

JS:   static f() {}
来源：http://xjx.ivvv.top

TS:   static f(): void {}
来源：http://wsy.yueranfly.top

Java: static void f() {}
来源：http://iof.yonumen.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://obu.zhixingplan.top

Ruby: def self.f; end
来源：http://fjo.ehwqpu.com

C#:   public static void F() {}
来源：http://gbg.pycfn.com

[G09] 接口 / 抽象类
来源：http://ika.gogol.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://gar.sxryk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sap.cdnleiting.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://uik.chenjidiqi.icu

TS:   interface Shape { area(): number; }
来源：http://ulx.c1oappe.top

Java: interface Shape { double area(); }
来源：http://ege.9152youxi.cn

Go:   type Shape interface { Area() float64 }
来源：http://duh.zhiwuduotai.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zpi.birdmap.top

C#:   interface IShape { double Area(); }
来源：http://afy.nwbrower.top

[G10] 访问控制
来源：http://ewg.redwolf501.top

Py:   约定 _protected / __private（不强制）
来源：http://tyj.sufxvd.cn

PHP:  public / protected / private
来源：http://znn.ydzc1.top

JS:   #private 字段；其余公开
来源：http://aag.shanyushiyangtech.top

TS:   public / protected / private
来源：http://rnr.0kj1m.cn

Java: public / protected / private / 默认包级
来源：http://qxe.fehbvm.com

Go:   首字母大写可导出，小写仅包内可见
来源：http://yna.jinqigfzy.top

Ruby: public / protected / private
来源：http://bqh.zdbjq.cn

C#:   public / protected / private / internal
来源：http://cba.shanyushiyangkeji.top

[G11] getter / setter
来源：http://azq.yj20258.top

Py:   @property 与 @x.setter
来源：http://rnr.fzhhl.top

PHP:  public function getName(): string { return $this->name; }
来源：http://udl.yj20258888.top

JS:   get name() { return this._name; }
来源：http://jlp.tanke756.top

TS:   get name(): string { return this._name; }
来源：http://tla.yongpay.top

Java: public String getName() { return name; }
来源：http://roq.yj202588.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://lci.andypj.xyz

Ruby: attr_accessor :name
来源：http://qqo.jinqigfzy.top

C#:   public string Name { get; set; }
来源：http://ymg.hnxiangtu.top

[G12] 对象转字符串
来源：http://sti.fktsv.cn

Py:   def __str__(self): return self.name
来源：http://lbs.jinyuanbaomall.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jfn.hcnkem.com

JS:   toString() { return this.name; }
来源：http://wjj.quarkkingdee.top

TS:   toString(): string { return this.name; }
来源：http://bqi.jinghuilouyu.cn

Java: @Override public String toString() { return name; }
来源：http://dkt.yvedp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hjp.nanxuanxn.top

Ruby: def to_s; @name; end
来源：http://ish.hnqzz.top

C#:   public override string ToString() => Name;
来源：http://qsy.daria6918.cn

[G13] 判断对象类型
来源：http://mog.zhongyouzk.top

Py:   isinstance(u, User)
来源：http://kzr.fzhhl.top

PHP:  $u instanceof User
来源：http://sfs.cashguo.top

JS:   u instanceof User
来源：http://yps.sweek.top

TS:   u instanceof User
来源：http://btk.epnwcf.com

Java: u instanceof User
来源：http://kvx.yonumen.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://jlh.ydjk.org.cn

Ruby: u.is_a?(User)
来源：http://svf.jianghu66.top

C#:   u is User
来源：http://ikv.jinqigufen.top

[G14] 数据类 / record
来源：http://uui.pengpengdd.cyou

Py:   @dataclass⏎class User: name: str; age: int
来源：http://csl.gogol.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://mcn.nanxinkj.top

JS:   // 无内置：普通类或对象字面量
来源：http://lfe.ydzc1.top

TS:   type User = { name: string; age: number };
来源：http://nek.ydzc1.top

Java: record User(String name, int age) {}
来源：http://syz.jinghuilouyu.cn

Go:   type User struct { Name string; Age int }
来源：http://sit.zhongyouzk.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ioq.pengpengdd.cyou

C#:   record User(string Name, int Age);
来源：http://env.fanxiaobao.xyz

[G15] 枚举
来源：http://piw.sjlbkw.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ydh.0kj1m.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wfj.jinghuilouyu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tqc.shuidangran.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bhj.yuanzhike.top

Java: enum Color { RED, GREEN }
来源：http://xfg.kuanghao11.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mit.hesvh.cn

Ruby: Color = %i[red green].freeze
来源：http://stv.sysykeji.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://loc.sufxvd.cn

[G16] 对象转数组 / 字典
来源：http://rkz.chenzaomai.com

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tzj.jinqigfzy.top

PHP:  get_object_vars($obj);
来源：http://tde.smart0.xyz

JS:   Object.entries(obj)
来源：http://fbp.xingfuxueyuan.xyz

TS:   Object.entries(obj)
来源：http://vmu.fanxiaobao.xyz

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bfv.pycfn.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://vsp.sjlbkw.cn

Ruby: obj.instance_variables
来源：http://rlu.yanxiufei.cn

C#:   // 用反射或 System.Text.Json
来源：http://jvp.9152youxi.cn

================================================================================
来源：http://khj.gzhubu.top

H. 异常与错误处理
来源：http://pog.zdqjudy.top

================================================================================
来源：http://ejc.meibo888.top

[H01] try / catch 基础
来源：http://euk.redwolf501.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uxe.gaohongyu789.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wfz.jqgufenzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://brc.shzxlz.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vnt.jqgfzy.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dyd.cdnleiting.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sxm.zhijiandao.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xxi.zhijiandao.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qeg.sysykeji.top

[H02] finally / ensure 收尾
来源：http://leq.gogol.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rfw.xuetiantiany.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bgm.epnwcf.com

JS:   try { f(); } finally { cleanup(); }
来源：http://hlf.zycfv.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kel.zhongyouzk.top

Java: try { f(); } finally { cleanup(); }
来源：http://bsm.svipenyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kpm.0kj1m.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pcs.pycfn.com

C#:   try { F(); } finally { Cleanup(); }
来源：http://wxn.nwbrower.top

[H03] 主动抛出异常
来源：http://lir.jiagoushi.top

Py:   raise ValueError("错误信息")
来源：http://gan.shuidangran.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xjv.quarkkingdee.top

JS:   throw new Error("错误信息");
来源：http://srh.fanxiaobao.xyz

TS:   throw new Error("错误信息");
来源：http://urr.mhx1999.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qfl.yonumen.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lsz.bjfxy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://pfc.hywenlv.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ihe.yfazqb.com

[H04] 自定义异常类型
来源：http://zay.yanxiufei.cn

Py:   class MyError(Exception): pass
来源：http://qdn.gotoacloud.top

PHP:  class MyError extends RuntimeException {}
来源：http://ulr.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://nyz.chenjidiqi.icu

TS:   class MyError extends Error {}
来源：http://dmd.mhx1999.top

Java: class MyException extends RuntimeException {}
来源：http://gav.meibo888.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yvq.cucudq.cn

Ruby: class MyError < StandardError; end
来源：http://xeh.jinqigufen.top

C#:   class MyException : Exception {}
来源：http://wjr.haohaochexian.top

[H05] 捕获特定类型
来源：http://ahq.ydzc1.top

Py:   except ValueError as e:
来源：http://tib.ivvv.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uyx.vehdjk.com

JS:   if (e instanceof TypeError) {}
来源：http://yuz.jiagoushi.top

TS:   if (e instanceof TypeError) {}
来源：http://skf.yvedp.cn

Java: catch (IOException | SQLException e) {}
来源：http://yhr.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ehe.pycfn.com

Ruby: rescue ArgumentError => e
来源：http://ktn.jlsjyb.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vfh.fzhhl.top

[H06] 可选值 / 空值安全访问
来源：http://xsu.havefunace.top

Py:   value = d.get("k") or default
来源：http://nje.bbcook.cn

PHP:  $v = $d["k"] ?? null;
来源：http://djw.svipenyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ifh.zhongyouzk.top

TS:   obj?.a?.b;  d ?? default
来源：http://exa.9152youxi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://een.epnwcf.com

Go:   if v, ok := m["k"]; ok { }
来源：http://ccc.ybcxt.top

Ruby: d&.dig(:a, :b)
来源：http://oxp.tian-w.cn

C#:   obj?.A?.B ?? default
来源：http://wmn.svipenyu.cn

[H07] 断言
来源：http://enf.shuidangran.top

Py:   assert x > 0, "必须为正"
来源：http://ywp.dianchejie.cn

PHP:  assert($x > 0);
来源：http://hsg.sweek.top

JS:   console.assert(x > 0);
来源：http://xer.cheryme.top

TS:   console.assert(x > 0);
来源：http://jgk.nanxinkj.top

Java: assert x > 0 : "必须为正";
来源：http://aig.hnxiangtu.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mzy.fktsv.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cua.xuetiantiany.cn

C#:   Debug.Assert(x > 0);
来源：http://eme.aibaodan.cn

[H08] 获取错误信息与堆栈
来源：http://crr.wangdashe.top

Py:   str(e);  traceback.format_exc()
来源：http://rwk.zhixingplan.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rbw.shuidangran.top

JS:   e.message;  e.stack
来源：http://prh.hesvh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://abr.hnxiangtu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://lhz.gaohongyu789.top

Go:   err.Error()
来源：http://yxl.epnwcf.com

Ruby: e.message;  e.backtrace
来源：http://hnh.fengsongda.top

C#:   e.Message;  e.StackTrace
来源：http://cdl.birdmap.top

[H09] 带错误码的异常
来源：http://tvj.ehwqpu.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ikt.ywan-chungtsiang.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://cwd.yj202588.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tcn.sjlbkw.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qjn.yj202588.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hph.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ksn.bjfxy.top

Ruby: raise MyError.new("fail", 500)
来源：http://lep.cucudq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zea.guannengcc.top

[H10] 资源自动释放
来源：http://rqb.cucudq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://utx.sweek.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://par.kuanghao11.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cdg.zhoulong.xyz

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kux.jlsjyb.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iul.aizwys.cn

Go:   defer f.Close()
来源：http://hkf.zhoulong.xyz

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cuv.gotoacloud.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uft.shanyushiyangkeji.top

================================================================================
来源：http://bew.yueranfly.top

I. 正则表达式
来源：http://vjk.cashguo.top

================================================================================
来源：http://jku.zhongyouzk.top

[I01] 判断是否匹配
来源：http://tza.jiagoushi.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hjl.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yhs.jiagoushi.top

JS:   /\d+/.test(s)
来源：http://qko.yangfankeji.com

TS:   /\d+/.test(s)
来源：http://ece.shangyingyoupin.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iiv.meibo888.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oef.yueranfly.top

Ruby: s.match?(/\d+/)
来源：http://qmi.ehwqpu.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bub.hywenlv.cn

[I02] 提取所有匹配
来源：http://lgf.nanxuanxn.top

Py:   re.findall(r"\d+", s)
来源：http://pws.yanxiufei.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dhy.fengsongda.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://otl.zdbjq.cn

TS:   s.match(/\d+/g)
来源：http://vqd.zhixingplan.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dya.nanxinkj.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://huq.vqdsnc.cn

Ruby: s.scan(/\d+/)
来源：http://lkb.9152youxi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zqv.jianghu66.top

[I03] 提取捕获分组
来源：http://nlr.shuidangran.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fnr.0kj1m.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gdq.snrcjt.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yww.mhx1999.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wrm.316326.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eua.ydjk.org.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zmk.svipenyu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uwc.0kj1m.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wed.shuidangran.top

[I04] 正则替换
来源：http://pra.smart0.xyz

Py:   re.sub(r"\d+", "#", s)
来源：http://wob.tian-w.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rmf.gotoacloud.top

JS:   s.replace(/\d+/g, "#")
来源：http://kes.316326.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://vcv.zycfv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wcz.fehbvm.com

Go:   re.ReplaceAllString(s, "#")
来源：http://phu.mhx1999.top

Ruby: s.gsub(/\d+/, "#")
来源：http://eqa.epnwcf.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jid.haohaochexian.top

[I05] 按正则拆分
来源：http://zpx.xuetiantiany.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zhs.yvedp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pin.zhongyouzk.top

JS:   s.split(/\s*,\s*/)
来源：http://ihk.fktsv.cn

TS:   s.split(/\s*,\s*/)
来源：http://coi.ywan-chungtsiang.top

Java: s.split("\\s*,\\s*")
来源：http://aho.52xcode.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qqu.bjfxy.top

Ruby: s.split(/\s*,\s*/)
来源：http://dvm.zhiwuduotai.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://svl.yangfankeji.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://adm.chenzaomai.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://npq.gaohongyu789.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vcw.nanxinkj.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uug.hywenlv.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cxs.fehbvm.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qvu.hcnkem.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zzf.xinyue.icu

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uta.cqqwz.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ntg.gotoacloud.top

[I07] 忽略大小写与多行模式
来源：http://yus.sysykeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ddy.gaohongyu789.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fse.gzhubu.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dbo.wangshuangyany.cn

TS:   /error/gim
来源：http://omf.ydjk.org.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kjg.ydjk.org.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ijk.yj20258.top

Ruby: s.scan(/error/i)
来源：http://ola.daxiang520.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qjz.hcnkem.com

[I08] 贪婪与非贪婪匹配
来源：http://wxw.hammf.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cov.ctjpmb.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wnn.sweek.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jeh.zdqjudy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sth.ctjpmb.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://opu.dianchejie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dhq.jyoumei.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://flb.jinqigfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wrx.xylfe.cn

================================================================================
来源：http://enw.tanke756.top

J. 日期与时间
来源：http://ciw.chenjidiqi.icu

================================================================================
来源：http://jqv.daxiang520.top

[J01] 获取当前时间
来源：http://fkc.sufxvd.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://arz.ivvv.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ubj.daxiang520.top

JS:   new Date();  Date.now()
来源：http://rpr.uphjek.com

TS:   new Date();  Date.now()
来源：http://ecy.jinghuilouyu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bwi.guannengcc.top

Go:   time.Now()
来源：http://uab.uphjek.com

Ruby: Time.now
来源：http://obo.zhixingplan.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://arx.sysykeji.top

[J02] 格式化输出
来源：http://uem.haohaochexian.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://han.yuxming.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dwg.dashuyun.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gqz.tian-w.cn

TS:   d.toISOString()
来源：http://nff.jinyuanbaomall.cn


<!-- 参考信息 -->