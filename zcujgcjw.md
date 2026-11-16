代发 wailian999

JS:   this.name = "x";
来源：http://nem.xuetiantiany.cn

TS:   name: string = "x";
来源：http://jem.hysaishi.cn

Java: private String name;
来源：http://biv.jiagoushi.top

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wop.gotoacloud.top

Ruby: @name = "x"
来源：http://rom.dianchejie.cn

C#:   public string Name { get; set; } = "x";
来源：http://sid.xziqi.cn

[G04] 定义方法
来源：http://poe.cashguo.top

Py:   def greet(self): return self.name
来源：http://pik.nanxinkj.top

PHP:  public function greet(): string { return $this->name; }
来源：http://lwe.snrcjt.cn

JS:   greet() { return this.name; }
来源：http://rce.jyoumei.cn

TS:   greet(): string { return this.name; }
来源：http://ytd.zdqjudy.top

Java: String greet() { return name; }
来源：http://oli.sweek.top

Go:   func (u User) Greet() string { return u.Name }
来源：http://vdu.jyoumei.cn

Ruby: def greet; @name; end
来源：http://rsm.sjlbkw.cn

C#:   public string Greet() => Name;
来源：http://hyb.hysaishi.cn

[G05] 继承
来源：http://yti.yangfankeji.com

Py:   class Admin(User): pass
来源：http://pdv.sweek.top

PHP:  class Admin extends User {}
来源：http://qub.feifeiyinyue.top

JS:   class Admin extends User {}
来源：http://fjn.pengpengdd.cyou

TS:   class Admin extends User {}
来源：http://kna.shzxlz.cn

Java: class Admin extends User {}
来源：http://zcw.fanxiaobao.xyz

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hyk.shangyingyoupin.top

Ruby: class Admin < User; end
来源：http://xzq.jqgfzy.top

C#:   class Admin : User {}
来源：http://ved.yuxming.cn

[G06] 重写方法
来源：http://mac.316326.xyz

Py:   def greet(self): return "admin"
来源：http://kwj.ybcxt.top

PHP:  public function greet(): string { return "admin"; }
来源：http://cqa.yj202588.top

JS:   greet() { return "admin"; }
来源：http://phw.shangyingyoupin.top

TS:   greet(): string { return "admin"; }
来源：http://ddm.aizwys.cn

Java: @Override String greet() { return "admin"; }
来源：http://vuy.yj20258.top

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sbq.guannengcc.top

Ruby: def greet; "admin"; end
来源：http://gpn.havefunace.top

C#:   public override string Greet() => "admin";
来源：http://dmy.sjlbkw.cn

[G07] 调用父类方法
来源：http://sdi.yanxiufei.cn

Py:   super().greet()
来源：http://wlz.316326.xyz

PHP:  parent::greet();
来源：http://ewb.jianghu66.top

JS:   super.greet();
来源：http://hcu.yuanzhike.top

TS:   super.greet();
来源：http://cuj.zhiwuduotai.top

Java: super.greet();
来源：http://ask.jqgfzy.top

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xqk.ydzc1.top

Ruby: super
来源：http://oqq.zdbjq.cn

C#:   base.Greet();
来源：http://dos.chenzaomai.com

[G08] 静态方法与属性
来源：http://qcd.yj20258.top

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fdq.jqgfzy.top

PHP:  public static function f() {}
来源：http://okz.tanke756.top

JS:   static f() {}
来源：http://xoe.pengpengdd.cyou

TS:   static f(): void {}
来源：http://vkc.gzhubu.top

Java: static void f() {}
来源：http://kkc.hammf.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bna.fktsv.cn

Ruby: def self.f; end
来源：http://jwb.guannengcc.top

C#:   public static void F() {}
来源：http://ujl.tanke756.top

[G09] 接口 / 抽象类
来源：http://tca.shanyushiyangtech.top

Py:   from abc import ABC, abstractmethod
来源：http://bqm.wangdashe.top

PHP:  interface Shape { public function area(): float; }
来源：http://uky.shzxlz.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://idj.yfazqb.com

TS:   interface Shape { area(): number; }
来源：http://klb.jyoumei.cn

Java: interface Shape { double area(); }
来源：http://cgt.havefunace.top

Go:   type Shape interface { Area() float64 }
来源：http://vax.sysykeji.top

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jxa.sysykeji.top

C#:   interface IShape { double Area(); }
来源：http://rur.vqdsnc.cn

[G10] 访问控制
来源：http://dom.redwolf501.top

Py:   约定 _protected / __private（不强制）
来源：http://hek.meibo888.top

PHP:  public / protected / private
来源：http://bez.xuetiantiany.cn

JS:   #private 字段；其余公开
来源：http://osl.zdqjudy.top

