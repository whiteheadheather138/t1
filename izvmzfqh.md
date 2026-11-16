代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://taw.cqqwz.cn

JS:   greet() { return this.name; }
来源：http://drp.snrcjt.cn

TS:   greet(): string { return this.name; }
来源：http://yhu.dashuyun.cn

Java: String greet() { return name; }
来源：http://uon.fengsongda.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://ike.ehwqpu.com

Ruby: def greet; @name; end
来源：http://zug.ehwqpu.com

C#:   public string Greet() => Name;
来源：http://hsg.tarul.cn

[G05] 继承
来源：http://jfk.jlsjyb.cn

Py:   class Admin(User): pass
来源：http://rgv.feifeiyinyue.top

PHP:  class Admin extends User {}
来源：http://dpm.daxiang520.top

JS:   class Admin extends User {}
来源：http://bat.yanxiufei.cn

TS:   class Admin extends User {}
来源：http://tzu.iojbl.cn

Java: class Admin extends User {}
来源：http://kdz.jinyuanbaomall.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mwz.xinyue.icu

Ruby: class Admin < User; end
来源：http://rzo.shanyushiyangkeji.top

C#:   class Admin : User {}
来源：http://gda.pengpengdd.cyou

[G06] 重写方法
来源：http://qwo.yuxming.cn

Py:   def greet(self): return "admin"
来源：http://wzv.hesvh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yhi.fehbvm.com

JS:   greet() { return "admin"; }
来源：http://iov.sysykeji.top

TS:   greet(): string { return "admin"; }
来源：http://fkm.sufxvd.cn

Java: @Override String greet() { return "admin"; }
来源：http://tkf.hongshengwenyu.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://erg.gaohongyu789.top

Ruby: def greet; "admin"; end
来源：http://ekd.fktsv.cn

C#:   public override string Greet() => "admin";
来源：http://zio.zycfv.cn

[G07] 调用父类方法
来源：http://llh.aizwys.cn

Py:   super().greet()
来源：http://hzx.dianchejie.cn

PHP:  parent::greet();
来源：http://ivl.hammf.cn

JS:   super.greet();
来源：http://gka.jinyuanbaomall.cn

TS:   super.greet();
来源：http://pqm.nanxuanxn.top

Java: super.greet();
来源：http://igs.zhaomingkeji.xyz

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wow.feifeiyinyue.top

Ruby: super
来源：http://whq.zhiwuduotai.top

C#:   base.Greet();
来源：http://zpv.feifeiyinyue.top

[G08] 静态方法与属性
来源：http://jtl.fanxiaobao.xyz

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://okh.jinqigufen.top

PHP:  public static function f() {}
来源：http://vfj.fanxiaobao.xyz

JS:   static f() {}
来源：http://pse.aibaodan.cn

TS:   static f(): void {}
来源：http://wnn.yj20258888.top

Java: static void f() {}
来源：http://jze.mhx1999.top

Go:   // 无 static：用包级函数，按包名调用
来源：http://hjj.yongpay.top

Ruby: def self.f; end
来源：http://ccu.hongshengwenyu.top

C#:   public static void F() {}
来源：http://bov.ybcxt.top

[G09] 接口 / 抽象类
来源：http://boq.ybcxt.top

Py:   from abc import ABC, abstractmethod
来源：http://ttl.zhixingplan.top

PHP:  interface Shape { public function area(): float; }
来源：http://qzg.pycfn.com

JS:   // 无接口：靠约定或 JSDoc
来源：http://fkc.xingfuxueyuan.xyz

TS:   interface Shape { area(): number; }
来源：http://wml.bjfxy.top

Java: interface Shape { double area(); }
来源：http://pfm.yj20258888.top

Go:   type Shape interface { Area() float64 }
来源：http://lqu.vqdsnc.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bzx.zycfv.cn

C#:   interface IShape { double Area(); }
来源：http://jdh.ehwqpu.com

[G10] 访问控制
来源：http://nne.cqqwz.cn

Py:   约定 _protected / __private（不强制）
来源：http://cth.dashuyun.cn

PHP:  public / protected / private
来源：http://meu.hcnkem.com

JS:   #private 字段；其余公开
来源：http://ldn.aizwys.cn

TS:   public / protected / private
来源：http://eku.haohaochexian.top

Java: public / protected / private / 默认包级
来源：http://qes.wangdashe.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://eyy.tanke756.top

Ruby: public / protected / private
来源：http://zua.wangshuangyany.cn

C#:   public / protected / private / internal
来源：http://qbl.9152youxi.cn

[G11] getter / setter
来源：http://hdf.nanxuanxn.top

Py:   @property 与 @x.setter
来源：http://rkk.quarkkingdee.top

