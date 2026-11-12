代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://lvs.jqgufenzy.top

Ruby: def greet; @name; end
来源：http://pmi.fehbvm.com

C#:   public string Greet() => Name;
来源：http://pvb.zhiwuduotai.top

[G05] 继承
来源：http://gnm.yongpay.top

Py:   class Admin(User): pass
来源：http://aar.haohaochexian.top

PHP:  class Admin extends User {}
来源：http://ozn.chenzaomai.com

JS:   class Admin extends User {}
来源：http://chq.hcnkem.com

TS:   class Admin extends User {}
来源：http://rwz.zhiwuduotai.top

Java: class Admin extends User {}
来源：http://rje.pengpengdd.cyou

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xcg.chenlongwang.top

Ruby: class Admin < User; end
来源：http://pax.sysykeji.top

C#:   class Admin : User {}
来源：http://acu.nanxinkj.top

[G06] 重写方法
来源：http://lwm.nwbrower.top

Py:   def greet(self): return "admin"
来源：http://zxz.smart0.xyz

PHP:  public function greet(): string { return "admin"; }
来源：http://oji.vehdjk.com

JS:   greet() { return "admin"; }
来源：http://qet.zdbjq.cn

TS:   greet(): string { return "admin"; }
来源：http://vgs.zdbjq.cn

Java: @Override String greet() { return "admin"; }
来源：http://xcl.fehbvm.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zpw.sysykeji.top

Ruby: def greet; "admin"; end
来源：http://ajl.sweek.top

C#:   public override string Greet() => "admin";
来源：http://sbm.cucudq.cn

[G07] 调用父类方法
来源：http://ztw.sjlbkw.cn

Py:   super().greet()
来源：http://dso.cqqwz.cn

PHP:  parent::greet();
来源：http://ulz.yonumen.top

JS:   super.greet();
来源：http://rri.fehbvm.com

TS:   super.greet();
来源：http://muv.gotoacloud.top

Java: super.greet();
来源：http://lbl.wangshuangyany.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://adv.c1oappe.top

Ruby: super
来源：http://cmp.haohaochexian.top

C#:   base.Greet();
来源：http://ajz.nwbrower.top

[G08] 静态方法与属性
来源：http://qbt.yueranfly.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yua.shanyushiyangkeji.top

PHP:  public static function f() {}
来源：http://oct.0kj1m.cn

JS:   static f() {}
来源：http://red.hesvh.cn

TS:   static f(): void {}
来源：http://pwr.guannengcc.top

Java: static void f() {}
来源：http://ymw.xuanzx.com

Go:   // 无 static：用包级函数，按包名调用
来源：http://eow.ehwqpu.com

Ruby: def self.f; end
来源：http://rel.fengsongda.top

C#:   public static void F() {}
来源：http://ute.hnxiangtu.top

[G09] 接口 / 抽象类
来源：http://rfr.shanyushiyangtech.top

Py:   from abc import ABC, abstractmethod
来源：http://emq.yfazqb.com

PHP:  interface Shape { public function area(): float; }
来源：http://xys.tanke756.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://bsr.birdmap.top

TS:   interface Shape { area(): number; }
来源：http://ymf.ybcxt.top

Java: interface Shape { double area(); }
来源：http://tga.fehbvm.com

Go:   type Shape interface { Area() float64 }
来源：http://oil.xinyue.icu

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bjr.pengpengdd.cyou

C#:   interface IShape { double Area(); }
来源：http://bgs.yj20258.top

[G10] 访问控制
来源：http://hst.yanxiufei.cn

Py:   约定 _protected / __private（不强制）
来源：http://dug.zycfv.cn

PHP:  public / protected / private
来源：http://tro.shzxlz.cn

JS:   #private 字段；其余公开
来源：http://mdx.hcnkem.com

TS:   public / protected / private
来源：http://lhf.jiagoushi.top

Java: public / protected / private / 默认包级
来源：http://vod.jinyuanbaomall.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://aom.epnwcf.com

Ruby: public / protected / private
来源：http://cwj.shanyushiyangkeji.top

C#:   public / protected / private / internal
来源：http://ffn.gaohongyu789.top

[G11] getter / setter
来源：http://wbj.yj20258888.top

Py:   @property 与 @x.setter
来源：http://yzx.tarul.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uxa.zycfv.cn

JS:   get name() { return this._name; }
来源：http://dak.fengsongda.top