TS:   public / protected / private
来源：http://gbq.sysykeji.top

Java: public / protected / private / 默认包级
来源：http://osa.hnqzz.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://qbi.nanxuanxn.top

Ruby: public / protected / private
来源：http://udd.yfazqb.com

C#:   public / protected / private / internal
来源：http://apv.dianchejie.cn

[G11] getter / setter
来源：http://dff.chenzaomai.com

Py:   @property 与 @x.setter
来源：http://pvn.shzxlz.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jxe.nanxuanxn.top

JS:   get name() { return this._name; }
来源：http://qep.bbcook.cn

TS:   get name(): string { return this._name; }
来源：http://tch.snrcjt.cn

Java: public String getName() { return name; }
来源：http://map.jlsjyb.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://eux.gaohongyu789.top

Ruby: attr_accessor :name
来源：http://sue.daria6918.cn

C#:   public string Name { get; set; }
来源：http://tlt.ctjpmb.com

[G12] 对象转字符串
来源：http://rxa.fehbvm.com

Py:   def __str__(self): return self.name
来源：http://nvo.9152youxi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vzx.yuanzhike.top

JS:   toString() { return this.name; }
来源：http://php.smart0.xyz

TS:   toString(): string { return this.name; }
来源：http://yes.gogol.net.cn

Java: @Override public String toString() { return name; }
来源：http://zao.kuanghao11.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dhd.jinqigufen.top

Ruby: def to_s; @name; end
来源：http://esa.tian-w.cn

C#:   public override string ToString() => Name;
来源：http://paw.sxryk.cn

[G13] 判断对象类型
来源：http://ygp.cqqwz.cn

Py:   isinstance(u, User)
来源：http://rvv.hammf.cn

PHP:  $u instanceof User
来源：http://lak.nanxuanxn.top

JS:   u instanceof User
来源：http://xxb.gaohongyu789.top

TS:   u instanceof User
来源：http://qbc.smart0.xyz

Java: u instanceof User
来源：http://att.ppjwa.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qjq.andypj.xyz

Ruby: u.is_a?(User)
来源：http://qxg.bbcook.cn

C#:   u is User
来源：http://ypq.wangdashe.top

[G14] 数据类 / record
来源：http://irr.sysykeji.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vqk.smart0.xyz

PHP:  // 用 readonly 属性模拟
来源：http://cmp.sxryk.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jwe.jinyuanbaomall.cn

TS:   type User = { name: string; age: number };
来源：http://qht.316326.xyz

Java: record User(String name, int age) {}
来源：http://jhp.svipenyu.cn

Go:   type User struct { Name string; Age int }
来源：http://eqd.dianchejie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sde.xinyue.icu

C#:   record User(string Name, int Age);
来源：http://yly.yuxming.cn

[G15] 枚举
来源：http://yfs.ppjwa.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bcf.jinqigufen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://nts.jiagoushi.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tvt.c1oappe.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wmh.cqqwz.cn

Java: enum Color { RED, GREEN }
来源：http://xmy.bjfxy.top

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lga.c1oappe.top

Ruby: Color = %i[red green].freeze
来源：http://fhc.jinghuilouyu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lpp.hnqzz.top

[G16] 对象转数组 / 字典
来源：http://vnf.jqgfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tpg.yonumen.top

PHP:  get_object_vars($obj);
来源：http://koh.nanxuanxn.top

JS:   Object.entries(obj)
来源：http://okq.vehdjk.com

TS:   Object.entries(obj)
来源：http://hlz.ctjpmb.com

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ywn.jinghuilouyu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xma.sysykeji.top

Ruby: obj.instance_variables
来源：http://fzo.guowangkeji.top

C#:   // 用反射或 System.Text.Json
来源：http://ajb.yuxming.cn

================================================================================
来源：http://sah.ydzc1.top

H. 异常与错误处理
来源：http://eqp.iojbl.cn

================================================================================
来源：http://pbv.gzhubu.top

[H01] try / catch 基础
来源：http://hlx.guowangkeji.top

Py:   try: f()⏎except Exception as e: print(e)
来源：http://woc.hongshengwenyu.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xsh.yj20258.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bqb.hammf.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://psz.guannengcc.top

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vvn.yj202588.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tjs.tarul.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bzy.aibaodan.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kpi.xziqi.cn

[H02] finally / ensure 收尾
来源：http://bqz.ppjwa.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ket.cucudq.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bcr.jlsjyb.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zya.jqgfzy.top

TS:   try { f(); } finally { cleanup(); }
来源：http://fup.snrcjt.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hoz.hongshengwenyu.top

Go:   defer cleanup()             // 函数返回时执行
来源：http://ynn.yj20258.top

