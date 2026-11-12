代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://wfo.daxiang520.top

JS:   greet() { return this.name; }
来源：http://kye.hcnkem.com

TS:   greet(): string { return this.name; }
来源：http://ljp.gogol.net.cn

Java: String greet() { return name; }
来源：http://fem.yfazqb.com

Go:   func (u User) Greet() string { return u.Name }
来源：http://onf.hnxiangtu.top

Ruby: def greet; @name; end
来源：http://sax.guannengcc.top

C#:   public string Greet() => Name;
来源：http://glc.redwolf501.top

[G05] 继承
来源：http://crc.zycfv.cn

Py:   class Admin(User): pass
来源：http://xgb.aibaodan.cn

PHP:  class Admin extends User {}
来源：http://ehg.jiagoushi.top

JS:   class Admin extends User {}
来源：http://kcx.sxryk.cn

TS:   class Admin extends User {}
来源：http://qve.fzhhl.top

Java: class Admin extends User {}
来源：http://ojb.pengpengdd.cyou

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qzo.gzhubu.top

Ruby: class Admin < User; end
来源：http://elk.cucudq.cn

C#:   class Admin : User {}
来源：http://yoo.mhx1999.top

[G06] 重写方法
来源：http://pzb.smart0.xyz

Py:   def greet(self): return "admin"
来源：http://rbe.gzhubu.top

PHP:  public function greet(): string { return "admin"; }
来源：http://wfd.dashuyun.cn

JS:   greet() { return "admin"; }
来源：http://fxw.jinqigfzy.top

TS:   greet(): string { return "admin"; }
来源：http://vyy.xingfuxueyuan.xyz

Java: @Override String greet() { return "admin"; }
来源：http://kos.jyoumei.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tah.aibaodan.cn

Ruby: def greet; "admin"; end
来源：http://hlt.chenzaomai.com

C#:   public override string Greet() => "admin";
来源：http://qid.iojbl.cn

[G07] 调用父类方法
来源：http://hjz.yongpay.top

Py:   super().greet()
来源：http://itj.gaohongyu789.top

PHP:  parent::greet();
来源：http://fdh.gotoacloud.top

JS:   super.greet();
来源：http://zlj.hnqzz.top

TS:   super.greet();
来源：http://gsl.hfpthk.cn

Java: super.greet();
来源：http://nvz.chenzaomai.com

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qko.hfpthk.cn

Ruby: super
来源：http://bma.pengpengdd.cyou

C#:   base.Greet();
来源：http://bhi.jinyuanbaomall.cn

[G08] 静态方法与属性
来源：http://ipn.fengsongda.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sel.tianlin.xyz

PHP:  public static function f() {}
来源：http://iar.zdbjq.cn

JS:   static f() {}
来源：http://nhq.ywan-chungtsiang.top

TS:   static f(): void {}
来源：http://xiv.jqgufenzy.top

Java: static void f() {}
来源：http://lun.kuanghao11.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nqi.ppjwa.cn

Ruby: def self.f; end
来源：http://imy.zdbjq.cn

C#:   public static void F() {}
来源：http://qlz.mhx1999.top

[G09] 接口 / 抽象类
来源：http://pkd.nwbrower.top

Py:   from abc import ABC, abstractmethod
来源：http://osc.zhoulong.xyz

PHP:  interface Shape { public function area(): float; }
来源：http://buo.zhongyouzk.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://btq.yj20258.top

TS:   interface Shape { area(): number; }
来源：http://shj.xziqi.cn

Java: interface Shape { double area(); }
来源：http://lgu.tarul.cn

Go:   type Shape interface { Area() float64 }
来源：http://ewz.ywan-chungtsiang.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tbj.ywan-chungtsiang.top

C#:   interface IShape { double Area(); }
来源：http://tvw.cashguo.top

[G10] 访问控制
来源：http://tpp.ywan-chungtsiang.top

Py:   约定 _protected / __private（不强制）
来源：http://jzy.hysaishi.cn

PHP:  public / protected / private
来源：http://qsf.iojbl.cn

JS:   #private 字段；其余公开
来源：http://dhn.shanyushiyangtech.top

TS:   public / protected / private
来源：http://map.sweek.top

Java: public / protected / private / 默认包级
来源：http://koo.chenlongwang.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://gql.yfazqb.com

Ruby: public / protected / private
来源：http://kpg.9152youxi.cn

C#:   public / protected / private / internal
来源：http://nqc.xinyue.icu

[G11] getter / setter
来源：http://jxc.fanxiaobao.xyz

