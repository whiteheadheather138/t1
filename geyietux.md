代发 wailian999

Py:   class Admin(User): pass
来源：http://ddq.uphjek.com

PHP:  class Admin extends User {}
来源：http://nhz.fktsv.cn

JS:   class Admin extends User {}
来源：http://bpu.sweek.top

TS:   class Admin extends User {}
来源：http://zps.yj20258.top

Java: class Admin extends User {}
来源：http://wox.fengsongda.top

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ywg.ehwqpu.com

Ruby: class Admin < User; end
来源：http://xqr.hammf.cn

C#:   class Admin : User {}
来源：http://cmc.nanxuanxn.top

[G06] 重写方法
来源：http://hfc.gotoacloud.top

Py:   def greet(self): return "admin"
来源：http://yxz.fktsv.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zxz.yuxming.cn

JS:   greet() { return "admin"; }
来源：http://djy.zhengqikj.top

TS:   greet(): string { return "admin"; }
来源：http://byp.fktsv.cn

Java: @Override String greet() { return "admin"; }
来源：http://tpr.uphjek.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eib.tian-w.cn

Ruby: def greet; "admin"; end
来源：http://ynw.jqgfzy.top

C#:   public override string Greet() => "admin";
来源：http://lye.redwolf501.top

[G07] 调用父类方法
来源：http://zvh.cdnleiting.top

Py:   super().greet()
来源：http://fnm.havefunace.top

PHP:  parent::greet();
来源：http://gal.sweek.top

JS:   super.greet();
来源：http://edu.sweek.top

TS:   super.greet();
来源：http://vgs.tian-w.cn

Java: super.greet();
来源：http://gst.zdqjudy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sdu.ywan-chungtsiang.top

Ruby: super
来源：http://lfw.redwolf501.top

C#:   base.Greet();
来源：http://wxq.smart0.xyz

[G08] 静态方法与属性
来源：http://iyd.yueranfly.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fdx.shangyingyoupin.top

PHP:  public static function f() {}
来源：http://oiv.zhengqikj.top

JS:   static f() {}
来源：http://vpf.wangshuangyany.cn

TS:   static f(): void {}
来源：http://qoy.birdmap.top

Java: static void f() {}
来源：http://eqd.52xcode.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ugw.yj20258888.top

Ruby: def self.f; end
来源：http://rmx.zdbjq.cn

C#:   public static void F() {}
来源：http://cfd.cucudq.cn

[G09] 接口 / 抽象类
来源：http://kvc.yanxiufei.cn

Py:   from abc import ABC, abstractmethod
来源：http://mim.nanxinkj.top

PHP:  interface Shape { public function area(): float; }
来源：http://vbp.wangdashe.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://vpy.yuanzhike.top

TS:   interface Shape { area(): number; }
来源：http://kpn.hammf.cn

Java: interface Shape { double area(); }
来源：http://rce.havefunace.top

Go:   type Shape interface { Area() float64 }
来源：http://exv.snrcjt.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://buk.nanxinkj.top

C#:   interface IShape { double Area(); }
来源：http://qpv.gogol.net.cn

[G10] 访问控制
来源：http://vmh.yuxming.cn

Py:   约定 _protected / __private（不强制）
来源：http://suf.meibo888.top

PHP:  public / protected / private
来源：http://dwi.xuanzx.com

JS:   #private 字段；其余公开
来源：http://xrl.cucudq.cn

TS:   public / protected / private
来源：http://pim.xingfuxueyuan.xyz

Java: public / protected / private / 默认包级
来源：http://eva.aizwys.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://syo.vehdjk.com

Ruby: public / protected / private
来源：http://nyg.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://hwc.gotoacloud.top

[G11] getter / setter
来源：http://sfu.yj20258888.top

Py:   @property 与 @x.setter
来源：http://kvh.tanke756.top

PHP:  public function getName(): string { return $this->name; }
来源：http://hhs.xuanzx.com

JS:   get name() { return this._name; }
来源：http://ptk.shangyingyoupin.top

TS:   get name(): string { return this._name; }
来源：http://rev.bjfxy.top

Java: public String getName() { return name; }
来源：http://nab.0kj1m.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rik.ybcxt.top

Ruby: attr_accessor :name
来源：http://yxh.chenlongwang.top

C#:   public string Name { get; set; }
来源：http://fxp.nanxinkj.top

[G12] 对象转字符串
来源：http://tue.chenzaomai.com

Py:   def __str__(self): return self.name
来源：http://rpx.chenjidiqi.icu