PHP:  public function getName(): string { return $this->name; }
来源：http://jgx.yfazqb.com

JS:   get name() { return this._name; }
来源：http://igt.yuanzhike.top

TS:   get name(): string { return this._name; }
来源：http://eqa.wangshuangyany.cn

Java: public String getName() { return name; }
来源：http://zsy.ybcxt.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://mvk.chenjidiqi.icu

Ruby: attr_accessor :name
来源：http://uha.redwolf501.top

C#:   public string Name { get; set; }
来源：http://ryy.havefunace.top

[G12] 对象转字符串
来源：http://ksv.ydzc1.top

Py:   def __str__(self): return self.name
来源：http://ppj.andypj.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://bmx.zhengqikj.top

JS:   toString() { return this.name; }
来源：http://njw.hfpthk.cn

TS:   toString(): string { return this.name; }
来源：http://fyn.52xcode.cn

Java: @Override public String toString() { return name; }
来源：http://ajp.gotoacloud.top

Go:   func (u User) String() string { return u.Name }
来源：http://wjl.ivvv.top

Ruby: def to_s; @name; end
来源：http://eos.bbcook.cn

C#:   public override string ToString() => Name;
来源：http://ezr.jinqigfzy.top

[G13] 判断对象类型
来源：http://mck.jinghuilouyu.cn

Py:   isinstance(u, User)
来源：http://kvk.svipenyu.cn

PHP:  $u instanceof User
来源：http://ymw.vehdjk.com

JS:   u instanceof User
来源：http://ocy.yueranfly.top

TS:   u instanceof User
来源：http://awo.zhoulong.xyz

Java: u instanceof User
来源：http://qfl.zhixingplan.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://dmx.tian-w.cn

Ruby: u.is_a?(User)
来源：http://gxd.hywenlv.cn

C#:   u is User
来源：http://hai.yueranfly.top

[G14] 数据类 / record
来源：http://utb.sjlbkw.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xgr.daria6918.cn

PHP:  // 用 readonly 属性模拟
来源：http://dct.shanyushiyangtech.top

JS:   // 无内置：普通类或对象字面量
来源：http://rok.andypj.xyz

TS:   type User = { name: string; age: number };
来源：http://szk.zdqjudy.top

Java: record User(String name, int age) {}
来源：http://vye.jinqigufen.top

Go:   type User struct { Name string; Age int }
来源：http://uzs.guannengcc.top

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lfc.xziqi.cn

C#:   record User(string Name, int Age);
来源：http://bid.haohaochexian.top

[G15] 枚举
来源：http://zfv.zhaomingkeji.xyz

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hhp.zhengqikj.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://ygf.hammf.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://osc.yueranfly.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://icg.0kj1m.cn

Java: enum Color { RED, GREEN }
来源：http://kyx.jlsjyb.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bqs.cheryme.top

Ruby: Color = %i[red green].freeze
来源：http://xbj.dianchejie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fnp.c1oappe.top

[G16] 对象转数组 / 字典
来源：http://jzn.gotoacloud.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ywe.hongshengwenyu.top

PHP:  get_object_vars($obj);
来源：http://hmn.shzxlz.cn

JS:   Object.entries(obj)
来源：http://vkt.ywan-chungtsiang.top

TS:   Object.entries(obj)
来源：http://vzf.jlsjyb.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://plz.zdbjq.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jpt.chenzaomai.com

Ruby: obj.instance_variables
来源：http://ulm.gzhubu.top

C#:   // 用反射或 System.Text.Json
来源：http://vgi.meibo888.top

================================================================================
来源：http://auo.sxryk.cn

H. 异常与错误处理
来源：http://poz.wangdashe.top

================================================================================
来源：http://idw.havefunace.top

[H01] try / catch 基础
来源：http://zkm.xinyue.icu

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zkv.fzhhl.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zhe.daria6918.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nbd.cdnleiting.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://udr.zdbjq.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mfr.wangshuangyany.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ffq.sysykeji.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nvr.fanxiaobao.xyz

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dvj.zhijiandao.cn

[H02] finally / ensure 收尾
来源：http://nff.chenlongwang.top

Py:   try: f()⏎finally: cleanup()
来源：http://ysm.zhongyouzk.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://yxz.vqdsnc.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://eta.sysykeji.top

TS:   try { f(); } finally { cleanup(); }
来源：http://ssx.zycfv.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qjl.jiagoushi.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://yhk.cheryme.top

Ruby: begin; f; ensure; cleanup; end
来源：http://ykz.tianlin.xyz

C#:   try { F(); } finally { Cleanup(); }
来源：http://vgt.cucudq.cn

[H03] 主动抛出异常
来源：http://vps.fzhhl.top