Py:   @property 与 @x.setter
来源：http://asd.wangshuangyany.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dkv.9152youxi.cn

JS:   get name() { return this._name; }
来源：http://abi.snrcjt.cn

TS:   get name(): string { return this._name; }
来源：http://blq.xuanzx.com

Java: public String getName() { return name; }
来源：http://coi.tianlin.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://fuo.sxryk.cn

Ruby: attr_accessor :name
来源：http://yki.xuetiantiany.cn

C#:   public string Name { get; set; }
来源：http://ibq.svipenyu.cn

[G12] 对象转字符串
来源：http://xgy.jinyuanbaomall.cn

Py:   def __str__(self): return self.name
来源：http://qjw.zhaomingkeji.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://day.jinghuilouyu.cn

JS:   toString() { return this.name; }
来源：http://msk.shuidangran.top

TS:   toString(): string { return this.name; }
来源：http://bak.redwolf501.top

Java: @Override public String toString() { return name; }
来源：http://nja.jiagoushi.top

Go:   func (u User) String() string { return u.Name }
来源：http://txz.daxiang520.top

Ruby: def to_s; @name; end
来源：http://ilq.hywenlv.cn

C#:   public override string ToString() => Name;
来源：http://mas.snrcjt.cn

[G13] 判断对象类型
来源：http://wod.fzhhl.top

Py:   isinstance(u, User)
来源：http://qfq.jinqigufen.top

PHP:  $u instanceof User
来源：http://vcb.shanyushiyangkeji.top

JS:   u instanceof User
来源：http://ujn.aibaodan.cn

TS:   u instanceof User
来源：http://cjk.fengsongda.top

Java: u instanceof User
来源：http://uye.316326.xyz

Go:   u, ok := v.(User)            // 类型断言
来源：http://vnu.fengsongda.top

Ruby: u.is_a?(User)
来源：http://mbi.fzhhl.top

C#:   u is User
来源：http://rhd.ybcxt.top

[G14] 数据类 / record
来源：http://ocr.chenlongwang.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wsi.guannengcc.top

PHP:  // 用 readonly 属性模拟
来源：http://yek.tarul.cn

JS:   // 无内置：普通类或对象字面量
来源：http://paq.zhengqikj.top

TS:   type User = { name: string; age: number };
来源：http://rdd.zdqjudy.top

Java: record User(String name, int age) {}
来源：http://kac.jianghu66.top

Go:   type User struct { Name string; Age int }
来源：http://tzz.hywenlv.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://elt.sjlbkw.cn

C#:   record User(string Name, int Age);
来源：http://omq.gzhubu.top

[G15] 枚举
来源：http://whi.jqgfzy.top

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gxq.jyoumei.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zdf.shanyushiyangtech.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ktk.pycfn.com

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vwh.xylfe.cn

Java: enum Color { RED, GREEN }
来源：http://xea.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gfe.zycfv.cn

Ruby: Color = %i[red green].freeze
来源：http://nxu.fzhhl.top

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ghn.redwolf501.top

[G16] 对象转数组 / 字典
来源：http://pnj.svipenyu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iel.yangfankeji.com

PHP:  get_object_vars($obj);
来源：http://dth.fzhhl.top

JS:   Object.entries(obj)
来源：http://qgj.hysaishi.cn

TS:   Object.entries(obj)
来源：http://poh.daria6918.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rcx.yfazqb.com

Go:   // 手写转换，或用 mapstructure 库
来源：http://bsa.redwolf501.top

Ruby: obj.instance_variables
来源：http://vlm.yfazqb.com

C#:   // 用反射或 System.Text.Json
来源：http://vaq.gotoacloud.top

================================================================================
来源：http://rxd.feifeiyinyue.top

H. 异常与错误处理
来源：http://ysp.cucudq.cn

================================================================================
来源：http://cei.ppjwa.cn

[H01] try / catch 基础
来源：http://lyo.tarul.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://api.meibo888.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rjp.guowangkeji.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tbk.svipenyu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xnl.xuetiantiany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jcu.hongshengwenyu.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nwp.shuidangran.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jsi.ctjpmb.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yhm.tanke756.top

[H02] finally / ensure 收尾
来源：http://mjg.tianlin.xyz

Py:   try: f()⏎finally: cleanup()
来源：http://azn.316326.xyz

PHP:  try { f(); } finally { cleanup(); }
来源：http://bhm.meibo888.top

JS:   try { f(); } finally { cleanup(); }
来源：http://wng.yuanzhike.top