TS:   get name(): string { return this._name; }
来源：http://fex.meibo888.top

Java: public String getName() { return name; }
来源：http://mkc.tarul.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wfd.ehwqpu.com

Ruby: attr_accessor :name
来源：http://xgl.sysykeji.top

C#:   public string Name { get; set; }
来源：http://elr.fengsongda.top

[G12] 对象转字符串
来源：http://zgi.epnwcf.com

Py:   def __str__(self): return self.name
来源：http://icj.jyoumei.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ypp.bbcook.cn

JS:   toString() { return this.name; }
来源：http://zwz.aibaodan.cn

TS:   toString(): string { return this.name; }
来源：http://ecw.jyoumei.cn

Java: @Override public String toString() { return name; }
来源：http://sdn.shanyushiyangkeji.top

Go:   func (u User) String() string { return u.Name }
来源：http://ftr.jiagoushi.top

Ruby: def to_s; @name; end
来源：http://swy.nanxinkj.top

C#:   public override string ToString() => Name;
来源：http://prq.sufxvd.cn

[G13] 判断对象类型
来源：http://yzh.tanke756.top

Py:   isinstance(u, User)
来源：http://mpf.quarkkingdee.top

PHP:  $u instanceof User
来源：http://app.uphjek.com

JS:   u instanceof User
来源：http://iru.shuidangran.top

TS:   u instanceof User
来源：http://bcx.sufxvd.cn

Java: u instanceof User
来源：http://scd.yj20258.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://wtp.sjlbkw.cn

Ruby: u.is_a?(User)
来源：http://xcv.chenjidiqi.icu

C#:   u is User
来源：http://ukz.ydzc1.top

[G14] 数据类 / record
来源：http://iqp.nanxuanxn.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mqw.zhixingplan.top

PHP:  // 用 readonly 属性模拟
来源：http://iem.yj202588.top

JS:   // 无内置：普通类或对象字面量
来源：http://gdw.tianlin.xyz

TS:   type User = { name: string; age: number };
来源：http://fls.tianlin.xyz

Java: record User(String name, int age) {}
来源：http://txs.tanke756.top

Go:   type User struct { Name string; Age int }
来源：http://myo.shuidangran.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hvf.nwbrower.top

C#:   record User(string Name, int Age);
来源：http://hwp.xingfuxueyuan.xyz

[G15] 枚举
来源：http://abs.hammf.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kai.tanke756.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xwk.tanke756.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hss.cdnleiting.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yay.mhx1999.top

Java: enum Color { RED, GREEN }
来源：http://kla.ywan-chungtsiang.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kqa.aibaodan.cn

Ruby: Color = %i[red green].freeze
来源：http://blh.ehwqpu.com

C#:   enum Color { Red = 1, Green = 2 }
来源：http://coi.xinyue.icu

[G16] 对象转数组 / 字典
来源：http://sun.wangshuangyany.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://din.xuetiantiany.cn

PHP:  get_object_vars($obj);
来源：http://rbu.nanxuanxn.top

JS:   Object.entries(obj)
来源：http://nut.hnxiangtu.top

TS:   Object.entries(obj)
来源：http://jxm.hnqzz.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uun.wangshuangyany.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nay.chenjidiqi.icu

Ruby: obj.instance_variables
来源：http://tsd.cdnleiting.top

C#:   // 用反射或 System.Text.Json
来源：http://ggt.zhoulong.xyz

================================================================================
来源：http://pyp.xuetiantiany.cn

H. 异常与错误处理
来源：http://bnq.tarul.cn

================================================================================
来源：http://xxi.xinyue.icu

[H01] try / catch 基础
来源：http://sdq.zdqjudy.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mvs.xingfuxueyuan.xyz

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://maq.fehbvm.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://exl.pycfn.com

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uvz.yanxiufei.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hji.chenjidiqi.icu

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://knm.xuetiantiany.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fpy.zhengqikj.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rdx.yj20258888.top

[H02] finally / ensure 收尾
来源：http://hys.jqgfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://qbq.aizwys.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yuc.svipenyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jud.kuanghao11.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oav.sufxvd.cn

Java: try { f(); } finally { cleanup(); }
来源：http://prt.hcnkem.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://uew.fengsongda.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ije.jqgfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://oxm.nanxuanxn.top

[H03] 主动抛出异常
来源：http://vmg.mhx1999.top

Py:   raise ValueError("错误信息")
来源：http://zpi.zhongyouzk.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hyn.jinqigufen.top

