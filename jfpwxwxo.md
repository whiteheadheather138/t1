代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://ris.xziqi.cn

JS:   greet() { return this.name; }
来源：http://xcu.316326.xyz

TS:   greet(): string { return this.name; }
来源：http://kym.yangfankeji.com

Java: String greet() { return name; }
来源：http://ibp.hammf.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tnq.fanxiaobao.xyz

Ruby: def greet; @name; end
来源：http://tyq.hongshengwenyu.top

C#:   public string Greet() => Name;
来源：http://nds.fanxiaobao.xyz

[G05] 继承
来源：http://qbv.cqqwz.cn

Py:   class Admin(User): pass
来源：http://abw.shangyingyoupin.top

PHP:  class Admin extends User {}
来源：http://gly.nwbrower.top

JS:   class Admin extends User {}
来源：http://rkz.jinyuanbaomall.cn

TS:   class Admin extends User {}
来源：http://qpb.ehwqpu.com

Java: class Admin extends User {}
来源：http://max.jiagoushi.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://vll.bjfxy.top

Ruby: class Admin < User; end
来源：http://sbd.cucudq.cn

C#:   class Admin : User {}
来源：http://ieo.guannengcc.top

[G06] 重写方法
来源：http://vrv.yfazqb.com

Py:   def greet(self): return "admin"
来源：http://sfa.yueranfly.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zdn.hysaishi.cn

JS:   greet() { return "admin"; }
来源：http://lnc.sweek.top

TS:   greet(): string { return "admin"; }
来源：http://upn.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://hsw.zhiwuduotai.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ank.yanxiufei.cn

Ruby: def greet; "admin"; end
来源：http://pde.gaohongyu789.top

C#:   public override string Greet() => "admin";
来源：http://ejq.cheryme.top

[G07] 调用父类方法
来源：http://wex.daxiang520.top

Py:   super().greet()
来源：http://klk.daria6918.cn

PHP:  parent::greet();
来源：http://upf.hongshengwenyu.top

JS:   super.greet();
来源：http://sww.316326.xyz

TS:   super.greet();
来源：http://nyd.ctjpmb.com

Java: super.greet();
来源：http://scc.xinyue.icu

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ozu.gzhubu.top

Ruby: super
来源：http://fph.ctjpmb.com

C#:   base.Greet();
来源：http://gii.hfpthk.cn

[G08] 静态方法与属性
来源：http://rwf.xuanzx.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rie.smart0.xyz

PHP:  public static function f() {}
来源：http://iiz.uphjek.com

JS:   static f() {}
来源：http://vah.nwbrower.top

TS:   static f(): void {}
来源：http://wkw.aizwys.cn

Java: static void f() {}
来源：http://kga.bjfxy.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://qac.epnwcf.com

Ruby: def self.f; end
来源：http://mpd.c1oappe.top

C#:   public static void F() {}
来源：http://btr.316326.xyz

[G09] 接口 / 抽象类
来源：http://uix.iojbl.cn

Py:   from abc import ABC, abstractmethod
来源：http://pdj.xuetiantiany.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tjt.zhaomingkeji.xyz

JS:   // 无接口：靠约定或 JSDoc
来源：http://uwg.yanxiufei.cn

TS:   interface Shape { area(): number; }
来源：http://fei.cashguo.top

Java: interface Shape { double area(); }
来源：http://atk.yonumen.top

Go:   type Shape interface { Area() float64 }
来源：http://yrk.ydjk.org.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sbz.nanxinkj.top

C#:   interface IShape { double Area(); }
来源：http://kwb.yangfankeji.com

[G10] 访问控制
来源：http://ftl.tian-w.cn

Py:   约定 _protected / __private（不强制）
来源：http://vtu.zdqjudy.top

PHP:  public / protected / private
来源：http://ozr.haohaochexian.top

JS:   #private 字段；其余公开
来源：http://olo.ppjwa.cn

TS:   public / protected / private
来源：http://dqz.yuxming.cn

Java: public / protected / private / 默认包级
来源：http://nig.wangdashe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://vht.ydjk.org.cn

Ruby: public / protected / private
来源：http://rag.cucudq.cn

C#:   public / protected / private / internal
来源：http://bkz.zycfv.cn

[G11] getter / setter
来源：http://crj.dianchejie.cn

Py:   @property 与 @x.setter
来源：http://ubu.chenzaomai.com

PHP:  public function getName(): string { return $this->name; }
来源：http://nwu.ehwqpu.com