TS:   try { f(); } finally { cleanup(); }
来源：http://txt.pengpengdd.cyou

Java: try { f(); } finally { cleanup(); }
来源：http://rua.hnxiangtu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://oos.zhoulong.xyz

Ruby: begin; f; ensure; cleanup; end
来源：http://ooi.cucudq.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ztq.tianlin.xyz

[H03] 主动抛出异常
来源：http://agf.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://jrs.hcnkem.com

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aep.fengsongda.top

JS:   throw new Error("错误信息");
来源：http://fki.gzhubu.top

TS:   throw new Error("错误信息");
来源：http://srn.sweek.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mmg.cheryme.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hpa.xuetiantiany.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zwm.sweek.top

C#:   throw new ArgumentException("错误信息");
来源：http://etq.52xcode.cn

[H04] 自定义异常类型
来源：http://ndx.zhongyouzk.top

Py:   class MyError(Exception): pass
来源：http://btk.yfazqb.com

PHP:  class MyError extends RuntimeException {}
来源：http://ynu.wangshuangyany.cn

JS:   class MyError extends Error {}
来源：http://wkb.yuanzhike.top

TS:   class MyError extends Error {}
来源：http://lix.cucudq.cn

Java: class MyException extends RuntimeException {}
来源：http://wcx.pengpengdd.cyou

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ora.haohaochexian.top

Ruby: class MyError < StandardError; end
来源：http://hnu.hcnkem.com

C#:   class MyException : Exception {}
来源：http://urg.chenzaomai.com

[H05] 捕获特定类型
来源：http://tii.xinyue.icu

Py:   except ValueError as e:
来源：http://sig.jlsjyb.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jla.9152youxi.cn

JS:   if (e instanceof TypeError) {}
来源：http://ghq.yvedp.cn

TS:   if (e instanceof TypeError) {}
来源：http://pgc.hnxiangtu.top

Java: catch (IOException | SQLException e) {}
来源：http://nzp.cheryme.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fze.shuidangran.top

Ruby: rescue ArgumentError => e
来源：http://ljw.nanxinkj.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://emm.yj20258.top

[H06] 可选值 / 空值安全访问
来源：http://suu.0kj1m.cn

Py:   value = d.get("k") or default
来源：http://hay.dianchejie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://iai.yuanzhike.top

JS:   obj?.a?.b;  d ?? default
来源：http://fcr.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qgf.svipenyu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qaf.gogol.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lpy.jqgfzy.top

Ruby: d&.dig(:a, :b)
来源：http://jgb.fengsongda.top

C#:   obj?.A?.B ?? default
来源：http://tcl.hfpthk.cn

[H07] 断言
来源：http://mon.xziqi.cn

Py:   assert x > 0, "必须为正"
来源：http://xlj.tanke756.top

PHP:  assert($x > 0);
来源：http://kyp.yueranfly.top

JS:   console.assert(x > 0);
来源：http://crw.zycfv.cn

TS:   console.assert(x > 0);
来源：http://ias.havefunace.top

Java: assert x > 0 : "必须为正";
来源：http://ofi.dianchejie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cwj.0kj1m.cn

Ruby: raise "必须为正" unless x > 0
来源：http://net.yvedp.cn

C#:   Debug.Assert(x > 0);
来源：http://pkd.kuanghao11.cn

[H08] 获取错误信息与堆栈
来源：http://vnj.pengpengdd.cyou

Py:   str(e);  traceback.format_exc()
来源：http://zuf.yfazqb.com

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cfk.havefunace.top

JS:   e.message;  e.stack
来源：http://gqg.ywan-chungtsiang.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://iwv.gaohongyu789.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ofu.tarul.cn

Go:   err.Error()
来源：http://dqj.yvedp.cn

Ruby: e.message;  e.backtrace
来源：http://nur.tarul.cn

C#:   e.Message;  e.StackTrace
来源：http://mvz.zhaomingkeji.xyz

[H09] 带错误码的异常
来源：http://siy.xylfe.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rgg.chenzaomai.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://mgn.uphjek.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dcj.yj20258.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jbf.chenlongwang.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cox.shanyushiyangtech.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oxz.yongpay.top

Ruby: raise MyError.new("fail", 500)
来源：http://zpc.dianchejie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zfm.iojbl.cn

[H10] 资源自动释放
来源：http://vht.cucudq.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zwh.zhijiandao.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ffd.aibaodan.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dhe.gaohongyu789.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kvi.nanxinkj.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rjv.jinqigufen.top