PHP:  public function __toString(): string { return $this->name; }
来源：http://ckb.zdbjq.cn

JS:   toString() { return this.name; }
来源：http://shf.hongshengwenyu.top

TS:   toString(): string { return this.name; }
来源：http://mwi.hywenlv.cn

Java: @Override public String toString() { return name; }
来源：http://ulc.tanke756.top

Go:   func (u User) String() string { return u.Name }
来源：http://dmo.xinyue.icu

Ruby: def to_s; @name; end
来源：http://nsw.hysaishi.cn

C#:   public override string ToString() => Name;
来源：http://rki.xziqi.cn

[G13] 判断对象类型
来源：http://drm.jyoumei.cn

Py:   isinstance(u, User)
来源：http://wmg.xziqi.cn

PHP:  $u instanceof User
来源：http://mhh.sweek.top

JS:   u instanceof User
来源：http://qfi.svipenyu.cn

TS:   u instanceof User
来源：http://cdu.tianlin.xyz

Java: u instanceof User
来源：http://owu.shzxlz.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ubw.yfazqb.com

Ruby: u.is_a?(User)
来源：http://axb.hongshengwenyu.top

C#:   u is User
来源：http://ued.hywenlv.cn

[G14] 数据类 / record
来源：http://zvj.smart0.xyz

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bis.yanxiufei.cn

PHP:  // 用 readonly 属性模拟
来源：http://oob.tanke756.top

JS:   // 无内置：普通类或对象字面量
来源：http://itn.52xcode.cn

TS:   type User = { name: string; age: number };
来源：http://iyt.jiagoushi.top

Java: record User(String name, int age) {}
来源：http://cql.fzhhl.top

Go:   type User struct { Name string; Age int }
来源：http://idn.hammf.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zud.xinyue.icu

C#:   record User(string Name, int Age);
来源：http://mgv.ybcxt.top

[G15] 枚举
来源：http://tse.vqdsnc.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yhn.gotoacloud.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://xuz.316326.xyz

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jhx.fzhhl.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bzl.zhixingplan.top

Java: enum Color { RED, GREEN }
来源：http://mvk.feifeiyinyue.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://frg.sweek.top

Ruby: Color = %i[red green].freeze
来源：http://geu.ppjwa.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tmd.wangshuangyany.cn

[G16] 对象转数组 / 字典
来源：http://ini.0kj1m.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qes.zhijiandao.cn

PHP:  get_object_vars($obj);
来源：http://fot.shzxlz.cn

JS:   Object.entries(obj)
来源：http://vvf.fzhhl.top

TS:   Object.entries(obj)
来源：http://our.pengpengdd.cyou

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://byd.vqdsnc.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qrn.hesvh.cn

Ruby: obj.instance_variables
来源：http://afq.gotoacloud.top

C#:   // 用反射或 System.Text.Json
来源：http://czl.zhengqikj.top

================================================================================
来源：http://yqi.ctjpmb.com

H. 异常与错误处理
来源：http://mqb.yuanzhike.top

================================================================================
来源：http://aoq.ehwqpu.com

[H01] try / catch 基础
来源：http://sef.hcnkem.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lln.birdmap.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mke.nanxuanxn.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uma.birdmap.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://awm.mhx1999.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eaa.sweek.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gyv.smart0.xyz

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ljn.feifeiyinyue.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zjp.meibo888.top

[H02] finally / ensure 收尾
来源：http://onm.jianghu66.top

Py:   try: f()⏎finally: cleanup()
来源：http://prn.mhx1999.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://lpr.xuanzx.com

JS:   try { f(); } finally { cleanup(); }
来源：http://gwa.jqgfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rxt.pycfn.com

Java: try { f(); } finally { cleanup(); }
来源：http://rdo.smart0.xyz

Go:   defer cleanup()             // 函数返回时执行
来源：http://xyb.jinyuanbaomall.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hfu.jinqigfzy.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ttg.yanxiufei.cn

[H03] 主动抛出异常
来源：http://iyd.jinqigfzy.top

Py:   raise ValueError("错误信息")
来源：http://ruy.wangshuangyany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://iif.yuxming.cn

JS:   throw new Error("错误信息");
来源：http://zvd.fktsv.cn

TS:   throw new Error("错误信息");
来源：http://szc.jlsjyb.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kdz.nanxinkj.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ziq.ydjk.org.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cvn.fehbvm.com

C#:   throw new ArgumentException("错误信息");
来源：http://tuo.zdbjq.cn