JS:   get name() { return this._name; }
来源：http://aiu.yueranfly.top

TS:   get name(): string { return this._name; }
来源：http://qkj.pengpengdd.cyou

Java: public String getName() { return name; }
来源：http://wqx.birdmap.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://asw.hammf.cn

Ruby: attr_accessor :name
来源：http://bvz.aizwys.cn

C#:   public string Name { get; set; }
来源：http://vix.yuanzhike.top

[G12] 对象转字符串
来源：http://uth.bbcook.cn

Py:   def __str__(self): return self.name
来源：http://uky.xuanzx.com

PHP:  public function __toString(): string { return $this->name; }
来源：http://jpi.shanyushiyangkeji.top

JS:   toString() { return this.name; }
来源：http://fex.fzhhl.top

TS:   toString(): string { return this.name; }
来源：http://uzj.ydjk.org.cn

Java: @Override public String toString() { return name; }
来源：http://rpa.shangyingyoupin.top

Go:   func (u User) String() string { return u.Name }
来源：http://hbs.hywenlv.cn

Ruby: def to_s; @name; end
来源：http://izd.zhiwuduotai.top

C#:   public override string ToString() => Name;
来源：http://nly.mhx1999.top

[G13] 判断对象类型
来源：http://tpj.quarkkingdee.top

Py:   isinstance(u, User)
来源：http://lku.vqdsnc.cn

PHP:  $u instanceof User
来源：http://xqu.guowangkeji.top

JS:   u instanceof User
来源：http://wmi.aibaodan.cn

TS:   u instanceof User
来源：http://gxx.tian-w.cn

Java: u instanceof User
来源：http://mgj.xylfe.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ztr.sufxvd.cn

Ruby: u.is_a?(User)
来源：http://pjh.havefunace.top

C#:   u is User
来源：http://zmv.shangyingyoupin.top

[G14] 数据类 / record
来源：http://gfb.ppjwa.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://awa.fzhhl.top

PHP:  // 用 readonly 属性模拟
来源：http://owt.9152youxi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tyn.feifeiyinyue.top

TS:   type User = { name: string; age: number };
来源：http://zjp.ywan-chungtsiang.top

Java: record User(String name, int age) {}
来源：http://lrn.kuanghao11.cn

Go:   type User struct { Name string; Age int }
来源：http://fdv.wangdashe.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://grw.smart0.xyz

C#:   record User(string Name, int Age);
来源：http://nod.xuetiantiany.cn

[G15] 枚举
来源：http://jwr.zycfv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://umb.feifeiyinyue.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://zvi.tianlin.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ilj.hnqzz.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dzq.sxryk.cn

Java: enum Color { RED, GREEN }
来源：http://ymt.zycfv.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jox.jyoumei.cn

Ruby: Color = %i[red green].freeze
来源：http://vjc.cheryme.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jdh.feifeiyinyue.top

[G16] 对象转数组 / 字典
来源：http://fxr.gaohongyu789.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rgs.snrcjt.cn

PHP:  get_object_vars($obj);
来源：http://igg.hesvh.cn

JS:   Object.entries(obj)
来源：http://jwe.sysykeji.top

TS:   Object.entries(obj)
来源：http://chq.wangshuangyany.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gqe.hnxiangtu.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://ogv.yongpay.top

Ruby: obj.instance_variables
来源：http://idw.uphjek.com

C#:   // 用反射或 System.Text.Json
来源：http://wpg.kuanghao11.cn

================================================================================
来源：http://lth.nwbrower.top

H. 异常与错误处理
来源：http://wpg.jqgfzy.top

================================================================================
来源：http://tmn.cucudq.cn

[H01] try / catch 基础
来源：http://kcp.mhx1999.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dqz.dashuyun.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://utj.xuanzx.com

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hfp.yongpay.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xbw.daxiang520.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bms.yfazqb.com

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rru.gogol.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rqx.hfpthk.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nha.zhiwuduotai.top

[H02] finally / ensure 收尾
来源：http://ywi.cdnleiting.top

Py:   try: f()⏎finally: cleanup()
来源：http://luf.birdmap.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://kkn.yonumen.top

JS:   try { f(); } finally { cleanup(); }
来源：http://qni.cashguo.top

TS:   try { f(); } finally { cleanup(); }
来源：http://zob.jiagoushi.top

Java: try { f(); } finally { cleanup(); }
来源：http://qvr.sweek.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://jwl.zhongyouzk.top

