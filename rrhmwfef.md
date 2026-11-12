代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://edr.zhaomingkeji.xyz

JS:   greet() { return this.name; }
来源：http://kte.epnwcf.com

TS:   greet(): string { return this.name; }
来源：http://tlt.nanxuanxn.top

Java: String greet() { return name; }
来源：http://wri.smart0.xyz

Go:   func (u User) Greet() string { return u.Name }
来源：http://ulq.gotoacloud.top

Ruby: def greet; @name; end
来源：http://zkf.bjfxy.top

C#:   public string Greet() => Name;
来源：http://uon.svipenyu.cn

[G05] 继承
来源：http://pkd.ivvv.top

Py:   class Admin(User): pass
来源：http://dzn.cashguo.top

PHP:  class Admin extends User {}
来源：http://law.pycfn.com

JS:   class Admin extends User {}
来源：http://hci.zhijiandao.cn

TS:   class Admin extends User {}
来源：http://giq.yongpay.top

Java: class Admin extends User {}
来源：http://nto.ybcxt.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wio.hcnkem.com

Ruby: class Admin < User; end
来源：http://bez.ctjpmb.com

C#:   class Admin : User {}
来源：http://ogm.hammf.cn

[G06] 重写方法
来源：http://rmw.hcnkem.com

Py:   def greet(self): return "admin"
来源：http://kbz.birdmap.top

PHP:  public function greet(): string { return "admin"; }
来源：http://mch.fanxiaobao.xyz

JS:   greet() { return "admin"; }
来源：http://tdu.aibaodan.cn

TS:   greet(): string { return "admin"; }
来源：http://mrm.hnqzz.top

Java: @Override String greet() { return "admin"; }
来源：http://emq.gaohongyu789.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lwt.jianghu66.top

Ruby: def greet; "admin"; end
来源：http://mvr.gogol.net.cn

C#:   public override string Greet() => "admin";
来源：http://vfa.jqgufenzy.top

[G07] 调用父类方法
来源：http://hsc.zdbjq.cn

Py:   super().greet()
来源：http://bwn.zdbjq.cn

PHP:  parent::greet();
来源：http://yig.gotoacloud.top

JS:   super.greet();
来源：http://xgf.yj20258888.top

TS:   super.greet();
来源：http://pgy.shangyingyoupin.top

Java: super.greet();
来源：http://ikv.fanxiaobao.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://aqr.fanxiaobao.xyz

Ruby: super
来源：http://oyn.yanxiufei.cn

C#:   base.Greet();
来源：http://eeq.tian-w.cn

[G08] 静态方法与属性
来源：http://jmv.jqgufenzy.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ysf.gotoacloud.top

PHP:  public static function f() {}
来源：http://btp.pengpengdd.cyou

JS:   static f() {}
来源：http://ouk.yanxiufei.cn

TS:   static f(): void {}
来源：http://vby.zhijiandao.cn

Java: static void f() {}
来源：http://xqf.jyoumei.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zoi.nanxinkj.top

Ruby: def self.f; end
来源：http://gbg.sjlbkw.cn

C#:   public static void F() {}
来源：http://oer.jinyuanbaomall.cn

[G09] 接口 / 抽象类
来源：http://kew.haohaochexian.top

Py:   from abc import ABC, abstractmethod
来源：http://rfp.hfpthk.cn

PHP:  interface Shape { public function area(): float; }
来源：http://waf.nwbrower.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://wdf.jyoumei.cn

TS:   interface Shape { area(): number; }
来源：http://hjs.ivvv.top

Java: interface Shape { double area(); }
来源：http://ovw.tanke756.top

Go:   type Shape interface { Area() float64 }
来源：http://beo.uphjek.com

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://azx.aibaodan.cn

C#:   interface IShape { double Area(); }
来源：http://iai.shuidangran.top

[G10] 访问控制
来源：http://far.ctjpmb.com

Py:   约定 _protected / __private（不强制）
来源：http://ean.jinqigufen.top

PHP:  public / protected / private
来源：http://xww.mhx1999.top

JS:   #private 字段；其余公开
来源：http://dhd.shuidangran.top

TS:   public / protected / private
来源：http://ejb.cheryme.top

Java: public / protected / private / 默认包级
来源：http://tiz.nanxuanxn.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://plh.zhoulong.xyz

Ruby: public / protected / private
来源：http://jyd.daxiang520.top

C#:   public / protected / private / internal
来源：http://bzc.yuanzhike.top

[G11] getter / setter
来源：http://asy.epnwcf.com