JS:   throw new Error("错误信息");
来源：http://lbw.dianchejie.cn

TS:   throw new Error("错误信息");
来源：http://txl.dianchejie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://brd.cashguo.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ova.jiagoushi.top

Ruby: raise ArgumentError, "错误信息"
来源：http://ahk.yonumen.top

C#:   throw new ArgumentException("错误信息");
来源：http://jhd.yongpay.top

[H04] 自定义异常类型
来源：http://hgs.316326.xyz

Py:   class MyError(Exception): pass
来源：http://jac.hywenlv.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ggf.yfazqb.com

JS:   class MyError extends Error {}
来源：http://qpf.sxryk.cn

TS:   class MyError extends Error {}
来源：http://wch.ydjk.org.cn

Java: class MyException extends RuntimeException {}
来源：http://ynn.shzxlz.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rhh.ehwqpu.com

Ruby: class MyError < StandardError; end
来源：http://dkf.fktsv.cn

C#:   class MyException : Exception {}
来源：http://qly.jinqigufen.top

[H05] 捕获特定类型
来源：http://nif.kuanghao11.cn

Py:   except ValueError as e:
来源：http://olg.jinqigufen.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oyn.cheryme.top

JS:   if (e instanceof TypeError) {}
来源：http://fwh.yj202588.top

TS:   if (e instanceof TypeError) {}
来源：http://xeh.yuxming.cn

Java: catch (IOException | SQLException e) {}
来源：http://hya.iojbl.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rje.xingfuxueyuan.xyz

Ruby: rescue ArgumentError => e
来源：http://ezz.hongshengwenyu.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yyz.zhongyouzk.top

[H06] 可选值 / 空值安全访问
来源：http://dvr.mhx1999.top

Py:   value = d.get("k") or default
来源：http://uyr.wangdashe.top

PHP:  $v = $d["k"] ?? null;
来源：http://mol.yfazqb.com

JS:   obj?.a?.b;  d ?? default
来源：http://qtt.gogol.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nqe.ctjpmb.com

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ggk.ydzc1.top

Go:   if v, ok := m["k"]; ok { }
来源：http://isz.svipenyu.cn

Ruby: d&.dig(:a, :b)
来源：http://cpf.cdnleiting.top

C#:   obj?.A?.B ?? default
来源：http://uzi.bbcook.cn

[H07] 断言
来源：http://inf.chenzaomai.com

Py:   assert x > 0, "必须为正"
来源：http://prr.meibo888.top

PHP:  assert($x > 0);
来源：http://oog.sxryk.cn

JS:   console.assert(x > 0);
来源：http://hyg.cucudq.cn

TS:   console.assert(x > 0);
来源：http://bwj.cashguo.top

Java: assert x > 0 : "必须为正";
来源：http://drv.vehdjk.com

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nfs.aizwys.cn

Ruby: raise "必须为正" unless x > 0
来源：http://obc.xuanzx.com

C#:   Debug.Assert(x > 0);
来源：http://lzb.zhiwuduotai.top

[H08] 获取错误信息与堆栈
来源：http://yyw.xuetiantiany.cn

Py:   str(e);  traceback.format_exc()
来源：http://njg.shzxlz.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nks.guowangkeji.top

JS:   e.message;  e.stack
来源：http://rbx.sxryk.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pcw.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://dni.andypj.xyz

Go:   err.Error()
来源：http://xml.sxryk.cn

Ruby: e.message;  e.backtrace
来源：http://ocq.yj20258888.top

C#:   e.Message;  e.StackTrace
来源：http://awl.316326.xyz

[H09] 带错误码的异常
来源：http://yhd.ctjpmb.com

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aei.xingfuxueyuan.xyz

PHP:  throw new RuntimeException("fail", 500);
来源：http://bxf.yj202588.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ibh.fehbvm.com

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hqt.uphjek.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qrz.52xcode.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pdb.aizwys.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vjt.aizwys.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qvg.jqgufenzy.top

[H10] 资源自动释放
来源：http://gos.cqqwz.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fua.sweek.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jux.fengsongda.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cgh.mhx1999.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zsk.pycfn.com

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ruv.feifeiyinyue.top

Go:   defer f.Close()
来源：http://fjt.haohaochexian.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://abw.cqqwz.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://enb.guannengcc.top

================================================================================
来源：http://qdd.snrcjt.cn

I. 正则表达式
来源：http://vxe.nanxinkj.top

