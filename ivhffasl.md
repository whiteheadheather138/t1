代发 wailian999

JS:   this.name = "x";
来源：http://pby.hesvh.cn

TS:   name: string = "x";
来源：http://klt.yvedp.cn

Java: private String name;
来源：http://tac.gotoacloud.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uwq.gaohongyu789.top

Ruby: @name = "x"
来源：http://ktz.nwbrower.top

C#:   public string Name { get; set; } = "x";
来源：http://llv.yonumen.top

[G04] 定义方法
来源：http://kob.ctjpmb.com

Py:   def greet(self): return self.name
来源：http://uay.sjlbkw.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ktl.jinghuilouyu.cn

JS:   greet() { return this.name; }
来源：http://ewc.mhx1999.top

TS:   greet(): string { return this.name; }
来源：http://kye.birdmap.top

Java: String greet() { return name; }
来源：http://yxv.havefunace.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ege.yfazqb.com

Ruby: def greet; @name; end
来源：http://txe.cheryme.top

C#:   public string Greet() => Name;
来源：http://fun.shanyushiyangtech.top

[G05] 继承
来源：http://yhs.pycfn.com

Py:   class Admin(User): pass
来源：http://xtz.yj20258.top

PHP:  class Admin extends User {}
来源：http://ynm.316326.xyz

JS:   class Admin extends User {}
来源：http://rod.jinqigfzy.top

TS:   class Admin extends User {}
来源：http://qor.jinqigufen.top

Java: class Admin extends User {}
来源：http://tqb.tianlin.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lqq.shanyushiyangkeji.top

Ruby: class Admin < User; end
来源：http://dam.yfazqb.com

C#:   class Admin : User {}
来源：http://gis.pycfn.com

[G06] 重写方法
来源：http://yxa.yonumen.top

Py:   def greet(self): return "admin"
来源：http://ahe.yj20258888.top

PHP:  public function greet(): string { return "admin"; }
来源：http://zxe.fehbvm.com

JS:   greet() { return "admin"; }
来源：http://asu.zhiwuduotai.top

TS:   greet(): string { return "admin"; }
来源：http://dze.sjlbkw.cn

Java: @Override String greet() { return "admin"; }
来源：http://pik.chenzaomai.com

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qhj.52xcode.cn

Ruby: def greet; "admin"; end
来源：http://wxp.chenlongwang.top

C#:   public override string Greet() => "admin";
来源：http://hwk.jinqigufen.top

[G07] 调用父类方法
来源：http://dsg.chenlongwang.top

Py:   super().greet()
来源：http://wbq.hongshengwenyu.top

PHP:  parent::greet();
来源：http://eux.tianlin.xyz

JS:   super.greet();
来源：http://fmx.smart0.xyz

TS:   super.greet();
来源：http://jrs.hysaishi.cn

Java: super.greet();
来源：http://gqh.yueranfly.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vcf.yj202588.top

Ruby: super
来源：http://mku.vehdjk.com

C#:   base.Greet();
来源：http://sxh.jinghuilouyu.cn

[G08] 静态方法与属性
来源：http://vyl.xuanzx.com

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lqn.ydjk.org.cn

PHP:  public static function f() {}
来源：http://err.c1oappe.top

JS:   static f() {}
来源：http://jhn.gaohongyu789.top

TS:   static f(): void {}
来源：http://tsn.chenzaomai.com

Java: static void f() {}
来源：http://zwf.zhaomingkeji.xyz

Go:   // 无 static：用包级函数，按包名调用
来源：http://tey.ivvv.top

Ruby: def self.f; end
来源：http://xcw.daxiang520.top

C#:   public static void F() {}
来源：http://ury.52xcode.cn

[G09] 接口 / 抽象类
来源：http://xwo.nanxuanxn.top

Py:   from abc import ABC, abstractmethod
来源：http://kus.tarul.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hwt.yj20258888.top

JS:   // 无接口：靠约定或 JSDoc
来源：http://goa.yonumen.top

TS:   interface Shape { area(): number; }
来源：http://irz.cqqwz.cn

Java: interface Shape { double area(); }
来源：http://bjf.hywenlv.cn

Go:   type Shape interface { Area() float64 }
来源：http://pdw.zhoulong.xyz

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ojk.daxiang520.top

C#:   interface IShape { double Area(); }
来源：http://avj.xuetiantiany.cn

[G10] 访问控制
来源：http://glt.yvedp.cn

Py:   约定 _protected / __private（不强制）
来源：http://yhf.yongpay.top

PHP:  public / protected / private
来源：http://poj.yj202588.top

JS:   #private 字段；其余公开
来源：http://qqn.fzhhl.top

TS:   public / protected / private
来源：http://jlz.cashguo.top