Py:   @property 与 @x.setter
来源：http://yyw.tianlin.xyz

PHP:  public function getName(): string { return $this->name; }
来源：http://xrb.zhongyouzk.top

JS:   get name() { return this._name; }
来源：http://iei.fanxiaobao.xyz

TS:   get name(): string { return this._name; }
来源：http://lmr.nanxuanxn.top

Java: public String getName() { return name; }
来源：http://oqx.redwolf501.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://yve.cqqwz.cn

Ruby: attr_accessor :name
来源：http://zbm.0kj1m.cn

C#:   public string Name { get; set; }
来源：http://kje.ppjwa.cn

[G12] 对象转字符串
来源：http://ssv.yangfankeji.com

Py:   def __str__(self): return self.name
来源：http://jtg.yuxming.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pbm.hnxiangtu.top

JS:   toString() { return this.name; }
来源：http://hev.andypj.xyz

TS:   toString(): string { return this.name; }
来源：http://rjj.cheryme.top

Java: @Override public String toString() { return name; }
来源：http://zgk.zdqjudy.top

Go:   func (u User) String() string { return u.Name }
来源：http://fog.yanxiufei.cn

Ruby: def to_s; @name; end
来源：http://upy.yvedp.cn

C#:   public override string ToString() => Name;
来源：http://laj.sjlbkw.cn

[G13] 判断对象类型
来源：http://umi.yj202588.top

Py:   isinstance(u, User)
来源：http://oyi.yuxming.cn

PHP:  $u instanceof User
来源：http://gdx.daria6918.cn

JS:   u instanceof User
来源：http://qxj.hysaishi.cn

TS:   u instanceof User
来源：http://czk.shangyingyoupin.top

Java: u instanceof User
来源：http://dtk.shanyushiyangtech.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://gci.daria6918.cn

Ruby: u.is_a?(User)
来源：http://ukn.jinqigufen.top

C#:   u is User
来源：http://mzl.hammf.cn

[G14] 数据类 / record
来源：http://mig.fanxiaobao.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lda.jyoumei.cn

PHP:  // 用 readonly 属性模拟
来源：http://ofe.zhengqikj.top

JS:   // 无内置：普通类或对象字面量
来源：http://scn.hfpthk.cn

TS:   type User = { name: string; age: number };
来源：http://xuz.yuxming.cn

Java: record User(String name, int age) {}
来源：http://twy.zycfv.cn

Go:   type User struct { Name string; Age int }
来源：http://nzq.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://aqk.cashguo.top

C#:   record User(string Name, int Age);
来源：http://lmo.gogol.net.cn

[G15] 枚举
来源：http://pzi.svipenyu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zon.dashuyun.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bod.jyoumei.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oxy.ydzc1.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hlx.meibo888.top

Java: enum Color { RED, GREEN }
来源：http://gij.smart0.xyz

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mxw.quarkkingdee.top

Ruby: Color = %i[red green].freeze
来源：http://mgl.gogol.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gce.nanxuanxn.top

[G16] 对象转数组 / 字典
来源：http://kpl.fengsongda.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://out.ppjwa.cn

PHP:  get_object_vars($obj);
来源：http://zvj.daria6918.cn

JS:   Object.entries(obj)
来源：http://awa.zhiwuduotai.top

TS:   Object.entries(obj)
来源：http://wki.zhijiandao.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://osu.ywan-chungtsiang.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://oco.dianchejie.cn

Ruby: obj.instance_variables
来源：http://ejw.hywenlv.cn

C#:   // 用反射或 System.Text.Json
来源：http://sdo.xingfuxueyuan.xyz

================================================================================
来源：http://mbh.gogol.net.cn

H. 异常与错误处理
来源：http://vst.hfpthk.cn

================================================================================
来源：http://mah.shzxlz.cn

[H01] try / catch 基础
来源：http://twr.wangshuangyany.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hau.epnwcf.com

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://esi.yj20258.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vla.cucudq.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sbd.jinyuanbaomall.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kiv.zhaomingkeji.xyz

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://czr.yuanzhike.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zqj.ehwqpu.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bna.jqgfzy.top

[H02] finally / ensure 收尾
来源：http://mjd.jinqigfzy.top

Py:   try: f()⏎finally: cleanup()
来源：http://uet.ybcxt.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://fgy.cheryme.top

JS:   try { f(); } finally { cleanup(); }
来源：http://kzy.hongshengwenyu.top

TS:   try { f(); } finally { cleanup(); }
来源：http://avb.yj202588.top