Go:   defer f.Close()
来源：http://hpq.tarul.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vqe.zhengqikj.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cfx.kuanghao11.cn

================================================================================
来源：http://hih.tian-w.cn

I. 正则表达式
来源：http://inj.ydzc1.top

================================================================================
来源：http://jhq.zhoulong.xyz

[I01] 判断是否匹配
来源：http://xdm.svipenyu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jty.wangdashe.top

PHP:  preg_match('/\d+/', $s);
来源：http://rut.yj20258.top

JS:   /\d+/.test(s)
来源：http://itm.nwbrower.top

TS:   /\d+/.test(s)
来源：http://kuh.cashguo.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://snp.shzxlz.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://viw.tarul.cn

Ruby: s.match?(/\d+/)
来源：http://zsc.hongshengwenyu.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ewr.xuetiantiany.cn

[I02] 提取所有匹配
来源：http://gkc.dianchejie.cn

Py:   re.findall(r"\d+", s)
来源：http://fvb.ivvv.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kvq.ppjwa.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://syd.shzxlz.cn

TS:   s.match(/\d+/g)
来源：http://umc.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vdp.tanke756.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jzc.zdqjudy.top

Ruby: s.scan(/\d+/)
来源：http://sgk.ybcxt.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://csy.wangdashe.top

[I03] 提取捕获分组
来源：http://fcs.quarkkingdee.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qfj.yonumen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bql.haohaochexian.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://een.shangyingyoupin.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cad.hnxiangtu.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jle.snrcjt.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ejx.ybcxt.top

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://adg.zhixingplan.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qbh.jyoumei.cn

[I04] 正则替换
来源：http://qgb.hywenlv.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nns.hfpthk.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://oci.cqqwz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hlp.zhixingplan.top

TS:   s.replace(/\d+/g, "#")
来源：http://iek.sufxvd.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qos.zhongyouzk.top

Go:   re.ReplaceAllString(s, "#")
来源：http://hxw.xuetiantiany.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xcu.tianlin.xyz

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://obo.shanyushiyangkeji.top

[I05] 按正则拆分
来源：http://yvc.9152youxi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mqs.andypj.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bfx.cashguo.top

JS:   s.split(/\s*,\s*/)
来源：http://eio.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://mna.xuanzx.com

Java: s.split("\\s*,\\s*")
来源：http://zhq.sxryk.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fge.jinqigfzy.top

Ruby: s.split(/\s*,\s*/)
来源：http://uja.dianchejie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yaa.tian-w.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gxl.hesvh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vei.hfpthk.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://unh.cashguo.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lso.sweek.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://btz.chenzaomai.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hja.aibaodan.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dih.yangfankeji.com

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ytm.ppjwa.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bpx.wangshuangyany.cn

[I07] 忽略大小写与多行模式
来源：http://jqi.mhx1999.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wwi.zhaomingkeji.xyz

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tvp.xylfe.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wty.cheryme.top

TS:   /error/gim
来源：http://yhi.iojbl.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hnd.jinqigufen.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ewt.nanxuanxn.top

Ruby: s.scan(/error/i)
来源：http://xec.yuxming.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rjk.ehwqpu.com

[I08] 贪婪与非贪婪匹配
来源：http://mez.zhoulong.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qxl.xuetiantiany.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sew.vehdjk.com

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ndg.kuanghao11.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iex.yueranfly.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://xzc.tarul.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dsh.birdmap.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dfi.fehbvm.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://agp.ppjwa.cn

================================================================================
来源：http://lpx.chenzaomai.com

J. 日期与时间
来源：http://jkm.c1oappe.top

================================================================================
来源：http://xqr.snrcjt.cn

[J01] 获取当前时间
来源：http://bww.gaohongyu789.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://diz.yj202588.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mfc.yueranfly.top

JS:   new Date();  Date.now()
来源：http://dwv.zhengqikj.top

TS:   new Date();  Date.now()
来源：http://nsx.chenjidiqi.icu

Java: LocalDateTime.now();  Instant.now()
来源：http://udi.birdmap.top

Go:   time.Now()
来源：http://caj.hfpthk.cn

Ruby: Time.now
来源：http://tpo.gaohongyu789.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dtk.bjfxy.top

[J02] 格式化输出
来源：http://awb.xuetiantiany.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://atw.tarul.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xvo.zycfv.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://txa.aizwys.cn

TS:   d.toISOString()
来源：http://din.hcnkem.com


<!-- 参考信息 -->