Java: public / protected / private / 默认包级
来源：http://ucg.hfpthk.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://num.52xcode.cn

Ruby: public / protected / private
来源：http://pvr.hesvh.cn

C#:   public / protected / private / internal
来源：http://lmn.ydzc1.top

[G11] getter / setter
来源：http://qzy.nwbrower.top

Py:   @property 与 @x.setter
来源：http://yry.xinyue.icu

PHP:  public function getName(): string { return $this->name; }
来源：http://bdm.hongshengwenyu.top

JS:   get name() { return this._name; }
来源：http://zaq.ydjk.org.cn

TS:   get name(): string { return this._name; }
来源：http://gij.xuanzx.com

Java: public String getName() { return name; }
来源：http://fkz.zhaomingkeji.xyz

Go:   func (u User) GetName() string { return u.Name }
来源：http://vlt.cheryme.top

Ruby: attr_accessor :name
来源：http://ifw.aizwys.cn

C#:   public string Name { get; set; }
来源：http://mfs.wangshuangyany.cn

[G12] 对象转字符串
来源：http://aqx.xuetiantiany.cn

Py:   def __str__(self): return self.name
来源：http://wmb.zdqjudy.top

PHP:  public function __toString(): string { return $this->name; }
来源：http://sal.jqgufenzy.top

JS:   toString() { return this.name; }
来源：http://mar.yonumen.top

TS:   toString(): string { return this.name; }
来源：http://non.feifeiyinyue.top

Java: @Override public String toString() { return name; }
来源：http://bdx.yueranfly.top

Go:   func (u User) String() string { return u.Name }
来源：http://ovv.yueranfly.top

Ruby: def to_s; @name; end
来源：http://kbu.yj202588.top

C#:   public override string ToString() => Name;
来源：http://iyv.fzhhl.top

[G13] 判断对象类型
来源：http://ylz.gaohongyu789.top

Py:   isinstance(u, User)
来源：http://izn.gzhubu.top

PHP:  $u instanceof User
来源：http://jie.wangshuangyany.cn

JS:   u instanceof User
来源：http://kds.shuidangran.top

TS:   u instanceof User
来源：http://vty.chenzaomai.com

Java: u instanceof User
来源：http://ggd.jyoumei.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gqh.chenlongwang.top

Ruby: u.is_a?(User)
来源：http://aby.guannengcc.top

C#:   u is User
来源：http://lef.guowangkeji.top

[G14] 数据类 / record
来源：http://jti.cdnleiting.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://csq.shanyushiyangtech.top

PHP:  // 用 readonly 属性模拟
来源：http://eym.9152youxi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rpp.fzhhl.top

TS:   type User = { name: string; age: number };
来源：http://owh.ppjwa.cn

Java: record User(String name, int age) {}
来源：http://zdh.jqgfzy.top

Go:   type User struct { Name string; Age int }
来源：http://srs.fanxiaobao.xyz

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://exv.epnwcf.com

C#:   record User(string Name, int Age);
来源：http://dup.zhengqikj.top

[G15] 枚举
来源：http://add.zycfv.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nqp.meibo888.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://fpt.hcnkem.com

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vlf.tarul.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://htq.yangfankeji.com

Java: enum Color { RED, GREEN }
来源：http://tsp.vehdjk.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rru.yueranfly.top

Ruby: Color = %i[red green].freeze
来源：http://uns.tianlin.xyz

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ooa.gotoacloud.top

[G16] 对象转数组 / 字典
来源：http://ljx.jinqigfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cim.hysaishi.cn

PHP:  get_object_vars($obj);
来源：http://ola.jinqigfzy.top

JS:   Object.entries(obj)
来源：http://chr.fzhhl.top

TS:   Object.entries(obj)
来源：http://fbo.feifeiyinyue.top

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xsy.aizwys.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://baa.jinqigfzy.top

Ruby: obj.instance_variables
来源：http://zaz.jianghu66.top

C#:   // 用反射或 System.Text.Json
来源：http://pjv.jianghu66.top

================================================================================
来源：http://nya.haohaochexian.top

H. 异常与错误处理
来源：http://kjo.xylfe.cn

================================================================================
来源：http://mwe.kuanghao11.cn

[H01] try / catch 基础
来源：http://bck.shangyingyoupin.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fly.cqqwz.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://anc.jqgfzy.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rhl.zhongyouzk.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pip.9152youxi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oft.fzhhl.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gsn.yueranfly.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://eop.uphjek.com

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kmw.yanxiufei.cn

[H02] finally / ensure 收尾
来源：http://bqb.feifeiyinyue.top

Py:   try: f()⏎finally: cleanup()
来源：http://jzh.gotoacloud.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://prr.yfazqb.com