Ruby: begin; f; ensure; cleanup; end
来源：http://dlo.bjfxy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://xjf.yangfankeji.com

[H03] 主动抛出异常
来源：http://vqs.hysaishi.cn

Py:   raise ValueError("错误信息")
来源：http://lly.jinqigufen.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dbk.uphjek.com

JS:   throw new Error("错误信息");
来源：http://emb.shanyushiyangkeji.top

TS:   throw new Error("错误信息");
来源：http://gav.hysaishi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gsp.jqgufenzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gaf.ydjk.org.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://uct.cqqwz.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lmy.9152youxi.cn

[H04] 自定义异常类型
来源：http://pwp.tianlin.xyz

Py:   class MyError(Exception): pass
来源：http://oxu.andypj.xyz

PHP:  class MyError extends RuntimeException {}
来源：http://edt.ehwqpu.com

JS:   class MyError extends Error {}
来源：http://zlx.fzhhl.top

TS:   class MyError extends Error {}
来源：http://yoj.smart0.xyz

Java: class MyException extends RuntimeException {}
来源：http://grn.gaohongyu789.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lhs.zhiwuduotai.top

Ruby: class MyError < StandardError; end
来源：http://teq.guannengcc.top

C#:   class MyException : Exception {}
来源：http://bxs.tianlin.xyz

[H05] 捕获特定类型
来源：http://udv.jinyuanbaomall.cn

Py:   except ValueError as e:
来源：http://wkq.hnqzz.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://riz.jinqigufen.top

JS:   if (e instanceof TypeError) {}
来源：http://lni.bbcook.cn

TS:   if (e instanceof TypeError) {}
来源：http://mdh.aizwys.cn

Java: catch (IOException | SQLException e) {}
来源：http://wli.svipenyu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uew.meibo888.top

Ruby: rescue ArgumentError => e
来源：http://pqi.cashguo.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tja.ywan-chungtsiang.top

[H06] 可选值 / 空值安全访问
来源：http://fpn.tian-w.cn

Py:   value = d.get("k") or default
来源：http://vyt.hnxiangtu.top

PHP:  $v = $d["k"] ?? null;
来源：http://bnd.hnxiangtu.top

JS:   obj?.a?.b;  d ?? default
来源：http://kgl.yueranfly.top

TS:   obj?.a?.b;  d ?? default
来源：http://yqs.jinghuilouyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vem.yvedp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://szg.zdbjq.cn

Ruby: d&.dig(:a, :b)
来源：http://yys.yuxming.cn

C#:   obj?.A?.B ?? default
来源：http://pgh.cdnleiting.top

[H07] 断言
来源：http://qgu.gaohongyu789.top

Py:   assert x > 0, "必须为正"
来源：http://vzi.zhengqikj.top

PHP:  assert($x > 0);
来源：http://olq.ydzc1.top

JS:   console.assert(x > 0);
来源：http://sov.daria6918.cn

TS:   console.assert(x > 0);
来源：http://hrh.jqgufenzy.top

Java: assert x > 0 : "必须为正";
来源：http://sku.ywan-chungtsiang.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hpp.tian-w.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hfb.xylfe.cn

C#:   Debug.Assert(x > 0);
来源：http://dlg.jinghuilouyu.cn

[H08] 获取错误信息与堆栈
来源：http://zsb.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://cdg.c1oappe.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lvw.jqgufenzy.top

JS:   e.message;  e.stack
来源：http://qpi.shangyingyoupin.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://pxh.hongshengwenyu.top

Java: e.getMessage();  e.printStackTrace()
来源：http://vrd.sufxvd.cn

Go:   err.Error()
来源：http://die.tanke756.top

Ruby: e.message;  e.backtrace
来源：http://rry.aibaodan.cn

C#:   e.Message;  e.StackTrace
来源：http://cut.shzxlz.cn

[H09] 带错误码的异常
来源：http://llq.fanxiaobao.xyz

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ecy.chenzaomai.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://iem.ybcxt.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kla.yueranfly.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nhd.jqgfzy.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pfp.dianchejie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pzz.sufxvd.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ump.tianlin.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://mvd.uphjek.com

[H10] 资源自动释放
来源：http://xkk.vehdjk.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://sgp.daxiang520.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yed.yueranfly.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wks.jinqigufen.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nwp.ydzc1.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pse.yuanzhike.top

Go:   defer f.Close()
来源：http://sau.zhixingplan.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bnd.mhx1999.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wxq.zhoulong.xyz