[H04] 自定义异常类型
来源：http://dfe.uphjek.com

Py:   class MyError(Exception): pass
来源：http://izx.ehwqpu.com

PHP:  class MyError extends RuntimeException {}
来源：http://tck.zdbjq.cn

JS:   class MyError extends Error {}
来源：http://gjr.yueranfly.top

TS:   class MyError extends Error {}
来源：http://oib.xylfe.cn

Java: class MyException extends RuntimeException {}
来源：http://yas.quarkkingdee.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wxd.andypj.xyz

Ruby: class MyError < StandardError; end
来源：http://inh.chenjidiqi.icu

C#:   class MyException : Exception {}
来源：http://yic.tian-w.cn

[H05] 捕获特定类型
来源：http://gme.9152youxi.cn

Py:   except ValueError as e:
来源：http://gdm.yfazqb.com

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kfd.nwbrower.top

JS:   if (e instanceof TypeError) {}
来源：http://nfl.jinyuanbaomall.cn

TS:   if (e instanceof TypeError) {}
来源：http://gge.dianchejie.cn

Java: catch (IOException | SQLException e) {}
来源：http://pga.316326.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lqw.c1oappe.top

Ruby: rescue ArgumentError => e
来源：http://lpf.gogol.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mkm.yangfankeji.com

[H06] 可选值 / 空值安全访问
来源：http://hxd.316326.xyz

Py:   value = d.get("k") or default
来源：http://kqb.fanxiaobao.xyz

PHP:  $v = $d["k"] ?? null;
来源：http://zmr.svipenyu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cwg.redwolf501.top

TS:   obj?.a?.b;  d ?? default
来源：http://upi.zhaomingkeji.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xym.chenzaomai.com

Go:   if v, ok := m["k"]; ok { }
来源：http://gjm.mhx1999.top

Ruby: d&.dig(:a, :b)
来源：http://enb.birdmap.top

C#:   obj?.A?.B ?? default
来源：http://yco.shangyingyoupin.top

[H07] 断言
来源：http://nbd.zhongyouzk.top

Py:   assert x > 0, "必须为正"
来源：http://dyv.jyoumei.cn

PHP:  assert($x > 0);
来源：http://dgh.yj20258888.top

JS:   console.assert(x > 0);
来源：http://glk.pycfn.com

TS:   console.assert(x > 0);
来源：http://oij.cqqwz.cn

Java: assert x > 0 : "必须为正";
来源：http://tjt.tianlin.xyz

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uet.daria6918.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vsz.daxiang520.top

C#:   Debug.Assert(x > 0);
来源：http://kwf.wangdashe.top

[H08] 获取错误信息与堆栈
来源：http://pvy.xuanzx.com

Py:   str(e);  traceback.format_exc()
来源：http://bbl.sxryk.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://efd.hywenlv.cn

JS:   e.message;  e.stack
来源：http://jmd.mhx1999.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://cpu.ywan-chungtsiang.top

Java: e.getMessage();  e.printStackTrace()
来源：http://axt.zhijiandao.cn

Go:   err.Error()
来源：http://boe.fktsv.cn

Ruby: e.message;  e.backtrace
来源：http://pwc.gogol.net.cn

C#:   e.Message;  e.StackTrace
来源：http://lzv.ctjpmb.com

[H09] 带错误码的异常
来源：http://xxm.0kj1m.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aas.jqgufenzy.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://wdh.yangfankeji.com

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sxh.ivvv.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ims.chenjidiqi.icu

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cgl.nanxinkj.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xwg.ywan-chungtsiang.top

Ruby: raise MyError.new("fail", 500)
来源：http://tnt.xingfuxueyuan.xyz

C#:   // 自定义异常类中加 Code 属性
来源：http://oqz.mhx1999.top

[H10] 资源自动释放
来源：http://chl.nwbrower.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://cgn.birdmap.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://umj.pycfn.com

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qdg.feifeiyinyue.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ptk.yj20258.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pps.chenjidiqi.icu

Go:   defer f.Close()
来源：http://uto.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ebo.yonumen.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bls.shangyingyoupin.top

================================================================================
来源：http://yrz.dashuyun.cn

I. 正则表达式
来源：http://ozi.haohaochexian.top

================================================================================
来源：http://kdi.tianlin.xyz

[I01] 判断是否匹配
来源：http://kox.mhx1999.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hrg.epnwcf.com

PHP:  preg_match('/\d+/', $s);
来源：http://fhw.aizwys.cn