JS:   try { f(); } finally { cleanup(); }
来源：http://yvu.yj202588.top

TS:   try { f(); } finally { cleanup(); }
来源：http://rik.redwolf501.top

Java: try { f(); } finally { cleanup(); }
来源：http://brc.epnwcf.com

Go:   defer cleanup()             // 函数返回时执行
来源：http://xiw.fzhhl.top

Ruby: begin; f; ensure; cleanup; end
来源：http://moz.shanyushiyangtech.top

C#:   try { F(); } finally { Cleanup(); }
来源：http://ema.smart0.xyz

[H03] 主动抛出异常
来源：http://cmz.yfazqb.com

Py:   raise ValueError("错误信息")
来源：http://mod.cdnleiting.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fjh.bbcook.cn

JS:   throw new Error("错误信息");
来源：http://csm.hysaishi.cn

TS:   throw new Error("错误信息");
来源：http://rhd.c1oappe.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://xpo.jqgufenzy.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gwk.shanyushiyangtech.top

Ruby: raise ArgumentError, "错误信息"
来源：http://bxp.sufxvd.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zwc.jinqigufen.top

[H04] 自定义异常类型
来源：http://xmb.jqgfzy.top

Py:   class MyError(Exception): pass
来源：http://bux.jlsjyb.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jzb.xinyue.icu

JS:   class MyError extends Error {}
来源：http://bfu.52xcode.cn

TS:   class MyError extends Error {}
来源：http://rzq.wangdashe.top

Java: class MyException extends RuntimeException {}
来源：http://npk.hesvh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qfy.hongshengwenyu.top

Ruby: class MyError < StandardError; end
来源：http://ypo.ywan-chungtsiang.top

C#:   class MyException : Exception {}
来源：http://uqk.bjfxy.top

[H05] 捕获特定类型
来源：http://iks.0kj1m.cn

Py:   except ValueError as e:
来源：http://wew.pengpengdd.cyou

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mxa.chenlongwang.top

JS:   if (e instanceof TypeError) {}
来源：http://hza.sufxvd.cn

TS:   if (e instanceof TypeError) {}
来源：http://spl.chenlongwang.top

Java: catch (IOException | SQLException e) {}
来源：http://tfz.316326.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lft.ppjwa.cn

Ruby: rescue ArgumentError => e
来源：http://jib.daria6918.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://eii.epnwcf.com

[H06] 可选值 / 空值安全访问
来源：http://wzx.fzhhl.top

Py:   value = d.get("k") or default
来源：http://dgj.ydjk.org.cn

PHP:  $v = $d["k"] ?? null;
来源：http://iuw.yuxming.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kwn.pengpengdd.cyou

TS:   obj?.a?.b;  d ?? default
来源：http://fpo.tianlin.xyz

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tfm.pycfn.com

Go:   if v, ok := m["k"]; ok { }
来源：http://udj.9152youxi.cn

Ruby: d&.dig(:a, :b)
来源：http://ofw.daxiang520.top

C#:   obj?.A?.B ?? default
来源：http://nht.xziqi.cn

[H07] 断言
来源：http://lqz.yj202588.top

Py:   assert x > 0, "必须为正"
来源：http://bom.yuanzhike.top

PHP:  assert($x > 0);
来源：http://wmf.iojbl.cn

JS:   console.assert(x > 0);
来源：http://ylb.xingfuxueyuan.xyz

TS:   console.assert(x > 0);
来源：http://kyy.guowangkeji.top

Java: assert x > 0 : "必须为正";
来源：http://yop.guannengcc.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kdc.cqqwz.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bac.316326.xyz

C#:   Debug.Assert(x > 0);
来源：http://vbe.cdnleiting.top

[H08] 获取错误信息与堆栈
来源：http://ync.9152youxi.cn

Py:   str(e);  traceback.format_exc()
来源：http://trk.haohaochexian.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rlv.hammf.cn

JS:   e.message;  e.stack
来源：http://ldu.haohaochexian.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://icg.jinqigufen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://akx.zhoulong.xyz

Go:   err.Error()
来源：http://yzq.yuanzhike.top

Ruby: e.message;  e.backtrace
来源：http://oaw.ppjwa.cn

C#:   e.Message;  e.StackTrace
来源：http://ppy.yj20258888.top

[H09] 带错误码的异常
来源：http://qfl.shanyushiyangkeji.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jon.hysaishi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vfj.gotoacloud.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jek.svipenyu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mvn.zhengqikj.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zxg.sweek.top

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://siy.sxryk.cn

Ruby: raise MyError.new("fail", 500)
来源：http://iza.yj20258.top

C#:   // 自定义异常类中加 Code 属性
来源：http://xkt.nanxinkj.top