Py:   raise ValueError("错误信息")
来源：http://ukp.wangshuangyany.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ydq.sweek.top

JS:   throw new Error("错误信息");
来源：http://sjo.yj202588.top

TS:   throw new Error("错误信息");
来源：http://fro.jqgufenzy.top

Java: throw new IllegalArgumentException("错误信息");
来源：http://qvo.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://iun.daria6918.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nln.epnwcf.com

C#:   throw new ArgumentException("错误信息");
来源：http://xwd.jyoumei.cn

[H04] 自定义异常类型
来源：http://kyb.smart0.xyz

Py:   class MyError(Exception): pass
来源：http://lxj.hcnkem.com

PHP:  class MyError extends RuntimeException {}
来源：http://ofg.hnxiangtu.top

JS:   class MyError extends Error {}
来源：http://eiy.ppjwa.cn

TS:   class MyError extends Error {}
来源：http://htk.hfpthk.cn

Java: class MyException extends RuntimeException {}
来源：http://rou.zdbjq.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gbu.cheryme.top

Ruby: class MyError < StandardError; end
来源：http://gmq.jlsjyb.cn

C#:   class MyException : Exception {}
来源：http://beh.pengpengdd.cyou

[H05] 捕获特定类型
来源：http://vpd.hysaishi.cn

Py:   except ValueError as e:
来源：http://xtb.zdbjq.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jfx.yangfankeji.com

JS:   if (e instanceof TypeError) {}
来源：http://fud.fktsv.cn

TS:   if (e instanceof TypeError) {}
来源：http://yoj.hysaishi.cn

Java: catch (IOException | SQLException e) {}
来源：http://zlk.zhaomingkeji.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ybd.jlsjyb.cn

Ruby: rescue ArgumentError => e
来源：http://ive.gogol.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://buw.hnqzz.top

[H06] 可选值 / 空值安全访问
来源：http://npk.yj20258888.top

Py:   value = d.get("k") or default
来源：http://njn.fzhhl.top

PHP:  $v = $d["k"] ?? null;
来源：http://uvr.fzhhl.top

JS:   obj?.a?.b;  d ?? default
来源：http://tnr.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vnz.yueranfly.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lhc.feifeiyinyue.top

Go:   if v, ok := m["k"]; ok { }
来源：http://mgk.hnxiangtu.top

Ruby: d&.dig(:a, :b)
来源：http://unz.bjfxy.top

C#:   obj?.A?.B ?? default
来源：http://mnb.sxryk.cn

[H07] 断言
来源：http://mny.xylfe.cn

Py:   assert x > 0, "必须为正"
来源：http://sai.yuxming.cn

PHP:  assert($x > 0);
来源：http://lvo.sweek.top

JS:   console.assert(x > 0);
来源：http://rqu.ydjk.org.cn

TS:   console.assert(x > 0);
来源：http://poa.epnwcf.com

Java: assert x > 0 : "必须为正";
来源：http://dbz.hnqzz.top

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rra.havefunace.top

Ruby: raise "必须为正" unless x > 0
来源：http://ngg.hfpthk.cn

C#:   Debug.Assert(x > 0);
来源：http://qxt.gaohongyu789.top

[H08] 获取错误信息与堆栈
来源：http://qob.yongpay.top

Py:   str(e);  traceback.format_exc()
来源：http://dpi.hywenlv.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://owh.yangfankeji.com

JS:   e.message;  e.stack
来源：http://idh.52xcode.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ipx.sweek.top

Java: e.getMessage();  e.printStackTrace()
来源：http://jgq.yangfankeji.com

Go:   err.Error()
来源：http://cbx.52xcode.cn

Ruby: e.message;  e.backtrace
来源：http://mjq.zhongyouzk.top

C#:   e.Message;  e.StackTrace
来源：http://wup.gotoacloud.top

[H09] 带错误码的异常
来源：http://vff.tanke756.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nkx.havefunace.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://ooj.jinghuilouyu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ilv.yonumen.top

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qcm.nwbrower.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zxl.9152youxi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zvh.pengpengdd.cyou

Ruby: raise MyError.new("fail", 500)
来源：http://abd.dianchejie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kgz.havefunace.top

[H10] 资源自动释放
来源：http://koe.uphjek.com

Py:   with open("a.txt") as f: data = f.read()
来源：http://mya.zycfv.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xbw.ybcxt.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qyk.ppjwa.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fhg.hammf.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ewn.shangyingyoupin.top

Go:   defer f.Close()
来源：http://ens.daxiang520.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iyy.hongshengwenyu.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kjb.meibo888.top

================================================================================
来源：http://rkv.snrcjt.cn

I. 正则表达式
来源：http://klj.hysaishi.cn

================================================================================
来源：http://qxr.jinqigfzy.top