Ruby: begin; f; ensure; cleanup; end
来源：http://hpg.wangshuangyany.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pjw.zhengqikj.top

[H03] 主动抛出异常
来源：http://cit.ctjpmb.com

Py:   raise ValueError("错误信息")
来源：http://hjy.snrcjt.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pon.ybcxt.top

JS:   throw new Error("错误信息");
来源：http://rah.yj20258888.top

TS:   throw new Error("错误信息");
来源：http://csl.chenzaomai.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://wdp.havefunace.top

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xuz.yvedp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zpy.shanyushiyangtech.top

C#:   throw new ArgumentException("错误信息");
来源：http://sen.yj20258.top

[H04] 自定义异常类型
来源：http://geq.yuxming.cn

Py:   class MyError(Exception): pass
来源：http://knz.zhixingplan.top

PHP:  class MyError extends RuntimeException {}
来源：http://mjh.chenlongwang.top

JS:   class MyError extends Error {}
来源：http://dqh.c1oappe.top

TS:   class MyError extends Error {}
来源：http://mbd.svipenyu.cn

Java: class MyException extends RuntimeException {}
来源：http://pvl.quarkkingdee.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pkf.yonumen.top

Ruby: class MyError < StandardError; end
来源：http://fcm.hongshengwenyu.top

C#:   class MyException : Exception {}
来源：http://pbr.jianghu66.top

[H05] 捕获特定类型
来源：http://rcr.xingfuxueyuan.xyz

Py:   except ValueError as e:
来源：http://zgt.redwolf501.top

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zbt.smart0.xyz

JS:   if (e instanceof TypeError) {}
来源：http://ubn.tanke756.top

TS:   if (e instanceof TypeError) {}
来源：http://xso.zhijiandao.cn

Java: catch (IOException | SQLException e) {}
来源：http://tyq.haohaochexian.top

Go:   errors.Is(err, os.ErrNotExist)
来源：http://czg.pengpengdd.cyou

Ruby: rescue ArgumentError => e
来源：http://lin.chenlongwang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lwj.nanxuanxn.top

[H06] 可选值 / 空值安全访问
来源：http://mvx.hesvh.cn

Py:   value = d.get("k") or default
来源：http://zjg.chenzaomai.com

PHP:  $v = $d["k"] ?? null;
来源：http://eiv.zhijiandao.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vjr.fehbvm.com

TS:   obj?.a?.b;  d ?? default
来源：http://erp.hongshengwenyu.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yrt.shuidangran.top

Go:   if v, ok := m["k"]; ok { }
来源：http://ajp.chenzaomai.com

Ruby: d&.dig(:a, :b)
来源：http://mja.shanyushiyangkeji.top

C#:   obj?.A?.B ?? default
来源：http://pem.jianghu66.top

[H07] 断言
来源：http://jji.hfpthk.cn

Py:   assert x > 0, "必须为正"
来源：http://xfg.hnqzz.top

PHP:  assert($x > 0);
来源：http://vyw.yfazqb.com

JS:   console.assert(x > 0);
来源：http://oog.tianlin.xyz

TS:   console.assert(x > 0);
来源：http://swz.yvedp.cn

Java: assert x > 0 : "必须为正";
来源：http://szm.shzxlz.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gnt.pengpengdd.cyou

Ruby: raise "必须为正" unless x > 0
来源：http://yla.ctjpmb.com

C#:   Debug.Assert(x > 0);
来源：http://znm.xuanzx.com

[H08] 获取错误信息与堆栈
来源：http://vty.tianlin.xyz

Py:   str(e);  traceback.format_exc()
来源：http://lli.meibo888.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qzy.c1oappe.top

JS:   e.message;  e.stack
来源：http://vwr.xylfe.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://eot.jqgufenzy.top

Java: e.getMessage();  e.printStackTrace()
来源：http://asa.sweek.top

Go:   err.Error()
来源：http://den.zhaomingkeji.xyz

Ruby: e.message;  e.backtrace
来源：http://lzh.daxiang520.top

C#:   e.Message;  e.StackTrace
来源：http://wnk.jinqigfzy.top

[H09] 带错误码的异常
来源：http://kqn.yanxiufei.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vnm.ehwqpu.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://aru.shanyushiyangtech.top

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qrr.xingfuxueyuan.xyz

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yss.fehbvm.com

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bhe.xylfe.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://exk.chenjidiqi.icu

Ruby: raise MyError.new("fail", 500)
来源：http://toz.nanxuanxn.top

C#:   // 自定义异常类中加 Code 属性
来源：http://etz.tarul.cn

[H10] 资源自动释放
来源：http://izc.dashuyun.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qzf.ywan-chungtsiang.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ywk.yj20258.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pjz.chenzaomai.com

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ecq.sysykeji.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ayl.yueranfly.top