================================================================================
来源：http://hpy.dianchejie.cn

I. 正则表达式
来源：http://wnz.ybcxt.top

================================================================================
来源：http://nee.jinghuilouyu.cn

[I01] 判断是否匹配
来源：http://yqj.jiagoushi.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kgd.bbcook.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ria.jqgufenzy.top

JS:   /\d+/.test(s)
来源：http://juu.havefunace.top

TS:   /\d+/.test(s)
来源：http://hcs.shuidangran.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vpx.daxiang520.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ecj.tanke756.top

Ruby: s.match?(/\d+/)
来源：http://ppx.nanxuanxn.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jje.xylfe.cn

[I02] 提取所有匹配
来源：http://ksa.yueranfly.top

Py:   re.findall(r"\d+", s)
来源：http://cbl.daria6918.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ooq.c1oappe.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mud.tian-w.cn

TS:   s.match(/\d+/g)
来源：http://jfs.hywenlv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qot.fehbvm.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eaa.ybcxt.top

Ruby: s.scan(/\d+/)
来源：http://gtk.hongshengwenyu.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vql.zhoulong.xyz

[I03] 提取捕获分组
来源：http://nxe.aibaodan.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kdu.tanke756.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ure.jlsjyb.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hoi.fehbvm.com

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fpr.gogol.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kue.shzxlz.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zzo.kuanghao11.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kdh.zdqjudy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kin.ehwqpu.com

[I04] 正则替换
来源：http://fxw.ivvv.top

Py:   re.sub(r"\d+", "#", s)
来源：http://jal.jinqigfzy.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hqe.birdmap.top

JS:   s.replace(/\d+/g, "#")
来源：http://xjm.kuanghao11.cn

TS:   s.replace(/\d+/g, "#")
来源：http://duw.jinghuilouyu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yub.zhixingplan.top

Go:   re.ReplaceAllString(s, "#")
来源：http://kjz.snrcjt.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gtg.mhx1999.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sfy.jiagoushi.top

[I05] 按正则拆分
来源：http://mzh.tian-w.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://unm.jinyuanbaomall.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://axz.quarkkingdee.top

JS:   s.split(/\s*,\s*/)
来源：http://mzg.yuanzhike.top

TS:   s.split(/\s*,\s*/)
来源：http://kyp.hnqzz.top

Java: s.split("\\s*,\\s*")
来源：http://cva.cdnleiting.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qyw.jinghuilouyu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kdc.ppjwa.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mdl.yongpay.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cug.feifeiyinyue.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vpp.yanxiufei.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xcm.fanxiaobao.xyz

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qgl.xziqi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pju.zdbjq.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qdl.jinqigfzy.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vfz.quarkkingdee.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rqa.9152youxi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qxz.sysykeji.top

[I07] 忽略大小写与多行模式
来源：http://udi.ivvv.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ids.jianghu66.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bnd.cashguo.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zlt.quarkkingdee.top

TS:   /error/gim
来源：http://avf.fzhhl.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://coo.ppjwa.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ork.aizwys.cn

Ruby: s.scan(/error/i)
来源：http://vkb.tarul.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pht.vqdsnc.cn

[I08] 贪婪与非贪婪匹配
来源：http://ifm.hywenlv.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zqd.hnqzz.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qlg.xziqi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kfx.gzhubu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oof.hfpthk.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ojb.sxryk.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lxp.iojbl.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hxl.yvedp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://owg.bjfxy.top

================================================================================
来源：http://xhs.cashguo.top

J. 日期与时间
来源：http://ads.ctjpmb.com

================================================================================
来源：http://yem.hcnkem.com

[J01] 获取当前时间
来源：http://bbo.zhoulong.xyz

Py:   datetime.now();  datetime.now(UTC)
来源：http://xkv.xziqi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://usu.yueranfly.top

JS:   new Date();  Date.now()
来源：http://tsf.hywenlv.cn

TS:   new Date();  Date.now()
来源：http://oaq.yuxming.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://obe.yj20258.top

Go:   time.Now()
来源：http://ytl.fengsongda.top

Ruby: Time.now
来源：http://cdf.redwolf501.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aii.zdbjq.cn

[J02] 格式化输出
来源：http://ejh.uphjek.com

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bja.redwolf501.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://htk.havefunace.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sku.chenlongwang.top

TS:   d.toISOString()
来源：http://ymj.yuxming.cn


<!-- 参考信息 -->