[H10] 资源自动释放
来源：http://qnn.gotoacloud.top

Py:   with open("a.txt") as f: data = f.read()
来源：http://lbn.cucudq.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ixq.vqdsnc.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nps.fengsongda.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yeq.yonumen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wxp.ydzc1.top

Go:   defer f.Close()
来源：http://hzu.meibo888.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jxp.hcnkem.com

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tvc.jianghu66.top

================================================================================
来源：http://idv.daria6918.cn

I. 正则表达式
来源：http://uvs.nanxinkj.top

================================================================================
来源：http://lsr.zhijiandao.cn

[I01] 判断是否匹配
来源：http://pnd.nanxinkj.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vta.jinqigufen.top

PHP:  preg_match('/\d+/', $s);
来源：http://mub.shanyushiyangtech.top

JS:   /\d+/.test(s)
来源：http://dqz.zycfv.cn

TS:   /\d+/.test(s)
来源：http://czz.feifeiyinyue.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rqf.mhx1999.top

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lwf.xinyue.icu

Ruby: s.match?(/\d+/)
来源：http://jjd.zdqjudy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://spn.aibaodan.cn

[I02] 提取所有匹配
来源：http://jsw.fktsv.cn

Py:   re.findall(r"\d+", s)
来源：http://ttd.ctjpmb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jhd.quarkkingdee.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dwt.jinqigufen.top

TS:   s.match(/\d+/g)
来源：http://qve.9152youxi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hww.zhixingplan.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mca.pycfn.com

Ruby: s.scan(/\d+/)
来源：http://bfo.jinqigfzy.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qoo.sjlbkw.cn

[I03] 提取捕获分组
来源：http://vqa.zhixingplan.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ook.yonumen.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pjx.birdmap.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://czx.dashuyun.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://akg.shuidangran.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://byr.zhaomingkeji.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eeo.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ifv.wangshuangyany.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tzn.dashuyun.cn

[I04] 正则替换
来源：http://urk.sysykeji.top

Py:   re.sub(r"\d+", "#", s)
来源：http://zkl.yfazqb.com

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ibh.tanke756.top

JS:   s.replace(/\d+/g, "#")
来源：http://enz.cashguo.top

TS:   s.replace(/\d+/g, "#")
来源：http://uqw.jinyuanbaomall.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rks.yongpay.top

Go:   re.ReplaceAllString(s, "#")
来源：http://wjo.fanxiaobao.xyz

Ruby: s.gsub(/\d+/, "#")
来源：http://gup.jinqigufen.top

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://laj.sufxvd.cn

[I05] 按正则拆分
来源：http://yaw.daxiang520.top

Py:   re.split(r"\s*,\s*", s)
来源：http://blu.bbcook.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rxm.epnwcf.com

JS:   s.split(/\s*,\s*/)
来源：http://uvo.wangdashe.top

TS:   s.split(/\s*,\s*/)
来源：http://bzs.jyoumei.cn

Java: s.split("\\s*,\\s*")
来源：http://gwv.xylfe.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gwl.snrcjt.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fxs.dianchejie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oqi.xziqi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jdk.fengsongda.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ssn.bjfxy.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fzu.dashuyun.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iav.gotoacloud.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qaq.shangyingyoupin.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mns.ydjk.org.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://efo.tian-w.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qxz.yuxming.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bas.yj202588.top

[I07] 忽略大小写与多行模式
来源：http://uxa.fengsongda.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jau.nwbrower.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qku.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fzu.hfpthk.cn

TS:   /error/gim
来源：http://svp.vehdjk.com

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qat.birdmap.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://omm.tarul.cn

Ruby: s.scan(/error/i)
来源：http://ntb.jinqigufen.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ksd.c1oappe.top

[I08] 贪婪与非贪婪匹配
来源：http://cac.birdmap.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qdp.smart0.xyz

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qlt.zhiwuduotai.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://upb.jinyuanbaomall.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://llc.ybcxt.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://tvc.yueranfly.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nhp.jinyuanbaomall.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pjk.ybcxt.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lnt.ybcxt.top

================================================================================
来源：http://dtf.shanyushiyangtech.top

J. 日期与时间
来源：http://ovu.chenzaomai.com

================================================================================
来源：http://rlv.jinyuanbaomall.cn

[J01] 获取当前时间
来源：http://mkc.pengpengdd.cyou

Py:   datetime.now();  datetime.now(UTC)
来源：http://aqw.cashguo.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aho.guannengcc.top

JS:   new Date();  Date.now()
来源：http://ofg.52xcode.cn

TS:   new Date();  Date.now()
来源：http://zmt.fanxiaobao.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://jhp.yj20258888.top


<!-- 参考信息 -->