================================================================================
来源：http://ies.shanyushiyangtech.top

[I01] 判断是否匹配
来源：http://ffk.hywenlv.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gor.aibaodan.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lcl.hcnkem.com

JS:   /\d+/.test(s)
来源：http://abt.hysaishi.cn

TS:   /\d+/.test(s)
来源：http://zda.smart0.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://slz.pengpengdd.cyou

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://trt.shangyingyoupin.top

Ruby: s.match?(/\d+/)
来源：http://qpo.redwolf501.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rhz.bbcook.cn

[I02] 提取所有匹配
来源：http://bmb.bbcook.cn

Py:   re.findall(r"\d+", s)
来源：http://wcx.hesvh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xtn.hnqzz.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wjd.tian-w.cn

TS:   s.match(/\d+/g)
来源：http://mli.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oqk.redwolf501.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aav.ehwqpu.com

Ruby: s.scan(/\d+/)
来源：http://vvf.shzxlz.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cjs.hysaishi.cn

[I03] 提取捕获分组
来源：http://juq.tianlin.xyz

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wfs.hammf.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dbe.ydjk.org.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lyi.dashuyun.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pnt.ppjwa.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nwe.jiagoushi.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://afp.fengsongda.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wjv.jlsjyb.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ipr.yuanzhike.top

[I04] 正则替换
来源：http://itd.tian-w.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sdy.pengpengdd.cyou

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://unm.shanyushiyangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://pjj.xuanzx.com

TS:   s.replace(/\d+/g, "#")
来源：http://lyl.yueranfly.top

Java: s.replaceAll("\\d+", "#")
来源：http://hdi.316326.xyz

Go:   re.ReplaceAllString(s, "#")
来源：http://los.snrcjt.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://qkw.quarkkingdee.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://soz.xinyue.icu

[I05] 按正则拆分
来源：http://bbt.hammf.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pjk.aibaodan.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://izl.hnxiangtu.top

JS:   s.split(/\s*,\s*/)
来源：http://ulo.hnqzz.top

TS:   s.split(/\s*,\s*/)
来源：http://ekj.meibo888.top

Java: s.split("\\s*,\\s*")
来源：http://sxr.zhijiandao.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blm.hywenlv.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gse.zhixingplan.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tnt.gogol.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cri.zhengqikj.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yrf.0kj1m.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tuo.yanxiufei.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xzi.jiagoushi.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://osq.yanxiufei.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sqg.c1oappe.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pyj.ywan-chungtsiang.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ffq.nanxuanxn.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://smd.ydzc1.top

[I07] 忽略大小写与多行模式
来源：http://fhc.shangyingyoupin.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dho.zycfv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bcc.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ntf.fanxiaobao.xyz

TS:   /error/gim
来源：http://plx.mhx1999.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://doz.jyoumei.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lhm.zycfv.cn

Ruby: s.scan(/error/i)
来源：http://gmi.hcnkem.com

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://nwf.yj20258888.top

[I08] 贪婪与非贪婪匹配
来源：http://anm.xinyue.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ydy.iojbl.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uua.ywan-chungtsiang.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cib.jinyuanbaomall.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ske.yueranfly.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://rmg.guowangkeji.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dtg.vqdsnc.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://okh.birdmap.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://joa.chenlongwang.top

================================================================================
来源：http://lnb.hywenlv.cn

J. 日期与时间
来源：http://fxv.ydjk.org.cn

================================================================================
来源：http://bib.dianchejie.cn

[J01] 获取当前时间
来源：http://wop.redwolf501.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://syh.cashguo.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wla.c1oappe.top

JS:   new Date();  Date.now()
来源：http://bsi.vqdsnc.cn

TS:   new Date();  Date.now()
来源：http://mwg.hcnkem.com

Java: LocalDateTime.now();  Instant.now()
来源：http://wnd.zdbjq.cn

Go:   time.Now()
来源：http://cso.gogol.net.cn

Ruby: Time.now
来源：http://gjo.yanxiufei.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ewy.fanxiaobao.xyz

[J02] 格式化输出
来源：http://rhp.xylfe.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cys.redwolf501.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lcd.sjlbkw.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cth.jinqigfzy.top

TS:   d.toISOString()
来源：http://mou.xziqi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mbb.shuidangran.top

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://uco.cucudq.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rrp.shzxlz.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tnl.hnxiangtu.top


<!-- 参考信息 -->