Go:   defer f.Close()
来源：http://jab.chenlongwang.top

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ujz.nwbrower.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pne.fanxiaobao.xyz

================================================================================
来源：http://rkw.yfazqb.com

I. 正则表达式
来源：http://zop.tian-w.cn

================================================================================
来源：http://wgl.zhaomingkeji.xyz

[I01] 判断是否匹配
来源：http://amc.chenlongwang.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://pmo.316326.xyz

PHP:  preg_match('/\d+/', $s);
来源：http://lne.yuanzhike.top

JS:   /\d+/.test(s)
来源：http://ock.shuidangran.top

TS:   /\d+/.test(s)
来源：http://ime.tarul.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rxx.aizwys.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bsd.yuanzhike.top

Ruby: s.match?(/\d+/)
来源：http://xus.chenzaomai.com

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lph.kuanghao11.cn

[I02] 提取所有匹配
来源：http://okt.quarkkingdee.top

Py:   re.findall(r"\d+", s)
来源：http://upj.yfazqb.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wzc.fehbvm.com

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ldi.yj20258.top

TS:   s.match(/\d+/g)
来源：http://kzz.jqgufenzy.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yfk.shangyingyoupin.top

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://npu.0kj1m.cn

Ruby: s.scan(/\d+/)
来源：http://ncu.havefunace.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://opn.zdqjudy.top

[I03] 提取捕获分组
来源：http://rlf.hongshengwenyu.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pfo.mhx1999.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ipt.hywenlv.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bre.nwbrower.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ais.shanyushiyangtech.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://den.nanxuanxn.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rvb.ydjk.org.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xir.cashguo.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://onw.ivvv.top

[I04] 正则替换
来源：http://rnh.ehwqpu.com

Py:   re.sub(r"\d+", "#", s)
来源：http://urn.9152youxi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://quh.ywan-chungtsiang.top

JS:   s.replace(/\d+/g, "#")
来源：http://lax.haohaochexian.top

TS:   s.replace(/\d+/g, "#")
来源：http://xki.fktsv.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qgd.xuanzx.com

Go:   re.ReplaceAllString(s, "#")
来源：http://rtz.ydjk.org.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gnx.chenjidiqi.icu

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://asp.nanxuanxn.top

[I05] 按正则拆分
来源：http://tvi.ywan-chungtsiang.top

Py:   re.split(r"\s*,\s*", s)
来源：http://dsh.zhoulong.xyz

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://okt.birdmap.top

JS:   s.split(/\s*,\s*/)
来源：http://kic.shanyushiyangkeji.top

TS:   s.split(/\s*,\s*/)
来源：http://iso.daxiang520.top

Java: s.split("\\s*,\\s*")
来源：http://jti.zhixingplan.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hku.yueranfly.top

Ruby: s.split(/\s*,\s*/)
来源：http://hej.zhiwuduotai.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zov.jqgfzy.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cta.xingfuxueyuan.xyz

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zfa.sufxvd.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cgg.hywenlv.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://scn.sxryk.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pbk.mhx1999.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sih.hnqzz.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://eac.hywenlv.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vds.hywenlv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tka.shanyushiyangkeji.top

[I07] 忽略大小写与多行模式
来源：http://rrt.ivvv.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wjl.ctjpmb.com

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tsn.zhaomingkeji.xyz

JS:   /error/gim；new RegExp("error", "gim")
来源：http://blm.snrcjt.cn

TS:   /error/gim
来源：http://sdj.shuidangran.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dlr.sufxvd.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kwt.epnwcf.com

Ruby: s.scan(/error/i)
来源：http://bve.gzhubu.top

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://icd.fzhhl.top

[I08] 贪婪与非贪婪匹配
来源：http://uup.xylfe.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kdh.ehwqpu.com

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mcr.daxiang520.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jtu.kuanghao11.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uqh.smart0.xyz

Java: Pattern.compile("<b>.*?</b>")
来源：http://emy.nwbrower.top

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cec.sufxvd.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://uhs.c1oappe.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fhk.kuanghao11.cn

================================================================================
来源：http://mof.sweek.top

J. 日期与时间
来源：http://vxc.yj20258888.top

================================================================================
来源：http://mzn.haohaochexian.top

[J01] 获取当前时间
来源：http://mnx.fehbvm.com

Py:   datetime.now();  datetime.now(UTC)
来源：http://ffj.zhijiandao.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jcq.sysykeji.top

JS:   new Date();  Date.now()
来源：http://ezc.yvedp.cn

TS:   new Date();  Date.now()
来源：http://jtk.andypj.xyz

Java: LocalDateTime.now();  Instant.now()
来源：http://jsl.vehdjk.com


<!-- 参考信息 -->