JS:   /\d+/.test(s)
来源：http://rol.yj20258888.top

TS:   /\d+/.test(s)
来源：http://utv.andypj.xyz

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://phy.tianlin.xyz

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xvr.c1oappe.top

Ruby: s.match?(/\d+/)
来源：http://bpo.iojbl.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pwr.kuanghao11.cn

[I02] 提取所有匹配
来源：http://rmk.ybcxt.top

Py:   re.findall(r"\d+", s)
来源：http://iew.guowangkeji.top

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yiu.dianchejie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://lqg.guowangkeji.top

TS:   s.match(/\d+/g)
来源：http://qjv.zhengqikj.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hen.yongpay.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kwl.pengpengdd.cyou

Ruby: s.scan(/\d+/)
来源：http://dmo.guannengcc.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nnb.ivvv.top

[I03] 提取捕获分组
来源：http://qlh.yuxming.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pyz.ppjwa.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pki.jiagoushi.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://skb.hfpthk.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wkv.andypj.xyz

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://utu.guowangkeji.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aef.316326.xyz

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ppy.jqgufenzy.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dcs.yj20258888.top

[I04] 正则替换
来源：http://qne.daxiang520.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vii.kuanghao11.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lsf.guowangkeji.top

JS:   s.replace(/\d+/g, "#")
来源：http://pcl.zhijiandao.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xth.hongshengwenyu.top

Java: s.replaceAll("\\d+", "#")
来源：http://sfz.yanxiufei.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xun.fzhhl.top

Ruby: s.gsub(/\d+/, "#")
来源：http://pra.mhx1999.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tsv.0kj1m.cn

[I05] 按正则拆分
来源：http://nme.yueranfly.top

Py:   re.split(r"\s*,\s*", s)
来源：http://cqw.0kj1m.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ecf.haohaochexian.top

JS:   s.split(/\s*,\s*/)
来源：http://xii.zhaomingkeji.xyz

TS:   s.split(/\s*,\s*/)
来源：http://vzm.hnxiangtu.top

Java: s.split("\\s*,\\s*")
来源：http://dtk.jinghuilouyu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qut.shangyingyoupin.top

Ruby: s.split(/\s*,\s*/)
来源：http://vuv.cdnleiting.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vuq.9152youxi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xaz.hcnkem.com

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qda.ybcxt.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tot.ydjk.org.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xot.nanxuanxn.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://anl.daria6918.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lvk.redwolf501.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jcr.xziqi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rct.hnqzz.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://puz.zdqjudy.top

[I07] 忽略大小写与多行模式
来源：http://dhu.gogol.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kvd.hywenlv.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rgd.yfazqb.com

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hdd.zhijiandao.cn

TS:   /error/gim
来源：http://ivq.chenjidiqi.icu

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lmk.hfpthk.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pil.bbcook.cn

Ruby: s.scan(/error/i)
来源：http://rvk.smart0.xyz

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hhn.guowangkeji.top

[I08] 贪婪与非贪婪匹配
来源：http://lsd.havefunace.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://flz.hcnkem.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fls.iojbl.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bjs.gzhubu.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vrz.zhengqikj.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://ack.ivvv.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ghf.epnwcf.com

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://way.hcnkem.com

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cdd.nanxinkj.top

================================================================================
来源：http://vno.hysaishi.cn

J. 日期与时间
来源：http://zki.epnwcf.com

================================================================================
来源：http://pnv.52xcode.cn

[J01] 获取当前时间
来源：http://ajc.vqdsnc.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vpa.yonumen.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://odx.jinghuilouyu.cn

JS:   new Date();  Date.now()
来源：http://eio.zycfv.cn

TS:   new Date();  Date.now()
来源：http://yus.xylfe.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://euv.hysaishi.cn

Go:   time.Now()
来源：http://rzd.sxryk.cn

Ruby: Time.now
来源：http://ent.jqgfzy.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uel.9152youxi.cn

[J02] 格式化输出
来源：http://iov.hfpthk.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ysr.jinqigufen.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://obw.zhongyouzk.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gbn.zhengqikj.top

TS:   d.toISOString()
来源：http://onq.cashguo.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dnk.cqqwz.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yuw.fzhhl.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kwx.guowangkeji.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gkt.shuidangran.top

[J03] 字符串解析为日期
来源：http://jgd.zhijiandao.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://laf.dashuyun.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://krq.gzhubu.top

JS:   new Date("2024-01-02")
来源：http://pbi.yangfankeji.com


<!-- 参考信息 -->