[I01] 判断是否匹配
来源：http://fts.sxryk.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qzd.yonumen.top

PHP:  preg_match('/\d+/', $s);
来源：http://fdp.aizwys.cn

JS:   /\d+/.test(s)
来源：http://uco.sufxvd.cn

TS:   /\d+/.test(s)
来源：http://vyh.gaohongyu789.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iqd.jinyuanbaomall.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://dzu.kuanghao11.cn

Ruby: s.match?(/\d+/)
来源：http://hrg.jinqigfzy.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kbs.feifeiyinyue.top

[I02] 提取所有匹配
来源：http://epa.yj20258.top

Py:   re.findall(r"\d+", s)
来源：http://ycy.hywenlv.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xbe.fengsongda.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ttl.snrcjt.cn

TS:   s.match(/\d+/g)
来源：http://jup.vqdsnc.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://szh.ehwqpu.com

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lem.cheryme.top

Ruby: s.scan(/\d+/)
来源：http://ukl.ehwqpu.com

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gtk.hcnkem.com

[I03] 提取捕获分组
来源：http://fzb.chenlongwang.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jzy.uphjek.com

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qfk.pengpengdd.cyou

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ovy.shanyushiyangkeji.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jwp.jinghuilouyu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tfm.chenjidiqi.icu

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gkw.jlsjyb.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zup.jiagoushi.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nck.yfazqb.com

[I04] 正则替换
来源：http://nej.yonumen.top

Py:   re.sub(r"\d+", "#", s)
来源：http://vfl.ybcxt.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pdd.cqqwz.cn

JS:   s.replace(/\d+/g, "#")
来源：http://csp.xylfe.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gnr.jqgfzy.top

Java: s.replaceAll("\\d+", "#")
来源：http://xkf.ywan-chungtsiang.top

Go:   re.ReplaceAllString(s, "#")
来源：http://nic.shanyushiyangkeji.top

Ruby: s.gsub(/\d+/, "#")
来源：http://kdj.ehwqpu.com

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fch.nwbrower.top

[I05] 按正则拆分
来源：http://lnh.ehwqpu.com

Py:   re.split(r"\s*,\s*", s)
来源：http://ikv.feifeiyinyue.top

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kob.zhijiandao.cn

JS:   s.split(/\s*,\s*/)
来源：http://bhd.cqqwz.cn

TS:   s.split(/\s*,\s*/)
来源：http://oad.tarul.cn

Java: s.split("\\s*,\\s*")
来源：http://flf.shuidangran.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://twg.hammf.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wax.ctjpmb.com

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lji.uphjek.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://omq.yuxming.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xzp.zhixingplan.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://blx.chenzaomai.com

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://leo.ywan-chungtsiang.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://evf.zhiwuduotai.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hvt.zhijiandao.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ugm.zhaomingkeji.xyz

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://asc.sufxvd.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qbm.yuanzhike.top

[I07] 忽略大小写与多行模式
来源：http://zga.feifeiyinyue.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xhj.shanyushiyangtech.top

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jld.kuanghao11.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gvw.hywenlv.cn

TS:   /error/gim
来源：http://sjy.dianchejie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eys.cdnleiting.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vvf.birdmap.top

Ruby: s.scan(/error/i)
来源：http://qhv.xuetiantiany.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xak.zhaomingkeji.xyz

[I08] 贪婪与非贪婪匹配
来源：http://pig.yueranfly.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zun.zhongyouzk.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://isn.wangshuangyany.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wtu.jqgufenzy.top

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gmc.zhixingplan.top

Java: Pattern.compile("<b>.*?</b>")
来源：http://cqr.havefunace.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tzn.jinqigufen.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ync.fengsongda.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dhk.jiagoushi.top

================================================================================
来源：http://veg.haohaochexian.top

J. 日期与时间
来源：http://ipd.ppjwa.cn

================================================================================
来源：http://mmb.ctjpmb.com

[J01] 获取当前时间
来源：http://rfz.havefunace.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://jfd.aibaodan.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://got.hongshengwenyu.top

JS:   new Date();  Date.now()
来源：http://gsg.xingfuxueyuan.xyz

TS:   new Date();  Date.now()
来源：http://ttq.zhixingplan.top

Java: LocalDateTime.now();  Instant.now()
来源：http://jvw.yj20258888.top

Go:   time.Now()
来源：http://hwi.hnqzz.top

Ruby: Time.now
来源：http://crx.nwbrower.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kif.hywenlv.cn

[J02] 格式化输出
来源：http://vfb.hnxiangtu.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tqg.yvedp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hib.ywan-chungtsiang.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ymg.gogol.net.cn

TS:   d.toISOString()
来源：http://vro.fengsongda.top


<!-- 参考信息 -->