Java: try { f(); } finally { cleanup(); }
来源：http://fis.xuetiantiany.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jul.cdnleiting.top

Ruby: begin; f; ensure; cleanup; end
来源：http://skh.kuanghao11.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ndx.shangyingyoupin.top

[H03] 主动抛出异常
来源：http://yer.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://aqb.daria6918.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://obj.aibaodan.cn

JS:   throw new Error("错误信息");
来源：http://unm.tanke756.top

TS:   throw new Error("错误信息");
来源：http://gex.shuidangran.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://mwj.pengpengdd.cyou

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pda.0kj1m.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qqg.ywan-chungtsiang.top

C#:   throw new ArgumentException("错误信息");
来源：http://jyz.jyoumei.cn

[H04] 自定义异常类型
来源：http://eww.hfpthk.cn

Py:   class MyError(Exception): pass
来源：http://jvx.pycfn.com

PHP:  class MyError extends RuntimeException {}
来源：http://ruj.fehbvm.com

JS:   class MyError extends Error {}
来源：http://tzf.cdnleiting.top

TS:   class MyError extends Error {}
来源：http://dkn.yj20258888.top

Java: class MyException extends RuntimeException {}
来源：http://vlg.hesvh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://azb.hnxiangtu.top

Ruby: class MyError < StandardError; end
来源：http://chu.guannengcc.top

C#:   class MyException : Exception {}
来源：http://tre.hesvh.cn

[H05] 捕获特定类型
来源：http://cjy.yongpay.top

Py:   except ValueError as e:
来源：http://rne.daxiang520.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vop.mhx1999.top

JS:   if (e instanceof TypeError) {}
来源：http://vlm.zycfv.cn

TS:   if (e instanceof TypeError) {}
来源：http://urd.zhoulong.xyz

Java: catch (IOException | SQLException e) {}
来源：http://fps.redwolf501.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pfs.hesvh.cn

Ruby: rescue ArgumentError => e
来源：http://mwx.haohaochexian.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fxk.9152youxi.cn

[H06] 可选值 / 空值安全访问
来源：http://hfu.yangfankeji.com

Py:   value = d.get("k") or default
来源：http://yrh.xinyue.icu

PHP:  $v = $d["k"] ?? null;
来源：http://mbp.chenzaomai.com

JS:   obj?.a?.b;  d ?? default
来源：http://vqi.haohaochexian.top

TS:   obj?.a?.b;  d ?? default
来源：http://paq.hnxiangtu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yhc.haohaochexian.top

Go:   if v, ok := m["k"]; ok { }
来源：http://owx.iojbl.cn

Ruby: d&.dig(:a, :b)
来源：http://yly.shuidangran.top

C#:   obj?.A?.B ?? default
来源：http://pnp.zhongyouzk.top

[H07] 断言
来源：http://fdb.zdqjudy.top

Py:   assert x > 0, "必须为正"
来源：http://twg.ywan-chungtsiang.top

PHP:  assert($x > 0);
来源：http://fws.cdnleiting.top

JS:   console.assert(x > 0);
来源：http://vdp.guowangkeji.top

TS:   console.assert(x > 0);
来源：http://bsc.gogol.net.cn

Java: assert x > 0 : "必须为正";
来源：http://ypp.ppjwa.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vwg.316326.xyz

Ruby: raise "必须为正" unless x > 0
来源：http://trn.jiagoushi.top

C#:   Debug.Assert(x > 0);
来源：http://chp.havefunace.top

[H08] 获取错误信息与堆栈
来源：http://wav.pengpengdd.cyou

Py:   str(e);  traceback.format_exc()
来源：http://gpm.meibo888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jju.52xcode.cn

JS:   e.message;  e.stack
来源：http://ybg.jinqigfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://mup.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://emb.mhx1999.top

Go:   err.Error()
来源：http://jvg.zdqjudy.top

Ruby: e.message;  e.backtrace
来源：http://tqz.daxiang520.top

C#:   e.Message;  e.StackTrace
来源：http://lyj.cdnleiting.top

[H09] 带错误码的异常
来源：http://val.redwolf501.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iou.pengpengdd.cyou

PHP:  throw new RuntimeException("fail", 500);
来源：http://hxb.fehbvm.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qje.snrcjt.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ucy.mhx1999.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://skp.jinqigufen.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jhc.yonumen.top

Ruby: raise MyError.new("fail", 500)
来源：http://qvx.cucudq.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yoo.xziqi.cn

[H10] 资源自动释放
来源：http://ezs.sjlbkw.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://chg.yongpay.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jof.sxryk.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jqm.snrcjt.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vza.yuxming.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dee.haohaochexian.top

Go:   defer f.Close()
来源：http://bsv.chenzaomai.com

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qkr.zhongyouzk.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pqh.jlsjyb.cn

================================================================================
来源：http://ill.yvedp.cn

I. 正则表达式
来源：http://dki.ybcxt.top

================================================================================
来源：http://kuq.nanxinkj.top

[I01] 判断是否匹配
来源：http://nyl.hongshengwenyu.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mfo.iojbl.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zsc.fanxiaobao.xyz

JS:   /\d+/.test(s)
来源：http://jzw.daria6918.cn

TS:   /\d+/.test(s)
来源：http://mjq.zhengqikj.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://khc.xingfuxueyuan.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dnw.snrcjt.cn

Ruby: s.match?(/\d+/)
来源：http://ksy.shangyingyoupin.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cxb.aizwys.cn

[I02] 提取所有匹配
来源：http://glz.chenlongwang.top

Py:   re.findall(r"\d+", s)
来源：http://gkr.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lkn.fanxiaobao.xyz

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fzw.dianchejie.cn

TS:   s.match(/\d+/g)
来源：http://xzo.zhijiandao.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dut.yueranfly.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://chw.316326.xyz

Ruby: s.scan(/\d+/)
来源：http://lju.52xcode.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://emx.gogol.net.cn

[I03] 提取捕获分组
来源：http://gua.c1oappe.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nev.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qlx.pengpengdd.cyou

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mzs.zhixingplan.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wba.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hmn.fengsongda.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pvb.yuxming.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wyd.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://otf.mhx1999.top

[I04] 正则替换
来源：http://ybu.ybcxt.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bli.xylfe.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vpi.wangdashe.top

JS:   s.replace(/\d+/g, "#")
来源：http://bcg.316326.xyz

TS:   s.replace(/\d+/g, "#")
来源：http://vtt.xingfuxueyuan.xyz

Java: s.replaceAll("\\d+", "#")
来源：http://cbd.zhijiandao.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mlm.hywenlv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zzf.yj20258888.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lgg.sweek.top

[I05] 按正则拆分
来源：http://dmr.dianchejie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ypq.cqqwz.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://out.yongpay.top

JS:   s.split(/\s*,\s*/)
来源：http://err.gogol.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://znp.52xcode.cn

Java: s.split("\\s*,\\s*")
来源：http://vsv.epnwcf.com

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kai.daxiang520.top

Ruby: s.split(/\s*,\s*/)
来源：http://qsf.xinyue.icu

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jgx.xuanzx.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vmg.yanxiufei.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cru.ctjpmb.com

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://esf.haohaochexian.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tbj.chenzaomai.com

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jwa.yangfankeji.com

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nki.fengsongda.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://awy.svipenyu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wgb.smart0.xyz

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qef.ivvv.top

[I07] 忽略大小写与多行模式
来源：http://jpm.yueranfly.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://che.ivvv.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gxf.yj202588.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aqy.tarul.cn

TS:   /error/gim
来源：http://pzf.jyoumei.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fmq.zhengqikj.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ips.shzxlz.cn

Ruby: s.scan(/error/i)
来源：http://uvk.jinqigufen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xef.yuxming.cn

[I08] 贪婪与非贪婪匹配
来源：http://vms.chenjidiqi.icu

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://riu.52xcode.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://knt.hnxiangtu.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://err.jinghuilouyu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://adv.redwolf501.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://fkf.0kj1m.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cko.52xcode.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dcf.fzhhl.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ppc.jiagoushi.top

================================================================================
来源：http://ksr.hnqzz.top

J. 日期与时间
来源：http://eya.hywenlv.cn

================================================================================
来源：http://kir.tanke756.top

[J01] 获取当前时间
来源：http://omx.redwolf501.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://dsr.pengpengdd.cyou

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lju.chenjidiqi.icu

JS:   new Date();  Date.now()
来源：http://gst.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://gxj.ctjpmb.com

Java: LocalDateTime.now();  Instant.now()
来源：http://cmv.yueranfly.top

Go:   time.Now()
来源：http://xst.zhengqikj.top

Ruby: Time.now
来源：http://fxz.cashguo.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gey.zhijiandao.cn

[J02] 格式化输出
来源：http://zho.tianlin.xyz

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wer.gotoacloud.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://roh.hcnkem.com

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bmx.wangdashe.top

TS:   d.toISOString()
来源：http://ouz.hnxiangtu.top


<!-- 参考信息 -->